# games
Jeu de Course de Voitures
Vue d'ensemble
Un jeu de course de voitures immersif créé avec HTML5 Canvas, CSS3 et JavaScript vanilla. Le joueur contrôle une voiture qui doit éviter les obstacles tout en ramassant des power-ups sur une piste défilante, avec des effets visuels avancés pour une expérience de jeu captivante.

Fonctionnalités
Modes de jeu
Solo : Jouez seul contre les obstacles
Multijoueur local : Deux joueurs côte à côte sur le même écran
Contrôles
Mode Solo et Joueur 1 (Multijoueur)
Flèche Gauche : Tourner à gauche
Flèche Droite : Tourner à droite
Flèche Haut : Accélérer
Flèche Bas : Freiner
Joueur 2 (Multijoueur)
Z : Accélérer
Q : Tourner à gauche
S : Freiner
D : Tourner à droite
Mobile (Tactile)
Boutons virtuels : Contrôles tactiles qui apparaissent automatiquement sur les écrans tactiles
Éléments de jeu
Voiture du joueur : Contrôlable avec les touches fléchées, choisie aléatoirement parmi 4 modèles à chaque partie
Piste défilante : Piste grise avec bordures blanches et lignes centrales animées
Obstacles : Voitures variées (sports, classic, truck, police) qui apparaissent aléatoirement sur la piste
Power-ups : Deux types de bonus ramassables avec effets visuels
🛡 Bouclier bleu : Invincibilité pendant 5 secondes (effet de bouclier animé)
⚡ Boost jaune : Vitesse x2 pendant 5 secondes
Modèles de voitures
Le jeu propose 4 types de véhicules différents :

