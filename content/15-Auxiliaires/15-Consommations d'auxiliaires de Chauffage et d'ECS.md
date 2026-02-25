# 15 Calcul des consommations d'auxiliaires des installations de chauffage (Caux_ch) et d'ECS (Caux_ecs)

Les consommations des auxiliaires des installations de chauffage, de refroidissement et d'ECS sont la somme des consommations des auxiliaires de génération et de distribution.

Consommation des auxiliaires des installations de chauffage :
$$C a u x_{-}c h=C a u x_{-}g e n_{-}c h+C a u x_{-}d i s t_{-}c h$$
Avec :
- Caux_gen_ch : consommation annuelle des auxiliaires de génération de l'installation de chauffage (Wh) :
$$C a u x_{-}g e n_{-}c h=Q_{a u x_{-}g_{-}c h}\,$$
- Qaux_g_ch : consommation annuelle des auxiliaires de génération de l'installation de chauffage (Wh)

- Caux_dist_ch : consommation annuelle des auxiliaires de distribution de l'installation de chauffage (Wh) Consommation des auxiliaires des installations d'ECS :
$$C a u x_{-}e c s=C a u x_{-}g e n_{-}e c s+C a u x_{-}d i s t_{-}e c s$$
Avec :
- Caux_gen_ecs : consommation annuelle des auxiliaires de génération de l'installation d'ECS (Wh)
$$C a u x_{-}g e n_{-}e c s=Q_{a u x_{-}g_{-}e c s}$$
- Qaux___ecs : consommation annuelle des auxiliaires de génération de l'installation d'ECS (Wh)

- Caux_dist_ecs : consommation annuelle des auxiliaires de distribution de l'installation d'ECS (Wh) :
$$C a u x_{-}d i s t_{-}e c s=Q_{c i r_{-}b}+Q_{t r a c}$$
- $Q_{c i r_{-}b}$ : consommation annuelle du circulateur de bouclage (Wh)
- $\mathrm{Q}_{\text {trac }}$ : consommation annuelle du traceur (Wh)


Les consommations des auxiliaires de distribution de chauffage et d'ECS sont prises nulles pour les installations individuelles en l'absence d'un circulateur externe au générateur.


Pour les installations de refroidissement, les consommations des auxiliaires de génération sont prises en compte dans le SEER (EER). Seules les consommations des auxiliaires de distribution sont donc à comptabiliser :
$$C a u x_{-}f r=C a u x_{-}d i s t_{-}f r$$
Avec :
- Caux_dist_fr : consommation annuelle des auxiliaires de distribution de l'installation de refroidissement (Wh)
