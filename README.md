# Projet-NSI-Bulls & Cows

## Description du projet
  
  Dans ce projet, je vais créer un jeu en ligne s'intitulant Bulls & Cows. Bulls & COWS est un jeu d'esprit ou de papier et de crayon pour deux jouers ou plus, antérieur
aux jeux Mastermind et Wordle. 

## Quelques problèmes pouvant apparaître sur la route

  - Cacher la liste de nombre qu'il faut trouver
  - faire en sorte de changer le résultat à chaque nouvelle partie

## MVP
 
  - Premièrement, je vais créer un programme pour avoir des numéros random
  - Deuxièmement, je vais créer le compteur d'essais
  - Troisièmement, je créerai bulls et cows

## Liste des Fonctions

...

def CreerNombre(): # Crée un nombre random.
    for i in range(4):
        x = random.randrange(9)
        nombre.append(x)
    if len(nombre) > len(set(nombre)): # S'il n'y a pas de nombres répétés, cela fera un loop jusqu'à se qu'il y ai au moins un nombre répété.
        nombre.clear()
        CreerNombre()
        
def JouerPartie():
    global essais
    essais += 1 # Rajout d'un essai à chaque fois que le résultat n'est pas trouvé.
    cows =0 # Fait un reset à chaque nouvelle partie.
    bulls = 0
    print(nombre)
    choix = input("Entrez une list de 4 nombres") # Message pour ajouter une liste de nombres.
    deviner = []

...

## Jeu tests

  Nous allons tester si les numéros sont random et si le programme marche
https://github.com/Yasmine-Zaky/projet-nsi-filtre
