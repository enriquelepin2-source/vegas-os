# VEGAS-OS // Terminal Casino 🎰

**VEGAS-OS** est un simulateur de casino interactif et immersif entièrement développé en un seul fichier (**Single-File App**) avec **HTML5, Tailwind CSS et JavaScript pur**. Présenté sous la forme d'un terminal de commande rétro/cyberpunk (inspiré des environnements cathodiques CRT), il intègre un système complet d'authentification utilisateur, un catalogue varié de jeux de casino, un système de séries de victoires dynamiques 🔥, une gestion VIP évolutive, un moteur sonore Web Audio API synthétisé et des thèmes graphiques déblocables via une boutique intégrée.

## 🚀 Fonctionnalités principales

* **Terminal Interactif Rétro (CRT) :**
  * Effets visuels d'écran cathodique (lignes de balayage / *scanlines*, lueur de phosphore, courbure et vignette d'écran).
  * Navigation fluide en ligne de commande avec auto-complétion contextuelle (`Tab`) et historique des commandes (`Flèche Haut / Bas`).
  * Barre de raccourcis rapides cliquables et personnalisables en bas d'écran (ajout, retrait et réinitialisation).
  * HUD supérieur en temps réel : utilisateur connecté, solde en banque, dette active, rang VIP et compteur de séries de victoires 🔥.

* **Catalogue de Jeux de Casino :**
  * 🎰 **Slots (Machine à sous) :** Rouleaux virtuels pondérés, remboursements sur cerises et gains multipliés jusqu'au Jackpot Suprême `[ 7 ] [ 7 ] [ 7 ]` ($\times 77$).
  * ♠️ **Blackjack (Table 21) :** Table complète avec tirage dynamique de cartes, options de tirage (*hit*), maintien (*stand*), doublage de mise (*double*) et **Split de paire** (séparation stricte de deux cartes de même rang pour jouer deux mains distinctes).
  * 🃏 **Ultimate Texas Hold'em (Poker) :** Affrontez la main du croupier en face-à-face avec mise initiale Ante + Blind, décisions d'enchère Play modulables (Play $\times 4$ préflop, Play $\times 2$ au flop, Play $\times 1$ à la river) et règle de qualification du croupier.
  * 🎡 **Roulette Européenne :** Cylindre de 37 cases (0 à 36), paris sur numéros pleins ($\times 36$), chances simples (Rouge/Noir, Pair/Impair, Manque/Passe) et douzaines (d1, d2, d3).
  * 🚀 **Crash (Fusée) :** Multiplicateur exponentiel en temps réel où le joueur doit s'éjecter à temps (`stop` / `cash`) avant l'explosion inopinée.
  * 🎲 **Dés (2D6) :** Lancer de deux dés à 6 faces avec calcul dynamique des cotes mathématiques selon les conditions de somme choisies (`sup` ou `inf`).

* **Systèmes Avancés & Économie :**
  * **Système de Séries 🔥 :** Enchaînez les victoires consécutives pour bénéficier d'un bonus progressif de $+1\%$ par palier de victoire. Les égalités (*push*) préservent la série en cours.
  * **Statistiques Détaillées & Probabilités :** Suivi individuel des taux de victoires par jeu (`stats`) et commande dédiée (`proba`) pour consulter les cotes exactes, la distribution des mains et les taux de retour (RTP).
  * **Hiérarchie VIP Évolutive :** Paliers automatiques basés sur votre capital (Bronze, Argent, Or, Platinum et Diamant).
  * **Aide Financière du Cartel :** Subvention périodique (`bonus`) ajustée à votre rang VIP (recharge toutes les 3 minutes) et système d'emprunt d'urgence (`emprunt` / `rembourser`, jusqu'à 5 000 \$ avec 30% d'intérêts).

* **Audio & Personnalisation Graphique :**
  * **Moteur Sonore Procédural (Web Audio API) :** Bruitages synthétiques rétro (frappe de touche, bips, lancers, gains, explosions) et musique d'ambiance cybernétique en boucle générée en direct, sans aucun fichier audio externe.
  * **Boutique de Thèmes CRT :** Débloquez et équipez différentes ambiances visuelles (`Matrix`, `Vert CRT`, `Ambre`, `Cyberpunk`, `Crimson Cyber`, `Or Impérial`).
  * **Persistance Locale :** Sauvegarde automatique des profils, mots de passe, soldes, statistiques et raccourcis via le stockage local (`localStorage`).

