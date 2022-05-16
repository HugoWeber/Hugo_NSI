# Hugo_NSI  

Règle du jeu:

Le Pierre/Feuille/Ciseau ce joue avec deux personnes.  
Dans ce jeu vous pouvez utilisés soit:  
La Pierre  
La Feuille  
Le Ciseau  
En fonction des objets utilisés, l'un des deux joueurs gagne, l'autre perd.  
Il estv posiible que les deux jpueurs utilisent le même objet, c'est une égalité.  

Décomposition en sous problèpe:  

Création de définitions, la première affichera un menu, la seconde donnera la règle du jeun au joeur et la troisième donnera à chaque objet un chifre qui lui sera propre(En gros poser la quetion suivante au joueur: "Choisir un chifre entre 1(Pierre), 2(Feuille) et 3(Ciseau)".  
Créer un programme permettant de donne les 9 solutions possible.  
Créer 3 image :   
1er image, signe de la Pierre  
2e image, signe de la Feuille  
3e image, signe du Ciseau  
Création d'un programmeatribuant chaque chifre à la bonne impage.  
Création d'un programme indiquant le gagnant ou si c'est une égalité.  

MVP:   

Les deux joueur pense à un objet.  
En fonction des résultat, l'un des joeurs gagne, l'autre perd.  
Mais il est possible qu'ils prennet le même objet, alors c'est une égalité.  


Cahier Journal:    

Jour1: - Règle du jeu  
       - Décomposition en sous problème.  
       - MVP  
       
Jour2: Création cahier journal.  

Jour3: Début des recherche poue la création du Pierre/Feuille/Ciseau.  

Jour4: Création des définition (début)  

Jour5: Création des définition (fin)  

Jour 6: Création du programme permettant de donner les 9 solutions. (début)  

Jour 7: Création du programme permettant de donner les 9 solutions. (fin)  

Jour8: Création du dernier programme indiquant le gagnant ou si c'est une égalité.  


Programme:

def menu():

    print("       |    PIERRE    |")
    print("       |    FEUILLE   |")
    print("       |    CISEAUX   |")
    
    print("1 - Regle")
    print("2 - Jouer")
    
    choix = int(input("Indiquer votre choix : " ))
    if choix == 1:
        regle()
    elif choix == 2:
        jeu()
    else:
        return menu()









def regle():

    print("La Pierre bat les Ciseaux")
    print("La Feuille bat la Pierre")
    print("Les Ciseaux battent la Feuille")
    print("Si vous et l'ordinateur avez") 
    print ("le meme objet, il y a egalite")
    

       
