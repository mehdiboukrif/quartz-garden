# 5 Calcul des consommations d'auxiliaires de ventilation

```
Données d'entrée :
- Type de VMC
- Type de bâtiment
- Surface habitable
```

La consommation annuelle d'auxiliaires de ventilation (kWhef/an) est donnée par la formule :
$$C a u x=8760*{\frac{P v e n t_{m o y}}{1000}}$$

Avec :$\text { Pvent }_{\text {moy }} : \ puissance \ moyenne\  des\  auxiliaires \ (W)$

### Puissance moyenne en maison individuelle :

| $\text { Pvent }_{\text {moy }}$ | jusqu'à 2012 | Après 2012 |
| :------------------------------: | :----------: | :--------: |
|         Simple Flux Auto         |  65 W -ThC   | 35 W -ThC  |
|        Simple Flux hygro         |  50 W -ThC   | 15 W -ThC  |
|           Double Flux            |  80 W -ThC   | 35 W -ThC  |

Les puissances d'auxiliaires tabulées ci-dessus pour les VMC double flux intègrent les puissances du soufflage et de l'extraction.

### Puissance moyenne en immeuble collectif  :

$$
\text { Pvent }_{\text {moy }}=\text { Pvent } * \text { Qvarep }_{\text {conv }} * \text { Sh }
$$

- Qvarep conv : débit d'air extrait conventionnel par unité de surface habitable $\left(\mathrm{m}^{3} /\left(\mathrm{h} . \mathrm{m}^{2}\right)\right.$ ) ([[4-Déperditions par renouvellement d'air|Voir chapitre 4]])
- Sh : surface habitable $\left(m^{2}\right)$
- Pvent : puissance des auxiliaires $\left(\mathrm{W} /\left(\mathrm{m}^{3} / \mathrm{h}\right)\right)$ :

| $\text { Pvent }_{\text {moy }}$ |                               Jusqu'à 2012                                |                                Après 2012                                 |
| :------------------------------: | :-----------------------------------------------------------------------: | :-----------------------------------------------------------------------: |
|    Simple Flux Auto réglable     | $0,46 \mathrm{~W}-\mathrm{ThC} /\left(\mathrm{m}^{3} / \mathrm{h}\right)$ | $0,25 \mathrm{~W}-\mathrm{ThC} /\left(\mathrm{m}^{3} / \mathrm{h}\right)$ |
|    Simple Flux hygro réglable    | $0,46 \mathrm{~W}-\mathrm{ThC} /\left(\mathrm{m}^{3} / \mathrm{h}\right)$ | $0,25 \mathrm{~W}-\mathrm{ThC} /\left(\mathrm{m}^{3} / \mathrm{h}\right)$ |
|    Double Flux Auto réglable     | $1,1 \mathrm{~W}-\mathrm{ThC} /\left(\mathrm{m}^{3} / \mathrm{h}\right)$  | $0,6 \mathrm{~W}-\mathrm{ThC} /\left(\mathrm{m}^{3} / \mathrm{h}\right)$  |

Les puissances d'auxiliaires des VMC basse pression sont les mêmes que pour les VMC classiques.

Les puissances d'auxiliaires tabulées ci-dessus pour les VMC double flux intègrent les puissances du soufflage et de l'extraction.

%%Zoom sur les consos et comparatif SF/DF%%
### Ventilation Hybride :

On considère que le système bascule d'un mode mécanique à un mode naturel et inversement. Les consommations d'auxiliaire ont lieu pendant le mode de fonctionnement mécanique.

Par défaut la durée de fonctionnement de l'extracteur mécanique est prise pour le mode grand débit:

|            | Durée d'utilisation en grand débit <br> (en h/semaine) |
| :--------: | :----------------------------------------------------: |
| Collectif  |                           28                           |
| individuel |                           14                           |

Les consommations d'auxiliaires pour une VMC hybride correspondent aux consommations d'une VMC classique autoréglable de 2001 à 2012 multipliées par le ratio du temps d'utilisation :

|  | Ratio du temps d'utilisation du <br> mode mécanique |
| :---: | :---: |
| Collectif | 0,167 |
| individuel | 0,083 |
%%Zoom sur les  ventilations hybrides (cf règles profeel)%%
**Partie suivante - [[6-Apports gratuits]]**