## 🛠️ Installation & Loi du Fichier Unique

Le projet applique rigoureusement le principe du **Fichier Unique (Single-File Mandate)** : l'intégralité du code (structure HTML5, styles Tailwind CSS et scanlines CRT, moteur sonore Web Audio API et moteur de jeu JavaScript) est contenue dans le fichier autonome `index.html` (ou `VEGAS-OS.html`).

### Pour lancer l'application localement :

1. Téléchargez ou clonez le dépôt sur votre machine :
   ```bash
   git clone https://gitlab.univ-nantes.fr/E253676K/vegas-os.git
   cd vegas-os
   ```

2. Ouvrez simplement le fichier **`index.html`** directement dans n'importe quel navigateur web moderne (*Google Chrome, Mozilla Firefox, Microsoft Edge, Safari, Brave*). Aucun serveur applicatif ni installation de dépendances (npm, python) n'est requis !

## 🎮 Commandes principales du Terminal

Une fois connecté avec votre nom d'utilisateur, tapez directement vos commandes dans le terminal :

| Commande | Syntaxe / Exemple | Description |
| :--- | :--- | :--- |
| `help` | `help [jeu]` | Affiche le catalogue général ou les règles spécifiques d'un jeu. |
| `proba` | `proba [jeu]` | Affiche les analyses mathématiques, cotes et taux de retour (RTP). |
| `slots` | `slots <mise\|all>` | Lance la machine à sous virtuelle *(alias: `slot`)*. |
| `blackjack` | `bj <mise\|all>` | Ouvre la table de Blackjack interactive 21 *(alias: `bj`)*. |
| `poker` | `poker <mise\|all>` | Démarre une table d'Ultimate Texas Hold'em *(alias: `ultimate`, `uth`)*. |
| `roulette` | `roulette <mise\|all> <pari>` | Lance une partie de roulette européenne (ex: `roulette 50 rouge`). |
| `crash` | `crash <mise\|all>` | Lance le mini-jeu de la fusée (tapez `stop` ou `cash` pour vous éjecter). |
| `dés` | `dés <mise\|all> <sup\|inf> <n>` | Parie sur la somme de 2D6 de 3 à 11 (ex: `dés 50 sup 7`). |
| `profil` | `profil` | Affiche votre dossier joueur, solde, valeur nette, records et série $\🔥$. |
| `vip` | `vip` | Affiche les avantages, subventions et conditions de la hiérarchie VIP. |
| `stats` | `stats [jeu]` | Affiche les bilans complets et taux de réussite globaux ou par jeu. |
| `bonus` | `bonus` | Réclame l'allocation financière du cartel selon votre palier VIP. |
| `emprunt` | `emprunt <montant>` | Emprunte des jetons au cartel (plafond 5 000 \$, intérêt 30%). |
| `rembourser` | `rembourser [montant\|all]` | Rembourse tout ou partie de votre dette active. |
| `theme` | `theme [nom]` / `theme buy [nom]` | Change de palette d'affichage ou achète un nouveau thème CRT. |
| `settings` | `settings` | Ouvre la fenêtre graphique de configuration sonore et raccourcis. |
| `logout` | `logout` | Sauvegarde la session en cours et retourne à l'écran de connexion. |
| `clear` | `clear` | Nettoie l'affichage du terminal *(alias: `cls`)*. |

## 🤝 Contribution

Les contributions pour enrichir l'expérience de ce casino rétro sont les bienvenues !

1. Créez une branche pour votre fonctionnalité (`git checkout -b feature/nouvelle-table`).
2. Validez vos changements (`git commit -m "feat: ajout d'un nouveau mini-jeu"`).
3. Poussez votre branche sur le dépôt distant (`git push origin feature/nouvelle-table`).
4. Ouvrez une *Merge Request* sur GitLab.

## 📄 Licence

Ce projet est distribué sous licence libre open-source. Consultez le code source pour plus de détails.
