# VEGAS-OS // Terminal Casino 🎰

**VEGAS-OS** est un simulateur de casino interactif et immersif développé sous la forme d'un terminal de commande rétro/cyberpunk (inspiré des moniteurs cathodiques CRT). Il intègre un système complet d'authentification par compte joueur, un catalogue varié de jeux de casino, une mécanique de séries de victoires dynamiques (🔥), une économie avec gestion VIP évolutive, un moteur sonore procédural (musique d'ambiance et bruitages synthétiques) et une boutique de palettes graphiques déblocables.

---

## 🌐 Jouer en ligne

Le jeu est directement accessible dans votre navigateur web sans aucun téléchargement ni installation :

👉 **[https://vegas-os.netlify.app/](https://vegas-os.netlify.app/)**

Compatible avec tous les navigateurs modernes (*Google Chrome, Mozilla Firefox, Microsoft Edge, Safari, Brave*), sur ordinateur comme sur mobile.

---

## 🌟 Fonctionnalités principales

- **Terminal Interactif Rétro (CRT) :**
  - Effets visuels d'écran cathodique : lignes de balayage (*scanlines*), lueurs de phosphore et courbure optique.
  - Navigation par ligne de commande avec auto-complétion contextuelle (`Tab`) et historique dynamique (`Flèche Haut / Bas`).
  - Barre de raccourcis rapides cliquables et personnalisables au bas de l'écran.
  - HUD système complet en en-tête : suivi en temps réel du solde, de la dette, du rang VIP et du compteur de séries de victoires.

- **Catalogue de Jeux de Casino :**
  - 🎰 **Slots (Machine à sous) :** Rouleaux virtuels pondérés, remboursements sur cerises et gains multipliés jusqu'au Jackpot Suprême `[ 7 ] [ 7 ] [ 7 ]` (x77).
  - ♠️ **Blackjack (Table 21) :** Distribution dynamique, options de tirage (*hit*), maintien (*stand*), doublage (*double*) et **Split de paire** (séparation stricte de deux cartes de même rang pour jouer deux mains indépendantes).
  - 🃏 **Ultimate Texas Hold'em (Poker) :** Affrontez la main du croupier avec mise initiale Ante + Blind, décisions d'enchère Play modulables (x4 préflop, x2 au flop, x1 à la river) et règle de qualification du croupier.
  - 🎡 **Roulette Européenne :** Cylindre standard de 37 numéros (0 à 36), paris sur numéros pleins (x36), chances simples (Rouge/Noir, Pair/Impair, Manque/Passe) et douzaines (d1, d2, d3).
  - 🚀 **Crash (Fusée) :** Multiplicateur exponentiel en temps réel où vous devez vous éjecter (`stop` / `cash`) avant l'explosion inopinée du vaisseau.
  - 🎲 **Dés (2D6) :** Lancer de deux dés à 6 faces avec calcul dynamique des cotes mathématiques selon les conditions choisies (`sup` ou `inf`).

- **Systèmes Avancés & Économie :**
  - **Séries de Victoires (🔥) :** Enchaînez les victoires consécutives pour bénéficier d'un bonus financier progressif (+1 % de gain par niveau de série). Les égalités (*push*) préservent la série en cours.
  - **Statistiques & Probabilités :** Suivi granulaire par jeu (taux de victoire, mises engagées, gains nets, records) et commande d'analyse mathématique (`proba`) détaillant l'espérance et le RTP de chaque table.
  - **Hiérarchie VIP Évolutive :** Paliers automatiques de prestige basés sur votre capital : **Bronze**, **Argent**, **Or**, **Platinum** et **Diamant**.
  - **Aide Financière du Cartel :** Subvention périodique (`bonus`) ajustée à votre rang VIP (recharge de 3 minutes) et système d'emprunt d'urgence (`emprunt` / `rembourser`) plafonné à 5 000 $.

- **Ambiance Sonore & Personnalisation Graphique :**
  - **Moteur Sonore Procédural (Web Audio API) :** Bruitages rétro (frappe de touche, bips, lancers de rouleaux, gains, explosions) et musique d'ambiance cyber-casino générée en direct sans aucun fichier audio externe.
  - **Boutique de Thèmes CRT :** Débloquez et appliquez différentes palettes d'affichage rétro (`Matrix`, `Vert CRT`, `Ambre`, `Cyberpunk`, `Crimson Cyber`, `Or Impérial`).
  - **Persistance Locale :** Sauvegarde automatique des comptes joueurs, mots de passe, soldes, statistiques et raccourcis via le stockage local du navigateur (`localStorage`).

---

## ⌨️ Commandes principales du Terminal

Une fois connecté avec votre nom d'utilisateur, tapez directement vos commandes dans le terminal :

| Commande | Syntaxe / Exemple | Description |
| :--- | :--- | :--- |
| `help` | `help [commande/jeu]` | Affiche le catalogue général ou les règles détaillées d'un jeu précis. |
| `proba` | `proba [jeu]` | Affiche les analyses statistiques, cotes mathématiques et taux de retour (RTP). |
| `slots` | `slots <mise\|all>` | Lance la machine à sous virtuelle *(alias : `slot`)*. |
| `blackjack` | `bj <mise\|all>` | Démarre une table de Blackjack interactive 21 *(alias : `bj`)*. |
| `poker` | `poker <mise\|all>` | Démarre une table d'Ultimate Texas Hold'em *(alias : `ultimate`, `uth`)*. |
| `roulette` | `roulette <mise\|all> <pari>` | Lance une partie de roulette européenne (ex: `roulette 50 rouge`, `roul 100 17`). |
| `crash` | `crash <mise\|all>` | Lance le mini-jeu de la fusée (tapez `stop` ou `cash` pour encaisser). |
| `dés` | `dés <mise\|all> <sup\|inf> <n>` | Parie sur la somme de 2D6 de 3 à 11 (ex: `dés 50 sup 7`). |
| `profil` | `profil` *(ou `compte`)* | Affiche la fiche joueur, solde, valeur nette, records et série 🔥. |
| `stats` | `stats [jeu]` | Affiche le bilan complet et les taux de réussite globaux ou par jeu. |
| `vip` | `vip` *(ou `grades`)* | Détaille les paliers de prestige, subventions et conditions d'accès. |
| `bonus` | `bonus` | Réclame l'allocation financière du Cartel selon votre palier VIP. |
| `emprunt` | `emprunt <montant>` | Emprunte des jetons au Cartel (plafond 5 000 $, intérêt 30 %). |
| `rembourser`| `rembourser [montant\|all]` | Rembourse tout ou partie de votre dette active. |
| `theme` | `theme [nom]` / `theme buy [nom]` | Change de palette d'affichage ou achète un nouveau thème CRT. |
| `settings` | `settings` *(ou `config`)* | Ouvre la fenêtre des réglages audio, musique et raccourcis. |
| `logout` | `logout` *(ou `deconnexion`)* | Sauvegarde la session active et retourne à l'écran de connexion. |
| `clear` | `clear` *(ou `cls`)* | Nettoie l'affichage du terminal. |

---

## 🤝 Contribution

Les contributions pour enrichir l'expérience de ce casino rétro sont les bienvenues :

1. Créez une branche dédiée à votre fonctionnalité (`git checkout -b feature/nouveau-jeu`).
2. Validez vos changements avec un message explicite (`git commit -m "feat: ajout d'un nouveau jeu"`).
3. Poussez votre branche sur le dépôt distant (`git push origin feature/nouveau-jeu`).
4. Ouvrez une **Merge Request** sur GitLab.

---

## 📄 Licence

Ce projet est distribué sous licence open-source libre. Consultez le code source pour plus de détails.