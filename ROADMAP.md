# ROADMAP

Feuille de route pour l'amélioration et le développement du jeu. Les sections ci‑dessous sont organisées par axes : visuel, gameplay, audio, progression, interface et technique. Chaque élément est formulé pour être transformé en ticket/issue si nécessaire.

---

## Sommaire
- 🎨 Améliorations visuelles
- 🎮 Gameplay enrichi
- 🔊 Audio
- 📊 Progression et scoring
- 🎯 Interface utilisateur
- 🛠️ Améliorations techniques
- 🗂️ Priorisation / Phases

---

## 🎨 Améliorations visuelles
- [ ] Effets de particules
  - Fumée derrière les voitures
  - Explosions lors des collisions
  - Étincelles pour les power‑ups
- [ ] Arrière‑plan animé
  - Décor défilant : arbres, bâtiments, montagnes
- [ ] Modèles de véhicules variés
  - Différents designs pour le joueur et les obstacles
- [ ] Effets météo
  - Pluie, neige, brouillard (impact sur la visibilité)
- [ ] Animations fluides
  - Transitions (game over, apparition/disparition des power‑ups)
- [ ] Mode nuit
  - Phares éclairant une zone limitée

---

## 🎮 Gameplay enrichi
- [ ] Système de vies
  - Ex. : 3 vies au lieu d'un game over direct
- [ ] Nouveaux power‑ups
  - Ralentissement du temps
  - Aimant à pièces
  - Réparation (restaure la vie ou l'état du véhicule)
- [ ] Obstacles variés
  - Camions lents
  - Motos rapides
  - Flaques d'huile qui font glisser
- [ ] Voies multiples
  - Plus de 3 voies pour plus de variété
- [ ] Virages de la route
  - Piste qui tourne légèrement (ajoute du dynamisme)
- [ ] Mode multijoueur local (technique)
  - Deux joueurs côte à côte (écran partagé ou contrôles partagés)

---

## 🔊 Audio
- [ ] Musique de fond
  - Thème musical dynamique selon la vitesse / difficulté
- [ ] Effets sonores
  - Moteur, klaxon, collision, ramassage de power‑ups, accélération
- [ ] Sons d'ambiance
  - Bruits de circulation, environnement urbain / campagne

---

## 📊 Progression et scoring
- [ ] Sauvegarde du high score
  - localStorage pour le meilleur score
- [ ] Tableau des records
  - Top 5 des meilleurs scores (affichage et reset)
- [ ] Système de pièces
  - Ramasser des pièces pour acheter des améliorations (warp shop)
- [ ] Niveaux de difficulté
  - Facile, Moyen, Difficile (sélection au démarrage)
- [ ] Missions / objectifs
  - Ex. : "Parcourir 1000m sans collision", "Ramasser 5 power‑ups"

---

## 🎯 Interface utilisateur
- [ ] Écran de démarrage
  - Menu avec instructions, sélection de difficulté, et options
- [ ] Pause
  - Touche P pour mettre en pause (ou bouton mobile)
- [ ] Indicateur de vitesse
  - Compteur de vitesse visuel
- [ ] Mini‑map
  - Vue d'ensemble de la piste et des obstacles à venir
- [ ] Barre de vie
  - Visible si le système de vies est activé
- [ ] Thèmes personnalisables
  - Changer la couleur/design de la voiture (cosmétiques)

---

## 🛠️ Améliorations techniques
- [ ] Contrôles tactiles
  - Boutons virtuels et support swipe pour mobile
- [ ] Optimisation mobile
  - Performance, réduction des allocations mémoire, images adaptées
- [ ] Partage de score
  - Boutons pour partager le record sur les réseaux sociaux
- [ ] Architecture et qualité
  - Séparer logique de rendu, tests unitaires sur la logique de jeu
- [ ] Localisation
  - Prévoir traduction (FR / EN) pour le menu et les messages

---

## 🗂️ Priorisation / Phases (suggestion)
- Phase 1 — Fondamentaux
  - High score, écran de démarrage, pause, contrôles tactiles basiques
- Phase 2 — Gameplay & progression
  - Système de vies, power‑ups essentiels, obstacles variés, niveaux de difficulté
- Phase 3 — Visuels & audio
  - Effets de particules, arrière‑plan animé, musique et SFX
- Phase 4 — Améliorations avancées
  - Multijoueur local, mini‑map, virages, météo, boutique/monnaie

---

Si tu veux, je peux :
- transformer chaque bullet en issues GitHub (avec priorités et labels),
- créer une branche et proposer un fichier mis à jour (`ROADMAP.md`) via un commit,
- ou réorganiser la roadmap selon tes priorités exactes.
