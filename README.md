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

from random import randint
choix = ["Pierre", "Feuille", "Ciseaux"]
ordi = choix[randint(0,2)]



def regle():
    
    print("La Pierre bat les Ciseaux. La Feuille bat la Pierre. Les Ciseaux battent la Feuille. Si vous et l'ordinateur avez le meme objet, il y a egalite")
    
    go_menu = float(input("Tapez 9 quand vous aurez fini de lire : "))
    if go_menu == 9:
        return menu()
    else:
        return menu
    
    

def jeu():
    score_ordi = 0
    score_joueur = 0
    
    point = int(input("Choississez le  nombre de points a atteindre pour gagner : "))
    if point == 0:
        return jeu()
    
    while score_ordi < point and score_joueur < point:
        print("Le score est de", score_joueur, "a", score_ordi,)
        
        choix_joueur = int(input("Que voulez vous choisir 1 = Pierre  /  2 = Feuille   /  3 = Ciseaux : "))
        ordi = choix[randint(0,2)]
        
        if choix_joueur == 1:
            print("Vous avez choisi Pierre")
            print("L'ordinateur a choisi", ordi)
        elif choix_joueur == 2:
            print("Vous avez choisi Feuille")
            print("L'ordinateur a choisi", ordi)
        elif choix_joueur == 3:
            print("Vous avez choisi Ciseaux")
            print("L'ordinateur a choisi", ordi)
        
        if choix_joueur == 1 and ordi == "Ciseaux" or choix_joueur == 2 and ordi == "Pierre" or choix_joueur == 3 and ordi == "Feuille":
            score_joueur = score_joueur + 1
            print("Vous marquez 1 point")
        elif choix_joueur == 1 and ordi == "Feuille" or choix_joueur == 2 and ordi == "Ciseaux" or choix_joueur == 3 and ordi == "Pierre":
            score_ordi = score_ordi + 1
            print("L'ordinateur marque 1 point")
        elif choix_joueur == 1 and ordi == "Pierre" or choix_joueur == 2 and ordi == "Feuille" or choix_joueur == 3 and ordi == "Ciseaux":
            print("Egalite")
        else:
            print("1, 2 ou 3\nC'est pas complique") 
    
       
    
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

menu()





  
    


    









def regle():

    print("La Pierre bat les Ciseaux")
    print("La Feuille bat la Pierre")
    print("Les Ciseaux battent la Feuille")
    print("Si vous et l'ordinateur avez") 
    print ("le meme objet, il y a egalite")
    

       
