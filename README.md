# whitepaper-zoc
The White Paper for the ZOC (Zombie On Chain) Tracker methodology.

# ZOC Tracker : Un outil d'analyse et de classification des contrats intelligents "Zombie On Chain"

Le projet **ZOC Tracker** introduit une nouvelle taxonomie et une méthodologie pour identifier les contrats intelligents déployés mais fonctionnellement abandonnés ou économiquement négligeables sur la blockchain.

## Le Concept ZOC (Zombie On Chain)

Le terme ZOC est utilisé pour désigner le **code persistant mais non fonctionnel**. Ce phénomène est une conséquence structurelle de l'immuabilité de la blockchain, conduisant à l'accumulation de "débris numériques".

Un contrat est classifié ZOC s'il répond à deux critères quantifiables :

1.  **Critère Temporel (X) :** Une inactivité externe continue d'au moins **neuf mois** (hypothèse de travail initiale).
2.  **Critère de Valeur (Y) :** Une valeur économique totale **négligeable** (Balance native < 0.001 ETH et actifs secondaires < 10 USD - seuils ajustables).

## Le White Paper Complet

Pour la définition formelle des critères (y compris la classification ZOC : Inerte, Verrouillé, Dangereux, Abandonné) et la méthodologie détaillée de l'algorithme, veuillez consulter notre article technique complet.

**[Lire le White Paper Complet : WHITEPAPER_ZOC.pdf]**

## Objectifs du ZOC Tracker

L'outil analytique vise à transformer ce diagnostic en opportunité :
* **Audit de Chaîne :** Fournir une métrique honnête de la vitalité des réseaux.
* **Sécurité et Éducation :** Identifier les contrats dangereux (failles connues) ou verrouillés (fonds piégés) pour l'audit.
* **Récupération de Trafic :** Identifier les **ZOC Abandonnés** qui reçoivent encore des appels résiduels, proposant des solutions (ex: implémentation d'un contrat proxy) pour rediriger ce trafic vers des protocoles sains.

## Contribution

Nous accueillons les contributions de la communauté sur les points suivants :
* Validation empirique des critères (X et Y).
* Développement du pipeline d'indexation (voir Section 3.1 du White Paper).
* Implémentation des modèles de classification ZOC.
