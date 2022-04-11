# Hugo_NSI

LE CASSE BRIQUE:  
 
Le but du casse brique est d'envoyer une balle à l'aide d'une planche pour casser des briques et donc gagner des points.  

Décomposition en sous problème:  

Faire apparaitre le jeu à l'aide de Tkinter (à faire plus tard).  
Faire apparaitre la balle (en noir), la planche (en noir), les briques en rouge.  
Créer une fonction permettant au joueur de déplacer la planche.
Créer une fonction permettant de faire apparaitre en même temps le score et le nombre de vie à chaque début de partie (faire apparaitre au joueur le nombre de vie restant à chaque fois qu'il en perd une).  
Créer une fonction permettant d'accumuler des points en temps réelle.  
Créer une fonction permettant à la balle d'être propulser à chaque début de partie et à chaque fois que le joueur perd une balle (garder le score initial après la perte d'une balle).    
Détection de collison entre la balle, la planche, les bords, le sol, le plafond.  
Afficher Game over lorsque le joueur ne possède plus de balle.  

MVP:  
La balle est lancé.  
Elle se dirige vers le haut, puis touche une brique. On gagne alors 1 point.  
Elle rebondi et se dirige alors vers le bas.  
Elle touche alors la planche et elle rebondie à nouveau.  

SDD:  
Affichage d'un terrain à l'aide de coordonnées en pixel. (les bords du terrain, le plafond et le sol).  
Position de la planche avec des coordonnées fixe. Ainsi que sa ligne de déplacement ("D"et"G").   
Position de la balle avec des coordonnnées définie  (tuples) du type (abscisse, ordonnées).  
