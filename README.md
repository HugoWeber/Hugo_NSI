# Hugo_NSI

LE CASSE BRIQUE/PONG:  

Ce jeu est la fusion du casse brique et du pig-pong.  
Le but du jeu est de renvoyer une balle à l'aide d'une planche.  
Il faut toucher le plafond pour accumuler des points.  
A chaque fois que la balle touche le plafond, la planche ou les bords. La balle rebondie.  
A noter, à chaque fois que la balle touche le plafond, elle se déplacera plus rapidement.  
A chaque début de partie le joueur possède 3 balles.  
Le joueur à perdu lorsqu'il n'aura plus de balle à sa disposition.  
Pour perdre une balle, il faut que cette dernière touche le sol.  

Décomposition en sous problème:  

Faire apparaitre le jeu à l'aide de Tkinter (à faire plus tard).  
Faire apparaitre la balle (en noir), la planche (en noir), le plafond (en bleu), le sol (en rouge), et les rebords.  
Créer une fonction permettant au joueur de déplacer la planche avec la lettre "Q" pour aller à gauche et la lettre "D" pour aller à droite.  
Créer une fonction permettant de faire apparaitre en même temps le score et le nombre de vie à chaque début de partie (faire apparaitre au joueur le nombre de vie restant à chaque fois qu'il en perd une).  
Créer une fonction permettant d'accumuler des points en temps réelle.  
Créer une fonction permettant à la balle d'être propulser à chaque début de partie et à chaque fois que le joueur perd une balle (garder le score initial après la perte d'une balle).  
Créer une fonction permettant à la balle de gagner en vitesse à chaque fois qu'elle touche le plafond.  
Détection de collison entr ela balle et la planche, les bords, le sol, le plafond.  
Afficher Game over lorsque le joueur ne possède plus de balle.  

MVP:  
La balle est lancé.  
Elle se dirige vers le haut, puis touche le plafond. On gagne alors 1 point.  
Elle rebondi et se dirige alors vers le bas.  
Elle touche alors la planche et elle rebondie.  

:  ()
Affichage d'un terrain à l'aide de coordonnées en pixel. (les bords du terrain, le plafond et le sol).  
Position de la planche avec des coordonnées fixe. Ainsi que sa ligne de déplacement ("D"et"G").  
planche et balle définient par des corrdonées (tuples) du type (abscisse, ordonnées) pour la MVP. A complexifié si besoin après.  
