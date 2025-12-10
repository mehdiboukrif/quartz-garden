# Quartz Static Site Generator with SPA Routing

## Overview

This is a Quartz v4.5.2 static site generator that transforms Obsidian notes (Markdown) into a website with Single Page Application (SPA) routing capabilities. The site provides fast navigation without full page reloads and includes support for third-party integrations like comment systems (Hyvor Talk) and GitHub-based discussions (Giscus).

**Key Features:**
- Static site generation from Markdown files
- SPA routing via custom `nav` events for seamless navigation
- Dynamic content updates without page reloads
- Theme switching (light/dark mode) with persistence
- Code syntax highlighting with copy-to-clipboard functionality
- Mermaid diagram support with modal viewing
- Multi-language support (French/English)
- Tag-based content organization

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture

**Static Site Generation**: The application uses Quartz as a static site generator that compiles Markdown files into HTML pages. Each page is pre-rendered at build time with consistent layouts and styling.

**SPA Routing System**: Instead of traditional multi-page navigation, the site implements client-side routing:
- Custom `nav` event dispatched on page transitions
- Content area dynamically updated without full page reloads
- Browser history management for proper back/forward navigation
- URL updates reflect current page without triggering server requests

**Rationale**: SPA routing provides instant navigation between pages, creating a more app-like experience while maintaining the SEO benefits of pre-rendered static HTML.

**Component-Based Structure**: The site uses a modular component approach with:
- Reusable UI components for headers, navigation, and content areas
- Script-based components (`prescript.js`, `postscript.js`) for initialization and cleanup
- Event-driven architecture for component lifecycle management

**Theme System**: Dual-theme support (light/dark) with:
- System preference detection via `prefers-color-scheme` media query
- LocalStorage persistence for user theme choice
- `saved-theme` attribute on document root for CSS targeting
- Pre-render script (`prescript.js`) to prevent flash of unstyled content

**Pros**: Fast theme switching, no flash during page load, respects user preferences
**Cons**: Requires JavaScript; users with JS disabled see default theme only

### Content Management

**Markdown Processing**: Obsidian-formatted Markdown files are transformed into HTML with:
- Automatic link resolution between pages
- Tag extraction for categorization
- Content indexing for search functionality (via `contentIndex.json`)

**Content Index**: A JSON-based content registry (`static/contentIndex.json`) that maps:
- Page slugs to file paths
- Titles and metadata
- Internal links and backlinks
- Tags for filtering and discovery

**Alternative Considered**: Database-backed content management was not needed since all content is static and generated at build time. JSON indexing provides sufficient query capabilities for client-side search.

### Code Enhancement Features

**Syntax Highlighting**: Code blocks include:
- Language-specific syntax highlighting
- Copy-to-clipboard buttons that appear on hover
- Visual feedback on successful copy operations
- Cleanup handlers to prevent memory leaks during SPA navigation

**Mermaid Diagrams**: Interactive diagram rendering with:
- Modal overlay for full-screen viewing
- Backdrop blur effect for focus
- Click-outside-to-close functionality
- Fixed positioning to prevent scroll issues

### Asset Management

**Static Assets**: All static resources are compiled into the `public/` directory:
- Minified CSS for production performance
- Bundled JavaScript with tree-shaking
- Optimized images and fonts
- Pre-generated HTML pages

**CSS Architecture**: Uses CSS custom properties (variables) for theming:
- `--light`, `--dark`, `--gray` for base colors
- `--primary`, `--secondary`, `--tertiary` for accent colors
- Per-theme syntax highlighting variables (giscus integration)

### Error Handling

**404 Page**: Custom not-found page (`404.html`) that:
- Maintains site navigation and styling
- Provides helpful links back to main content
- Supports the same SPA routing as other pages

## External Dependencies

### Comment System Integration (Hyvor Talk)

**Service**: Hyvor Talk commenting platform
**Website ID**: 11990
**Integration Challenge**: The project documentation reveals a critical incompatibility between Hyvor Talk's `embed.js` script and SPA routing.

**Problem**: The Hyvor Talk widget fails when the `<hyvor-talk-comments>` element is dynamically recreated during SPA navigation, throwing:
```
NotFoundError: Failed to execute 'removeChild' on 'Node'
```

**Attempted Solutions**:
1. Dynamic component recreation on `nav` events - resulted in infinite loading loops
2. `HyvorTalk.reload()` API - widget loaded but failed to isolate comments per page
3. Explicit page ID passing to `reload(page_id, page_url)` - API ignored parameters

**Current Status**: Integration is incomplete due to third-party script limitations. Alternative solutions may include server-side rendering of comments or switching to a different comment provider.

### Alternative Comment System (Giscus)

**Service**: GitHub Discussions-based commenting
**Styling**: Custom CSS themes for both light and dark modes located in `public/static/giscus/`

**Rationale**: Giscus uses GitHub's infrastructure, making it free and well-suited for technical/developer-focused content. It leverages existing GitHub authentication.

**Integration Points**:
- Custom CSS variables map Quartz theme colors to Giscus UI
- Theme switching synchronized between site and comment widget
- GitHub repository required for hosting discussions

**Pros**: Free, developer-friendly, no vendor lock-in, markdown support
**Cons**: Requires GitHub account to comment, not ideal for general audiences

### Font Loading

**Service**: Google Fonts API
**Implementation**: Preconnect hints for performance optimization
```html
<link rel="preconnect" href="https://fonts.googleapis.com"/>
<link rel="preconnect" href="https://fonts.gstatic.com"/>
```

**Rationale**: Preconnect establishes early connections to font servers, reducing latency when fonts are requested.

### Build & Deployment

**Platform**: GitHub Pages (inferred from documentation URL: `mehdiboukrif.github.io`)
**Build Process**: Static files generated to `public/` directory
**Deployment**: Automated GitHub Actions workflow (standard for GitHub Pages + Quartz)

**Content Source**: Obsidian vault containing Markdown notes
**Output**: Static HTML/CSS/JS bundle deployed to CDN

### Browser APIs

**LocalStorage**: Theme preference persistence
**History API**: SPA routing and navigation state management
**MatchMedia API**: System theme preference detection
**Clipboard API**: Code copying functionality