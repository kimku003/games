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
- [x] Effets de particules
  - Fumée derrière les voitures
  - Explosions lors des collisions
  - Étincelles pour les power‑ups
- [x] Arrière‑plan animé
  - Décor défilant : arbres, bâtiments, montagnes
- [x] Modèles de véhicules variés
  - Différents designs pour le joueur et les obstacles
- [x] Effets météo
  - Pluie, neige, brouillard (impact sur la visibilité)
- [x] Animations fluides
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
- [x] Obstacles variés
  - Camions lents
  - Motos rapides
  - Flaques d'huile qui font glisser
- [ ] Voies multiples
  - Plus de 3 voies pour plus de variété
- [ ] Virages de la route
  - Piste qui tourne légèrement (ajoute du dynamisme)
- [x] Mode multijoueur local (technique)
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
- [x] Sauvegarde du high score
  - localStorage pour le meilleur score
- [ ] Tableau des records
  - Top 5 des meilleurs scores (affichage et reset)
- [ ] Système de pièces
  - Ramasser des pièces pour acheter des améliorations (warp shop)
- [x] Niveaux de difficulté
  - Facile, Moyen, Difficile (réglable dans le menu Pause)
- [ ] Missions / objectifs
  - Ex. : "Parcourir 1000m sans collision", "Ramasser 5 power‑ups"

---

## 🎯 Interface utilisateur
- [x] Écran de démarrage
  - Menu avec instructions et options (la difficulté est déplacée dans Pause)
- [x] Lien public du jeu
  - https://kimku003.github.io/games/race.html
- [x] Pause
  - Bouton ⏸️ flottant et touche P
  - Panneau de réglages dans Pause: Mode de contrôle (Touches/Swipe), Difficulté, Muet (préférence mémorisée)
- [x] Indicateur de vitesse
  - Compteur de vitesse visuel
- [ ] Mini‑map
  - Vue d'ensemble de la piste et des obstacles à venir
- [ ] Barre de vie
  - Visible si le système de vies est activé
- [x] Thèmes personnalisables
  - Changer la couleur/design de la voiture (cosmétiques)
- [x] Contrôles tactiles minimalistes
  - Boutons directionnels sans icônes, masqués en mode Swipe
  - Astuce "Swipe" affichée une seule fois

---

## 🛠️ Améliorations techniques
- [x] Contrôles tactiles
  - Boutons virtuels et support swipe pour mobile, bascule Touches/Swipe depuis Pause
- [ ] Optimisation mobile
  - Performance, réduction des allocations mémoire, images adaptées
- [x] Partage de score
  - Boutons pour partager le record sur les réseaux sociaux (URL publique intégrée)
- [ ] Architecture et qualité
  - Séparer logique de rendu, tests unitaires sur la logique de jeu
- [ ] Localisation
  - Prévoir traduction (FR / EN) pour le menu et les messages
