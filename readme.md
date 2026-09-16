# VEGAS-OS // Terminal Casino 🎰

**VEGAS-OS** est un simulateur de casino interactif et immersif entièrement développé en un seul fichier (Single-File App) avec **HTML5, Tailwind CSS et JavaScript pur**. Présenté sous la forme d'un terminal de commande rétro/cyberpunk (inspiré des environnements CRT), il intègre un système d'authentification des utilisateurs, plusieurs jeux de casino entièrement jouables, un système de séries de victoires dynamiques 🔥, une gestion VIP évolutive et des thèmes graphiques déblocables.

---

## 🚀 Fonctionnalités principales

- **Terminal Interactif Rétro (CRT) :**
  - Effets visuels d'écran cathodique (lignes de balayage / scanlines, lueurs de phosphore).
  - Navigation par commandes textuelles avec autocomplétion (`Tab`) et historique des commandes (`Flèche Haut/Bas`).
  - Barre de raccourcis rapide personnalisable en bas d'écran.
- **Catalogue de Jeux de Casino :**
  - 🎰 **Slots (Machine à sous) :** Rouleaux virtuels pondérés, gains multipliés (jusqu'au Jackpot x77), remboursements sur cerises.
  - ♠️ **Blackjack :** Table de 21 complète avec cartes dynamiques, options de tirage (*hit*), maintien (*stand*) et doublage (*double*).
  - 🎡 **Roulette Européenne :** Cylindre de 37 cases (0 à 36), paris sur numéros pleins (x36), couleurs, parités, passes/manques ou douzaines.
  - 🚀 **Crash (Fusée) :** Multiplicateur exponentiel en temps réel où le joueur doit s'éjecter avant l'explosion.
  - 🎲 **Dés (2D6) :** Lancer de deux dés avec cotes dynamiques selon les conditions de somme (*sup* ou *inf*).
- **Systèmes Avancés & Économie :**
  - **Système de Séries 🔥 :** Enchaînez les victoires pour obtenir un bonus progressif de $+1\%$ par victoire consécutive.
  - **Statistiques & Probabilités :** Suivi individuel des taux de victoires par jeu et commande dédiée (`proba`) pour consulter les cotes mathématiques exactes et les taux RTP.
  - **Hiérarchie VIP :** Paliers dynamiques (Bronze, Argent, Or, Platinum, Diamant) selon votre capital.
  - **Aide financière du Cartel :** Subvention quotidienne (`bonus`) et système d'emprunt (`emprunt` / `rembourser`).
- **Boutique de Thèmes CRT & Personnalisation :**
  - Changez d'ambiance visuelle à la volée (`Matrix`, `Vert CRT`, `Ambre`, `Cyberpunk`, `Crimson`).
  - Sauvegarde automatique des profils et des préférences via le stockage local du navigateur (`localStorage`).

---

## 🛠️ Installation & Loi du Fichier Unique

Le projet repose sur le principe du **Fichier Unique (Single-File Mandate)** : l'intégralité de l'application (structure, styles CSS, moteur audio Web Audio API et logique JavaScript) est contenue dans le fichier unique `VEGAS-OS.html`.

### Pour lancer l'application localement :
1. Téléchargez ou clonez le dépôt sur votre machine.
2. Ouvrez simplement le fichier **`VEGAS-OS.html`** directement dans n'importe quel navigateur web moderne (Google Chrome, Firefox, Microsoft Edge, Safari). Aucun serveur web ni installation de dépendances n'est requis !

```bash
# Exemple de clonage du dépôt
git clone https://gitlab.univ-nantes.fr/E253676K/test.git
cd test
```

---

## 🎮 Commandes principales du Terminal

Une fois connecté avec votre nom d'utilisateur, tapez directement vos commandes dans le terminal :

| Commande | Description |
| :--- | :--- |
| `help` | Affiche le catalogue complet de toutes les commandes disponibles. |
| `proba [jeu]` | Affiche les analyses mathématiques, cotes et taux de retour (RTP). |
| `slots <mise\|all>` | Lance une partie sur la machine à sous (alias: `slot`). |
| `blackjack <mise\|all>` | Ouvre la table de Blackjack interactive (alias: `bj`). |
| `roulette <mise\|all> <pari>` | Lance une partie de roulette européenne (ex: `roulette 50 rouge`). |
| `crash <mise\|all>` | Lance le mini-jeu de la fusée (utilisez `stop` pour encaisser). |
| `dés <mise\|all> <sup\|inf> <n>`| Lance un pari sur la somme de 2 dés (ex: `dés 100 sup 7`). |
| `profil` | Affiche votre dossier joueur, solde, dettes et records de séries. |
| `vip` | Affiche les avantages et conditions de la hiérarchie VIP. |
| `stats` | Affiche le taux de réussite individuel pour chaque jeu. |
| `bonus` | Réclame l'aide financière du cartel (+250 $ toutes les 3 minutes). |
| `emprunt <montant>` | Emprunte des jetons au cartel (jusqu'à 5 000 $, taux 30%). |
| `rembourser [montant\|all]`| Rembourse tout ou partie de votre dette active. |
| `theme [nom]` | Change le thème visuel (`matrix`, `amber`, `cyberpunk`, `crimson`, `default`). |
| `settings` | Ouvre la fenêtre graphique de configuration, audio et thèmes. |
| `logout` | Sauvegarde la session en cours et retourne à l'écran de login. |
| `clear` | Nettoie l'affichage du terminal. |

---

## 🤝 Contribution

Les contributions pour améliorer l'expérience de ce terminal de casino sont les bienvenues ! 
1. Créez une branche pour votre fonctionnalité (`git checkout -b feature/nouvelle-fonction`).
2. Validez vos changements (`git commit -m "feat: ajout d'un nouveau mini-jeu"`).
3. Poussez votre branche sur le dépôt (`git push origin feature/nouvelle-fonction`).
4. Ouvrez une *Merge Request* sur GitLab.

## 📄 Licence

Ce projet est distribué sous licence open-source. Consultez le code source pour plus de détails.
