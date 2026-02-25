# 8 Modélisation de l'intermittence

>   Données d'entrée
> - Type de bâtiment
> - Type de chauffage (divisé, central)
> - Type de régulation (par pièce ou non)
> - Equipement d'intermittence (absent, central sans minimum de température, ...)
> - Type d'émetteur (air soufflé, convecteurs, ...)
> - Présence d'un comptage
> - Hauteur moyenne sous plafond

Le facteur d'intermittence traduit les baisses temporaires de température, réalisées pour différentes raisons, absence, ralenti de nuit et éventuellement de façon inégale dans les pièces.

Il est égal au rapport entre les besoins réels, compte tenu d'un comportement moyen des occupants, et les besoins théoriques. Le facteur d'intermittence est donné par la formule :

$$
I N T=\frac{I o}{1+0,1 *(G-1)}
$$

Avec :

$$
G=\frac{G V}{H s p * S h}
$$

- GV : déperditions annuelles de l'enveloppe (W/K) (déterminé en [[3-Déperditions GV]])
- Sh : surface habitable (m²)
- Hsp : hauteur moyenne sous plafond (m)

## Facteur I0 - maisons individuelles - (chauffage individuel)

### Chauffage divisé
#### Inertie légère ou moyenne
**Équipements d'intermittence**

| Type de Régulation | Type Chauffage             | Absent | Central sans <br> minimum de <br>température | Central avec <br> minimum de <br>température | Par pièce avec <br> minimum de <br>température | Par pièce avec <br> minimum de <br>température et <br> détection de <br> présence |
| ------------------ | -------------------------- | :----: | :------------------------------------------: | :------------------------------------------: | :--------------------------------------------: | :-------------------------------------------------------------------------------: |
| Pièce par pièce    | Air soufflé                |  0,84  |                     0,83                     |                     0,81                     |                      0,77                      |                                       0,75                                        |
| Pièce par pièce    | Radiateur / <br>Convecteur |  0,84  |                     0,83                     |                     0,81                     |                      0,77                      |                                       0,75                                        |
| Pièce par pièce    | Plafond chauffant          |  0,84  |                     0,83                     |                     0,81                     |                      0,77                      |                                       0,75                                        |
| Pièce par pièce    | Plancher chauffant         |  0,90  |                     0,89                     |                     0,88                     |                      0,86                      |                                         -                                         |

#### Inertie lourde ou très lourde
(Chauffage divisé)

| Type de Régulation (AVEC ou SANS régulation pièce par pièce) | Type Chauffage             | Absent | Central sans <br> minimum de <br>température | Central avec <br> minimum de <br>température | Par pièce avec <br> minimum de <br>température | Par pièce avec <br> minimum de <br>température et <br> détection de <br> présence |
| ------------------------------------------------------------ | -------------------------- | :----: | :------------------------------------------: | :------------------------------------------: | :--------------------------------------------: | :-------------------------------------------------------------------------------: |
| **Avec**                                                     | Air soufflé                |  0,86  |                     0,85                     |                     0,83                     |                      0,80                      |                                       0,78                                        |
| **Avec**                                                     | Radiateur / <br>Convecteur |  0,86  |                     0,85                     |                     0,83                     |                      0,80                      |                                       0,78                                        |
| **Avec**                                                     | Plafond chauffant          |  0,86  |                     0,85                     |                     0,83                     |                      0,80                      |                                       0,78                                        |
| **Avec**                                                     | Plancher chauffant         |  0,92  |                     0,91                     |                     0,90                     |                      0,88                      |                                         -                                         |

### Chauffage central
#### Inertie légère ou moyenne

| Type de Régulation (AVEC ou SANS régulation pièce par pièce) | Type Chauffage             | Absent | Central sans <br> minimum de <br>température | Central avec <br> minimum de <br>température | Par pièce avec <br> minimum de <br>température | Par pièce avec <br> minimum de <br>température et <br> détection de <br> présence |
| ------------------------------------------------------------ | -------------------------- | :----: | :------------------------------------------: | :------------------------------------------: | :--------------------------------------------: | :-------------------------------------------------------------------------------: |
| **Avec**                                                     | Air soufflé                |  0,86  |                     0,85                     |                     0,83                     |                      0,79                      |                                       0,77                                        |
| **Avec**                                                     | Radiateur / <br>Convecteur |  0,88  |                     0,87                     |                     0,85                     |                      0,82                      |                                       0,80                                        |
| **Avec**                                                     | Plafond chauffant          |  0,88  |                     0,87                     |                     0,85                     |                      0,82                      |                                       0,80                                        |
| **Avec**                                                     | Plancher chauffant         |  0,90  |                     0,89                     |                     0,88                     |                      0,86                      |                                         -                                         |
| **Sans**                                                     | Air soufflé                |  0,90  |                     0,89                     |                     0,87                     |                       -                        |                                                                                   |
| **Sans**                                                     | Radiateur                  |  0,91  |                     0,90                     |                     0,88                     |                       -                        |                                                                                   |
| **Sans**                                                     | Plafond chauffant          |  0,91  |                     0,90                     |                     0,88                     |                       -                        |                                                                                   |
| **Sans**                                                     | Plancher chauffant         |  0,92  |                     0,91                     |                     0,90                     |                       -                        |                                                                                   |