Sports : Voiture rouge avec aileron, compacte et rapide
Classic : Voiture bleue classique, équilibrée
Truck : Camion gris, plus large et imposant
Police : Voiture de police noire avec gyrophares rouge et bleu
Effets visuels avancés
Système de particules
Fumée : Derrière toutes les voitures en mouvement
Explosions : Lors des collisions (20 particules avec dégradé de couleur)
Étincelles : Lors du ramassage de power-ups (10 particules en forme d'étoile)
Arrière-plan animé
Décor défilant dynamique avec :

Arbres : Sapins verts sur les côtés de la route
Bâtiments : Immeubles gris avec fenêtres illuminées aléatoires
Panneaux : Panneaux de signalisation jaunes
Effets météorologiques
La météo change automatiquement tous les 10 secondes entre :

Pluie : Gouttes rapides et inclinées (100 particules)
Neige : Flocons lents avec mouvement oscillant (80 particules)
Brouillard : Effet de brume avec dégradé de gris semi-transparent
Animations fluides
Power-ups : Rotation continue + pulsation de taille + dégradé radial brillant
Bouclier : Animation pulsante et ondulante autour de la voiture
Game Over : Apparition en fondu + effet de tremblement
HUD Power-up : Animation pulse quand un power-up est actif
Système de score
Le score augmente en fonction de la distance parcourue
Plus la voiture va vite, plus le score augmente rapidement
Le score final s'affiche à l'écran Game Over avec animations
Difficulté progressive
La vitesse de base augmente automatiquement tous les 10 secondes
La météo change également tous les 10 secondes pour varier le challenge
Plus le jeu progresse, plus il devient difficile
Interface utilisateur
Menu principal : Sélection du mode de jeu et personnalisation
Score : Affiché en haut à gauche de l'écran (les deux joueurs en multijoueur)
Indicateur de power-up : Affiché en haut à droite quand un power-up est actif (avec animation pulse)
Écran Game Over : Affiche le score final et un bouton pour recommencer avec animations, affiche quel joueur a perdu en multijoueur
Personnalisation : Menu pour choisir la couleur de la voiture (6 couleurs disponibles)
Partage social : Boutons pour partager votre score sur Twitter, Facebook et WhatsApp
Responsive
Le jeu s'adapte automatiquement à différentes tailles d'écran
Fonctionne sur desktop et appareils mobiles
Structure du projet
.
├── index.html      # Fichier principal contenant tout le code (HTML, CSS, JS)
└── README.md       # Documentation du projet

Architecture technique
Technologies utilisées
HTML5 Canvas : Rendu 2D du jeu
CSS3 : Stylisation, animations et responsive design
JavaScript Vanilla : Logique du jeu (pas de frameworks)
Composants principaux
Système de rendu : Dessine la piste, l'arrière-plan, la météo, les voitures, les obstacles et les power-ups
Boucle de jeu : Gère les mises à jour et le rendu à 60 FPS via requestAnimationFrame
Détection de collision : Vérifie les collisions entre la voiture et les obstacles/power-ups
Gestion des événements : Capture les touches du clavier pour les contrôles
Système de spawn : Génère aléatoirement les obstacles, power-ups et objets d'arrière-plan
Système de particules : Classe Particle pour gérer fumée, explosions et étincelles
Objets d'arrière-plan : Classe BackgroundObject pour arbres, bâtiments et panneaux
Système météo : Classe WeatherParticle pour pluie, neige et brouillard
Classes JavaScript
Particle : Gère les particules (fumée, explosion, étincelle) avec cycle de vie
BackgroundObject : Gère les éléments de décor défilant (arbres, bâtiments, panneaux)
WeatherParticle : Gère les particules météorologiques (pluie, neige)
Dernières modifications
2025-11-06 : Ajout du multijoueur, contrôles mobiles et personnalisation
Implémentation du mode multijoueur local
Deux joueurs côte à côte sur le même écran
Joueur 1 : touches fléchées, Joueur 2 : ZQSD
Détection de collision séparée pour chaque joueur
Système de power-ups fonctionnel pour les deux joueurs
Affichage des scores pour les deux joueurs
Écran Game Over indiquant quel joueur a perdu
Ajout des contrôles tactiles pour mobile
Boutons virtuels qui apparaissent automatiquement sur écrans tactiles
Interface responsive adaptée aux petits écrans
Système de personnalisation
Menu de sélection de couleur (6 couleurs disponibles)
Rouge, Bleu, Vert, Jaune, Violet, Orange
Fonctionnalité de partage social
Boutons de partage pour Twitter, Facebook et WhatsApp
Partage du score directement depuis l'écran Game Over
Menu principal avec sélection du mode de jeu
2025-11-06 : Ajout des améliorations visuelles majeures
Implémentation du système de particules complet
Fumée derrière les voitures
Explosions lors des collisions (20 particules avec dégradé)
Étincelles lors du ramassage de power-ups (10 particules en étoile)
Ajout de l'arrière-plan animé avec décor défilant
Arbres, bâtiments, panneaux de signalisation
Spawn aléatoire et défilement synchronisé
Implémentation de 4 modèles de voitures variés
Sports (rouge, avec aileron)
Classic (bleue, équilibrée)
Truck (gris, plus large)
Police (noire, avec gyrophares)
Sélection aléatoire pour le joueur à chaque partie
Dimensions correctement mises à jour selon le type
Ajout des effets météorologiques
Pluie (100 gouttes rapides)
Neige (80 flocons oscillants)
Brouillard (dégradé semi-transparent)
Changement automatique tous les 10 secondes
Création d'animations fluides
Power-ups : rotation + pulsation + dégradé radial
Bouclier : animation pulsante et ondulante
Game Over : fade-in + shake
HUD power-up : animation pulse
2025-11-06 : Création initiale du jeu
Implémentation de la voiture contrôlable
Création de la piste défilante avec animations
Ajout des obstacles et système de collision
Intégration des power-ups (bouclier et boost)
Système de score dynamique
Difficulté progressive
Interface utilisateur responsive
Écran Game Over avec bouton restart
Améliorations futures possibles
Ajouter des effets sonores et musique de fond
Créer un système de high score avec localStorage
Implémenter différents types d'obstacles avec comportements variés (motos rapides, camions lents)
Créer un système de vies au lieu d'un game over immédiat
Ajouter des bonus supplémentaires (ralentissement du temps, aimant à pièces)
Implémenter des virages de route
Ajouter un mode nuit avec phares
Ajouter un mode multijoueur en ligne
Performance
Le jeu maintient une bonne performance grâce à :

Suppression automatique des objets hors écran
Gestion efficace des particules avec cycle de vie
Utilisation de requestAnimationFrame pour un rendu fluide
Optimisation du nombre de particules météo
Nettoyage régulier des tableaux d'objets
