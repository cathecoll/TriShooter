# Formalisation du prototype TriShooter 

### Caméra
Caméra 2D, Fixe, Vue d’ensemble, Top down view  

### Characters
**TriShooter** : Trois triangles placés l’extrémité d’un cercle prenant la largeur de l’écran. Les triangles sont orientés vers l’intérieur et pointent vers le centre. Les trois shooters se déplacent comme s’il étaient placés sur un cercle. La rotation de ce cercle fictif va entraîner les trois shooters. Les trois shooters tirent en continu.  

**Les Cibles** : Elles naissent au centre de l’écran (il s’agit aussi du centre du cercle fictif du TriShooter). Elle vont se déplacer vers l'extérieur cercle fictif du TriShooter, tout en grossissant. Le génération des cibles se fera de différentes manières (aléatoire, en cercle, en ruban, ...).  
La collision entre une cible et un shooter provoquera la destruction de ce shooter.

### Contrôles
**Contrôleur** : Smartphone  

**Type d’input** : Slide continu sur l’écran. Le joueur va déplacer son doigt horizontalement sur l'écran. Ce mouvement sera converti en mouvement de rotation du cercle fictif dur lequel les 3 shooters sont placés.  
**Emplacement des inputs** : toute le zone de jeu. Le système va prendre les segments entre deux positions successives du doigt du joueur et le centre de l’écran. L’angle défini par les deux segments va définir la rotation qui sera appliqués au TriShooter.  

**Automatisations** : 
1. Collecte d’objets donnant un bonus.  
2. Tir continu du TriShooter
3. Grossissement et déplacement des cibles
4. Destruction d’une cible si elle est touchée
5. Destruction du TriShooter si il est touché par une cible

