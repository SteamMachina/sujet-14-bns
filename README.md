EXERCICE 1 (4 points) 

 
 
 
Écrire une fonction recherche qui prend en paramètres elt un nombre et tab un 
tableau de nombres, et qui renvoie le tableau des indices de elt dans tab si elt est 
dans tab et le tableau vide [] sinon. 

Exemples : 

>>> recherche(3, [3, 2, 1, 3, 2, 1]) 
[0, 3] 
>>> recherche(4, [1, 2, 3]) 
[] 

EXERCICE 2 (4 points) 

Un  professeur  de  NSI  décide  de  gérer  les  résultats  de  sa  classe  sous  la  forme  d’un 
dictionnaire :  

les clefs sont les noms des élèves ; 
les valeurs sont des dictionnaires dont les clefs sont les types d’épreuves et les 
valeurs sont les notes obtenues associées à leurs coefficients. 

Avec : 

resultats = {'Dupont':{'DS1' : [15.5, 4], 
                       'DM1' : [14.5, 1], 
                       'DS2' : [13, 4], 
                       'PROJET1' : [16, 3], 
                       'DS3' : [14, 4]}, 
             'Durand':{'DS1' : [6 , 4], 
                       'DM1' : [14.5, 1], 
                       'DS2' : [8, 4], 
                       'PROJET1' : [9, 3], 
                       'IE1' : [7, 2], 
                       'DS3' : [8, 4], 
                       'DS4' :[15, 4]}} 
 
L’élève dont le nom est Durand a ainsi obtenu au DS2 la note de 8 avec un coefficient 4. 
 
Le professeur crée une fonction moyenne qui prend en paramètre le nom d’un de ces 
élèves et lui renvoie sa moyenne arrondie au dixième.  

Compléter le code du professeur ci-dessous : 

 

def moyenne(nom): 
    if nom in ...: 
        notes = resultats[nom] 
        total_points = ... 
        total_coefficients = ... 
        for ...  in notes.values(): 
            note , coefficient = valeurs 
            total_points = total_points + ... * coefficient 
            total_coefficients = ... + coefficient 
        return round( ... / total_coefficients , 1 ) 
    else: 
        return -1 
 
