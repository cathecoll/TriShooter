# TriShooter Game Design Document

## Elevator Pitch
Shooter. Trois canons sont montés sur un anneau invisible, encerclant la sortie d’un puit qui est empruntée par des ennemis qu’il faut détruire. 

## Références/Inspirations
Jeu de tirs (arcade) des années 80. BallBlaster  

## Genre
Shooter, Arcade, HyperCasual  

## Design Pillar
Agilité, Satisfaction, Moment de tension suivis par quelques secondes de détente.

## Les 3 C
### Caméra
Caméra 2D, Fixe, Vue d’ensemble, Top down view  

### Characters
**TriShooter** :  
Il s'agit de trois shooters  placés l’extrémité d’un cercle imaginaire prenant la largeur de l’écran. 
Les shooters sont des triangles pointent vers le centre de ce cercle et se déplacent comme s’il y étaient fixés. Les trois shooters tirent en continu.  

**Les Cibles** : 
Elles naissent au centre de l’écran (il s’agit aussi du centre du cercle fictif du TriShooter). 
Elle vont se déplacer vers l'extérieur du cercle imaginaire tout en grossisant.
La génération des ennemis se fera soit aléatoirement, soit selon un schéma donné (à déterminer dans le level design).

### Contrôles
**Contrôleur** :   
Smartphone  

**Type d’input** :   
Slide continu sur l’écran. Le joueur va tracer avec son doigt des mouvements horizontaux qui seront traduits sous forme de rotation du TriShooter.
Emplacement des inputs: toute le zone de jeu. Le système va prendre les segments entre deux positions successives du doigt du 
joueur et le centre de l’écran. L’angle défini par les deux segments va définir la rotation qui sera appliqués au character.

**Automatisations** : 
* Collecte d’objet donnant un bonus.
* Tir continu du TriShooter
* Grossissement et déplacement des cibles
* Destruction d’une cible si elle est touchée
* Destruction du TriShooter si il est touché par une cible

## Core Gameplay
### Micro:
Détruire un ennemi => Orienter les canons => Tirer sur un ennemi => Détruire l’ennemi => Un point comptabilisé.  
Obtenir un bouclier de 5 secondes => Guider un canon sur un baril => collecter le bonus baril => canon protégé pendant 5 secondes.    
Obtenir un bonus => Tirer un triangulaire => Détruire l’ennemi triangulaire => bonus obtenu  
Obtenir un canon de rechange => Tirer sur le dernier ennemi triangulaire de la vague => Détruire ce dernier ennemi => obtenir un canon de rechange obtenu.   

### Moyen
Terminer le niveau : tenir pendant 2 minutes sans se faire toucher par un ennemi.  
Dépasser un taux moyen de réussite : Taux = Nb Ennemis Abbatus/ Nb Ennemis générés.
Obtenir une prime de mission : terminer le niveau => prime obtenue  
Acheter un nouveau canon : sélectionner achat canon => canon acheté  

### Macro
Terminer le jeu => Terminer tous les niveaux => Jeu terminé  

## Conditions de victoire et de défaite
### Conditions de victoire
**Victoire niveau** :   
1. Terminer le niveau avec au moins un Shooter restant,
2. Avoir un résultat de tir suppérieur ou égal à 60%.  

**Victoire Jeu** : 
1. Terminer tous les niveaux

### Conditions de défaite
1. Les trois canons sont détruits et il n’y a plus d’argent pour les remplacer.
2. Le taux de réussite est inférieur à 60%.

## Game Flow

## Level Design
### Briques de Gameplay: 
**TriShooter** : Trois shooters sur un anneau imaginaire
* Vitesse déplacement shooter (contrôlée par le joueur)
* Vitesse de tir  

**Ennemis**:
* Comportement visuel (grossissent ou non)
* Taille (Petit - Moyen - Gros)
* Schéma vague ennemis (Aléatoire - Cercle - Ruban)
* Est destructible ou non
* Vitesse de déplacement
* Couleur/Sprite  

**Bonus**:
* Bonus à abattre/collecter
* Invulnérabilité Shooter pendant un laps de temps
* Reconstruction shooter détruit

### Situations de jeu


## Meta Game

## Monétisation

## Look and Feel

## Maquette Graphique
