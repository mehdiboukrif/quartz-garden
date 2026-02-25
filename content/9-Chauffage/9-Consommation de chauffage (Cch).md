#chauffage
# 9 Calcul de la consommation de chauffage (Cch)

> Données d'entrée principales:
> - Rendement de génération : Rg (sans dimension)
> - Rendement d'émission : Re (sans dimension)
> - Rendement de distribution : Rd (sans dimension)
> - Rendement de régulation : Rr (sans dimension)
> - Type d'installation de chauffage : avec ou sans solaire ; base + appoint...
> - Présence d'une ventouse (ou assistance par ventilateur) sur l'équipement

> [!Guide DPE CEREMA]
> Les règles de priorisation d’accès à la donnée sont à respecter (visuel, document justificatif, valeur par défaut). 
Les relevés suivants sont interdits : 
>- Toutes actions destructives, intégrant le démontage des chaudières par exemple.
Si vous ne pouvez pas obtenir de documentation et que vous ne pouvez pas accéder à certains équipements (en collectif notamment), il est important de choisir alors les valeurs par défaut. 
>
> Précisions sur les équipements de chauffage :  
> - Cascade de deux générateurs : 
> 	- Ne seront traités que les configurations de cascade à deux générateurs. En présence d’une cascade avec plus de deux générateurs, seuls les deux premiers de la cascade seront pris en compte. Aux deux générateurs seront  affectés la puissance totale de l’installation. La répartition des puissances des générateurs non retenus sur les 2 générateurs modélisés dans la cascade se fera de façon à maintenir le même ratio de puissance entre les deux ; 
> 	- Dans les cas des cascades avec priorité, s’il y a plus de deux générateurs, rentrer les deux plus performants. Le générateur 1 sera le plus performant ou à défaut le plus puissant et sera considéré comme  prioritaire  si  aucune  information  complémentaire  n’est  disponible. Mettre en commentaire la présence des autres (nombre et puissance de chacun si vous pouvez les avoir) ; 
> 
>
> - Les performances de l’équipement sont prises par défaut, en fonction de son type et de son année d’installation. Si aucune information n’est disponible sur son année d’installation, il faut prendre la date de construction, de rénovation du bâtiment, ou la date la plus ancienne possible le cas échéant ; 
> 
> - Il faut bien différencier une chaudière hybride et un chauffage base + appoint ; 
> 
> - Aucune  veilleuse  n’est  considérée  si  on  ne  peut  pas  la  voir.  D’autant  plus  qu’aucune  chaudière récente n’est munie d’une veilleuse ; 
> 
> - Dans le cas de convecteurs électriques, différentes technologies peuvent être installées (convecteur simple, à inertie, avec détecteur de présence, …). Un ratio de surface doit être rentré pour chaque type ; 
> 
> - Une pompe à chaleur (PAC) hybride est l’association d’une chaudière à condensation (gaz ou fioul) et d’une PAC air/eau ou eau/eau. Le système de régulation permet selon les conditions climatiques de produire la chaleur avec le générateur le plus performant.
> 
> - Si  vous  ne  pouvez  pas  récupérer  les  données  obligatoires  pour  pouvoir  réaliser  le  diagnostic (puissance des systèmes, …), vous devez saisir un chauffage fioul ; 
> 
> - Une  fiche  technique,  une  facture ou  un  compte  rendu  d’entretien  de  chaudière ne  peuvent  être acceptés que si le modèle de la chaudière installée est indiqué. Si ce n’est pas le cas il faut prendre l’année la plus défavorable (le plus récent entre le modèle et la construction). 
> 
> **Cas particulier dans le cas d’un DPE appartement (uniquement) :** 
> En présence d’une installation de production collective de chauffage, si aucune information n’est communiquée, les valeurs par défaut suivantes seront prises. 
> Dans le cas où certaines de ces informations sont connues sur l’installation collective, elles pourront être utilisées et complétées par les valeurs par défaut : 
> - Chaudière atmosphérique mixte standard datant de la construction du bâtiment ;
> - Energie utilisée par le système : fioul ; 
> - Réseau de distribution non isolé ; 
> - Chaudières avec veilleuse pour les bâtiments construits avant 2003. 

[[9.1-Installation de chauffage seule]]
[[9.1.1-Consommation de chauffage]]
[[9.1.2-Installation classique]]
[[9.1.3-Installation avec plusieurs émissions pour un même générateur]]
[[9.1.4-Installation avec plusieurs générateurs pour une même émission]]
[[9.2-Chauffage solaire]]
[[9.3-Insert ou poêle bois en appoint]]
[[9.4-Insert, poêle bois (ou biomasse) en appoint avec un chauffage électrique dans la salle de bains]]
[[9.5 Insert ou poêle bois en appoint et un chauffage électrique dans la salle de bains (différent du chauffage principal)]]
[[9.6-Chauffage solaire et insert ou poêle bois en appoint]]
[[9.7-Chaudière en relève de PAC avec insert ou poêle bois en appoint]]
[[9.8-Chauffage collectif avec base+appoint]]
[[9.9-Convecteur bi-jonction]]
[[9.10-Installations différentes et indépendantes couplées ou non]]
[[9.11-Générateur bi-énergie]]