#### Inertie lourde ou très lourde
(Chauffage central)

| Type de Régulation (AVEC ou SANS régulation pièce par pièce) | Type Chauffage         | Absent | Central sans <br> minimum de <br>température | Central avec <br> minimum de <br>température | Par pièce avec <br> minimum de <br>température | Par pièce avec <br> minimum de <br>température et <br> détection de <br> présence |
| ------------------------------------------------------------ | ---------------------- | :----: | :------------------------------------------: | :------------------------------------------: | :--------------------------------------------: | :-------------------------------------------------------------------------------: |
| **Avec**                                                     | Air soufflé            |  0,88  |                     0,87                     |                     0,85                     |                      0,82                      |                                       0,80                                        |
| **Avec**                                                     | Radiateur / Convecteur |  0,90  |                     0,89                     |                     0,87                     |                      0,85                      |                                       0,82                                        |
| **Avec**                                                     | Plafond chauffant      |  0,90  |                     0,89                     |                     0,87                     |                      0,85                      |                                       0,82                                        |
| **Avec**                                                     | Plancher chauffant     |  0,92  |                     0,91                     |                     0,90                     |                      0,88                      |                                         -                                         |
| **Sans**                                                     | Air soufflé            |  0,91  |                     0,91                     |                     0,89                     |                       -                        |                                                                                   |
| **Sans**                                                     | Radiateur              |  0,93  |                     0,92                     |                     0,90                     |                       -                        |                                                                                   |
| **Sans**                                                     | Plafond chauffant      |  0,93  |                     0,92                     |                     0,90                     |                       -                        |                                                                                   |
| **Sans**                                                     | Plancher chauffant     |  0,94  |                     0,93                     |                     0,92                     |                       -                        |                                                                                   |

Une maison individuelle branchée sur un réseau collectif de fourniture d'énergie pour le chauffage sera traitée comme une maison individuelle avec un chauffage individuel central.

## Facteur I0 Pour les immeubles collectifs avec chauffage individuel

### Chauffage *individuel* et divisé

| Type de Régulation (AVEC ou SANS régulation pièce par pièce) |                      | Absent | Central sans <br> minimum de <br>température <br> | Central avec <br> minimum de  température <br> | Par pièce avec <br> minimum de  température <br> | Par pièce avec minimum <br> de température et <br> détection de présence <br> |
| ------------------------------------------------------------ | -------------------- | :----: | :-----------------------------------------------: | :--------------------------------------------: | :----------------------------------------------: | :---------------------------------------------------------------------------: |
| **Avec**                                                     | Air soufflé          |  0,90  |                       0,89                        |                      0,88                      |                       0,86                       |                                     0,83                                      |
| **Avec**                                                     | Radiateur/Convecteur |  0,90  |                       0,89                        |                      0,88                      |                       0,86                       |                                     0,83                                      |
| **Avec**                                                     | Plafond chauffant    |  0,90  |                       0,89                        |                      0,88                      |                       0,86                       |                                     0,83                                      |
| **Avec**                                                     | Plancher chauffant   |  0,95  |                       0,94                        |                      0,93                      |                       0,91                       |                                       -                                       |

### Chauffage *individuel* et central

| Type de Régulation (AVEC ou SANS régulation pièce par pièce) |                    | Absent | Central sans <br> minimum de <br>température <br> | Central avec <br> minimum de  température <br> | Par pièce avec <br> minimum de  température <br> | Par pièce avec minimum <br> de température et <br> détection de présence <br> |
| :----------------------------------------------------------: | :----------------: | :----: | :-----------------------------------------------: | :--------------------------------------------: | :----------------------------------------------: | :---------------------------------------------------------------------------: |
|                           **Avec**                           |    Air soufflé     |  0,91  |                       0,90                        |                      0,89                      |                       0,87                       |                                     0,84                                      |
|                           **Avec**                           |     Radiateur      |  0,93  |                       0,92                        |                      0,91                      |                       0,89                       |                                     0,86                                      |
|                           **Avec**                           | Plafond chauffant  |  0,93  |                       0,92                        |                      0,91                      |                       0,89                       |                                     0,86                                      |
|                           **Avec**                           | Plancher chauffant |  0,95  |                       0,94                        |                      0,93                      |                       0,91                       |                                       -                                       |
|                           **Sans**                           |    Air soufflé     |  0,95  |                       0,94                        |                      0,93                      |                        -                         |                                       -                                       |
|                           **Sans**                           |     Radiateur      |  0,96  |                       0,95                        |                      0,94                      |                        -                         |                                       -                                       |
|                           **Sans**                           | Plafond chauffant  |  0,96  |                       0,95                        |                      0,94                      |                        -                         |                                       -                                       |
|                           **Sans**                           | Plancher chauffant |  0,97  |                       0,96                        |                      0,95                      |                        -                         |                                       -                                       |


