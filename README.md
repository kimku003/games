# games — Jeu de course de voitures

## Vue d'ensemble
Jeu de course immersif construit avec HTML5 Canvas, CSS3 et JavaScript (vanilla). Le joueur contrôle une voiture, évite des obstacles et ramasse des power-ups sur une piste défilante.

---

## Table des matières
- [Fonctionnalités](#fonctionnalités)
  - [Modes de jeu](#modes-de-jeu)
  - [Contrôles](#contrôles)
  - [Éléments de jeu](#éléments-de-jeu)
  - [Power-ups](#power-ups)
  - [Modèles de voitures](#modèles-de-voitures)
  - [Effets visuels avancés](#effets-visuels-avancés)
  - [Météo](#météo)
  - [Système de score et difficulté](#système-de-score-et-difficulté)
  - [Interface utilisateur](#interface-utilisateur)
  - [Responsive & mobile](#responsive--mobile)
- [Structure du projet](#structure-du-projet)
- [Architecture technique](#architecture-technique)
- [Classes principales](#classes-principales)
- [Dernières modifications](#dernières-modifications)
- [Améliorations futures possibles](#améliorations-futures-possibles)
- [Performance](#performance)

---

## Fonctionnalités

### Modes de jeu
- Solo : jouer seul contre des obstacles.
- Multijoueur local : deux joueurs côte à côte sur le même écran.

### Contrôles
- Mode Solo et Joueur 1 (Multijoueur)
  - Flèche Gauche : tourner à gauche
  - Flèche Droite : tourner à droite
  - Flèche Haut : accélérer
  - Flèche Bas : freiner
- Joueur 2 (Multijoueur)
  - Z : accélérer
  - Q : tourner à gauche
  - S : freiner
  - D : tourner à droite
- Mobile (tactile)
  - Boutons virtuels : contrôles tactiles qui apparaissent automatiquement sur écrans tactiles

### Éléments de jeu
- Voiture du joueur : choisie aléatoirement parmi 4 modèles à chaque partie.
- Piste défilante : piste grise avec bordures blanches et lignes centrales animées.
- Obstacles : voitures variées (sports, classic, truck, police) générées aléatoirement.
- Power-ups : ramassables, avec effets visuels.

### Power-ups
- 🛡 Bouclier bleu : invincibilité pendant 5 secondes (effet de bouclier animé).
- ⚡ Boost jaune : vitesse x2 pendant 5 secondes.

### Modèles de voitures
4 types de véhicules avec caractéristiques visuelles et physiques :
- Sports : rouge, aileron, compacte et rapide.
- Classic : bleue, équilibrée.
- Truck : gris, large et imposant.
- Police : noire, gyrophares rouge/bleu.

---

## Effets visuels avancés

### Système de particules
- Fumée : derrière toutes les voitures en mouvement.
- Explosions : lors des collisions (env. 20 particules avec dégradé).
- Étincelles : lors du ramassage de power-ups (≈10 particules en forme d'étoile).

### Arrière-plan animé
Décor défilant synchronisé avec la piste :
- Arbres (sapins) sur les côtés.
- Bâtiments avec fenêtres illuminées aléatoirement.
- Panneaux de signalisation.

---

## Météo
La météo change automatiquement toutes les 10 secondes (variations de challenge) :
- Pluie : gouttes rapides et inclinées (≈100 particules).
- Neige : flocons lents avec oscillation (≈80 particules).
- Brouillard : dégradé semi-transparent simulant la brume.

---

## Animations & UI visuelles
- Power-ups : rotation continue + pulsation + dégradé radial.
- Bouclier : animation pulsante et ondulante autour de la voiture.
- Game Over : apparition en fondu + effet de tremblement.
- HUD power-up : animation "pulse" quand actif.
- Animation fluide via requestAnimationFrame.

---

## Système de score et difficulté
- Score basé sur la distance parcourue.
- Le score augmente plus rapidement si la voiture va vite.
- Difficulté progressive : vitesse de base augmentée automatiquement tous les 10 secondes ; météo change pour varier la difficulté.
- Score final affiché sur l'écran Game Over avec animations.

---

## Interface utilisateur
- Menu principal : sélection du mode et personnalisation.
- Score : affiché en haut à gauche (deux scores en multijoueur).
- Indicateur de power-up : en haut à droite quand actif (avec animation).
- Écran Game Over : affiche le score final, qui a perdu en multijoueur, et bouton pour recommencer.
- Personnalisation : choix de couleur de voiture (6 couleurs).
- Partage social : boutons pour partager le score sur Twitter, Facebook, WhatsApp.

### Personnalisation des couleurs
- 6 couleurs disponibles : Rouge, Bleu, Vert, Jaune, Violet, Orange

---

## Responsive & Mobile
- Adaptation automatique aux différentes tailles d'écran.
- Fonctionne sur desktop et appareils mobiles grâce à contrôles tactiles et responsive CSS.

---

## Structure du projet
Arborescence principale :
.
├── index.html      # Fichier principal contenant HTML, CSS et JS intégrés  
└── README.md       # Documentation du projet

---

## Architecture technique

### Technologies
- HTML5 Canvas : rendu 2D.
- CSS3 : styles, animations, responsive.
- JavaScript (vanilla) : logique du jeu (sans frameworks).

### Composants principaux
- Système de rendu : dessine piste, arrière-plan, météo, voitures, obstacles, power-ups.
- Boucle de jeu : update & render à 60 FPS via requestAnimationFrame.
- Détection de collision : collisions voiture / obstacle / power-up.
- Gestion des événements : capture clavier et entrées tactiles.
- Système de spawn : génération aléatoire d'obstacles, power-ups et décor.
- Système de particules : gestion du cycle de vie des particules.
- Objets d'arrière-plan : arbres, bâtiments, panneaux.
- Système météo : pluie, neige, brouillard.

---

## Classes JavaScript (principales)
- Particle : gère particules (fumée, explosion, étincelle) et leur cycle de vie.
- BackgroundObject : gère objets de décor défilant (arbres, bâtiments, panneaux).
- WeatherParticle : gère particules météorologiques (pluie, neige).

---

## Dernières modifications
- 2025-11-05 : Ajout du multijoueur, contrôles mobiles et personnalisation
  - Mode multijoueur local (deux joueurs).
  - Détection de collision séparée, power-ups fonctionnels pour les deux joueurs.
  - Affichage des scores pour les deux joueurs et écran Game Over indiquant quel joueur a perdu.
  - Contrôles tactiles et interface responsive.
  - Menu de sélection de couleur (6 couleurs).
  - Boutons de partage social.
  - Menu principal avec sélection du mode.

- 2025-11-06 : Améliorations visuelles majeures
  - Système de particules complet (fumée, explosions, étincelles).
  - Arrière-plan animé : arbres, bâtiments, panneaux.
  - 4 modèles de voitures avec dimensions adaptées.
  - Système météo (pluie, neige, brouillard) changeant automatiquement.
  - Animations fluides pour power-ups, bouclier et Game Over.

- 2025-11-06 : Création initiale
  - Voiture contrôlable, piste défilante, obstacles, collisions, power-ups, score et difficulté progressive.

---

## Améliorations futures possibles
- Ajouter sons et musique de fond.
- Système de high score (localStorage).
- Objets obstacles avec comportements variés (motos, camions).
- Système de vies au lieu d'un game over immédiat.
- Nouveaux power-ups (ralentissement du temps, aimant à pièces).
- Virages de route et mode nuit avec phares.
- Mode multijoueur en ligne.

---

## Performance
- Suppression automatique des objets hors écran.
- Gestion efficace des particules (cycle de vie).
- Utilisation de requestAnimationFrame pour rendu fluide.
- Optimisation du nombre de particules météo.
- Nettoyage régulier des tableaux d'objets.

---

Merci d'avoir consulté la documentation.
