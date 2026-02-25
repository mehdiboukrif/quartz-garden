# 3 Calcul des déperditions de l'enveloppe GV 

 ```
Données d'entrée :
- Caractéristiques de l'enveloppe (linéaires, surfaces, U )
- Surface des parois déperditives i (murs, plafonds, planchers, baies, portes)
- Linéaires de ponts thermiques
 ```
 
La somme GV des déperditions par les parois et par renouvellement d'air (W/K) s'exprime de la manière suivante :

$$G V=D P m u r ~+D P p l a n c h e r_{\_} b a s+D P p l a n c h e r_{-} h a u t+D P m e n u i s e r i e+P T+D R$$

Avec :

- PT : déperditions par les ponts thermiques (W/K) ([[3.4-Déperditions ponts thermiques|voir partie 3.4]])
- DR : déperditions par le renouvellement d'air (W/K) ([[4-Déperditions par renouvellement d'air|voir partie 4]])
- DPparoi : déperdition par la paroi (W/K) :

$$\begin{array}{c}{{D P m u r=\displaystyle\sum_{i}b_{i}\ast\,S m u r_{i}\ast\,U m u r_{i}}}\\ {{\nonumber}}\\ {{D P p l a n c h e r\_b a s=\displaystyle\sum_{i}b_{i}\ast\,S p b_{i}\ast\,U p b_{i}}}\\ {{\nonumber}}\\ {{\nonumber}}\\ {{D P p l a n c h e r\_h a u t=\displaystyle\sum_{i}b_{i}\ast\,S p h_{i}\ast\,U p h_{i}}}\\ {{\nonumber}}\\ {{\nonumber}}\\ {{D P m e n u i s e r i e=\displaystyle\sum_{i}b_{i}\ast\,S m e n u i s e r i e_{i}\ast\,U m e n s u i s e r i e_{i}}}\end{array}$$

Avec :

- $b_{i}:$ coefficient de réduction des déperditions pour la paroi i ([[3.1-Coefficient réduction b|voir partie 3.1]])
- Sparoi $i$ : surface de la paroi déperditive i $\left(\mathrm{m}^{2}\right)$
- Uparoi $i_{i}$ : coefficient de transmission thermique de la paroi i $\left(\mathrm{W} /\left(\mathrm{m}^{2} . \mathrm{K}\right)\right)$ (voir [[3.2-U des parois opaques|partie 3.2]] et [[3.3-U parois vitrées et portes|partie 3.3]] )

On appelle menuiserie l'ensemble vitrage-protection solaire des fenêtres, portes-fenêtres et portes.

Attention : Les parois donnant sur un bâtiment autre que d'habitation sont aussi considérées déperditives.

La surface prise en compte pour l'établissement du DPE est la surface habitable du bâtiment. Cette surface intègre les vérandas chauffées (voir [[6.3-Espaces tampons solarisés (ETS)]]).

> [!quote]- Extrait guide du diagnostiqueur - **ZOOM Surface**
> 
> La surface prise en compte pour l'établissement du DPE est la surface de référence définie par l'arrêté du 25 mars 2024 : *« Cette surface est la surface habitable du bâtiment, à laquelle il est ajoutée les surfaces des vérandas chauffées ainsi que les surfaces des locaux chauffés pour l'usage principal d'occupation humaine, d'une hauteur sous plafond d'au moins 1,80 m. »*
> 
> Elle consiste à évaluer la surface d'un bien immobilier en tenant compte de son état physique et de sa situation matérielle au moment de la visite du diagnostic, sans interprétation des critères d'habitabilité, mais en incluant la notion de surface chauffée pour l’usage principal d’occupation humaine susceptible d'influencer les consommations énergétiques d'un bâtiment d’habitation.
> ![[Pasted image 20241201145715.png]]
> 


> La surface de référence définie pour le DPE n’a pas vocation à vérifier les critères établis dans : 
- la surface de la partie privative soumis aux dispositions de l’article 46 de la loi du 10 juillet 1965 (surface dite « Carrez »)  ; 
- la surface utile définie par l’article R.353-16 du CCH ; 
- toute autre surface définie par des textes concernant 
	- l’habitabilité définie dans le Code de la santé publique ; 
	- la décence à l’occupation humaine définie par le Décret n°2002-120 du 30 janvier 2002. 

**Pour obtenir la surface de référence, plusieurs cas se présentent :** 
- Un  certificat  de  surface  habitable  est réalisé  (cas  d’un  bail  en  maison)  →  il  est  accepté comme preuve ; 
- Les vérandas chauffées devront être ajoutées si ce n’est pas déjà le cas, ainsi que les surface des locaux chauffés pour l’usage principal d’occupation humaine d’une hauteur sous plafond d’au moins 1,80 mètres. 
- Un des documents suivants est fourni par le propriétaire → étude thermique réglementaire (RT-Ex, RT2005, RT2012, RE2020), plans d’exécution. 
- Le syndic de copropriété ou le bailleur social fournit la surface habitable de l’immeuble ainsi que la surface de chacun des lots → obligatoire pour la réalisation d’un DPE collectif ; 

**Dans tous les autres cas**  
- le diagnostiqueur doit mesurer la surface de référence 
- Le diagnostiqueur doit vérifier la cohérence des documents fournis avec le bien examiné 




[[Lexique - Guide CEREMA-Juillet 2024-V3]]


![[Pasted image 20241201151645.png]]

En présence d'un espace non habitable chauffé (par exemple un garage ou un sous-sol), cet espace est traité dans le DPE comme un espace non chauffé. Dans ce cas, le diagnostiqueur ==devra obligatoirement mentionner dans le rapport que cet espace ne doit pas être chauffé et intégrer ce commentaire dans la justification des écarts entre les factures et les consommations conventionnelles.

**Parties suivantes**
[[3.1-Coefficient réduction b]]
[[3.2.1-U mur]]
[[3.2.2-U plancher bas (Upb)]]
[[3.2.3-U plancher haut (Uph)]]
[[3.3-U parois vitrées et portes]]
[[3.3.1-Performance du vitrage]]
[[3.3.3-Ujn fenêtres et portes-fenêtres]]
[[3.3.4-Ud des portes]]
[[3.4-Déperditions ponts thermiques]]
[[3.4.1-Mur et Plancher bas]]
[[3.4.2-Mur et Plancher intermédiaire]]
[[3.4.3-Mur et Plancher haut]]
[[3.4.4-Mur et Refend]]
[[3.4.5-Menuiserie et mur]]