## Facteur I0 Pour les immeubles collectifs avec chauffage collectif
### Absence de comptage individuel

| Type de Régulation (AVEC ou SANS régulation pièce par pièce) |  Type d'émetteurs  | Absent | Central collectif | Central collectif avec détection de présence |
| :----------------------------------------------------------: | :----------------: | :----: | :---------------: | :------------------------------------------: |
|                           **Avec**                           |    Air soufflé     |  1,01  |       0,99        |                     0,96                     |
|                           **Avec**                           |     Radiateur      |  1,03  |       1,01        |                     0,98                     |
|                           **Avec**                           | Plafond chauffant  |  1,03  |       1,01        |                     0,98                     |
|                           **Avec**                           | Plancher chauffant |  1,05  |       1,03        |                                              |
|                           **Sans**                           |    Air soufflé     |  1,03  |       1,01        |                                              |
|                           **Sans**                           |     Radiateur      |  1,05  |       1,03        |                                              |
|                           **Sans**                           | Plafond chauffant  |  1,05  |       1,03        |                                              |
|                           **Sans**                           | Plancher chauffant |  1,07  |       1,05        |                                              |
   
### Présence d'un comptage individuel

| Type de Régulation (AVEC ou SANS régulation pièce par pièce) |  Type d'émetteurs  | Absent | Central collectif | Central collectif avec détection de présence |
| :----------------------------------------------------------: | :----------------: | :----: | :---------------: | :------------------------------------------: |
|                             Avec                             |    Air soufflé     |  0,93  |       0,91        |                     0,88                     |
|                             Avec                             |     Radiateur      |  0,95  |       0,93        |                     0,90                     |
|                             Avec                             | Plafond chauffant  |  0,95  |       0,93        |                     0,90                     |
|                             Avec                             | Plancher chauffant |  0,97  |       0,95        |                                              |
|                             Sans                             |    Air soufflé     |  0,95  |       0,93        |                                              |
|                             Sans                             |     Radiateur      |  0,97  |       0,95        |                                              |
|                             Sans                             | Plafond chauffant  |  0,97  |       0,95        |                                              |
|                             Sans                             | Plancher chauffant |  0,99  |       0,97        |                                              |

En immeuble collectif, le chauffage mixte, c'est-à-dire dont une partie est facturée collectivement et une autre individuellement, est traité au niveau de l'intermittence comme un système collectif avec comptage individuel.

Seule l'intermittence de l'appoint est prise en compte sur les installations base + appoint. Une régulation zonale peut être considérée comme une régulation pièce par pièce.

L'équipement d'intermittence peut être :

- En chauffage individuel
	- Absent : pas d'équipement permettant de programmer des réduits de température ;
	- Central sans minimum de température : équipements permettant une programmation seulement de la fonction marche arrêt et donc ne garantissant pas un minimum de température ;
	- Central avec un minimum de température : équipement pouvant assurer :
		- Centralement un ralenti ou un abaissement de température fixe, non modifiable par l'occupant, ainsi que la fonction hors gel ;
		- Centralement un ralenti ou un abaissement de température au choix de l'occupant ;
	- Pièce par pièce avec minimum de température : équipement permettant d'obtenir par pièce un ralenti ou un abaissement de température fixe, non modifiable par l'occupant.

- En chauffage collectif
	- Absent : pas de réduit de nuit ;
	- Central collectif : possibilité de ralenti de nuit.

Un plancher chauffant avec une régulation zone jour/zone nuit peut être associée à une régulation pièce par pièce.

Un poêle sera modélisé comme un radiateur/convecteur pour la détermination de l'intermittence

Un système de chauffage divisé est un système pour lequel la génération et l'émission sont confondues. C'est le cas des convecteurs électriques, planchers chauffants électriques, ...

Un système de chauffage central comporte un générateur central, individuel ou collectif, et une distribution par fluide chauffant : air ou eau.

**Partie suivante** [[9-Consommation de chauffage (Cch)]]