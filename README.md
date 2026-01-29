Jour 2 : SQL - DDL & DML

Objectif du jour : Savoir créer des tables simples et manipuler les données (insérer, mettre à jour, supprimer).

Questions Théoriques : 

1-Quelle est la différence entre DDL (CREATE, ALTER) et DML (INSERT, UPDATE, DELETE) ? : la difference entre DDL et DML et DDL crea la structure du basse de donner et DML prendre la partie content du cette basse de donner
2. À quoi sert une clé primaire ? : Une clé primaire sert à identifier de manière unique chaque row dans un tableau 
3. Comment filtre-t-on des données avec la clause WHERE ? : pour filtrer les donner avec where nous fair a conditions avec where entre une column et un value  

● Challenges Pratiques :
CREATE TABLE Produits (
  id INT AUTO_INCREMENT PRIMARY KEY ,
  nom VARCHAR(255) NOT NULL ,
  prix DECIMAL(10 , 4) NOT NULL, 
  stock INT NOT NULL
);

2- 
INSERT INTO Produits (nom , prix , stock) VALUE ('bimo' , 1.99 , 200) , ('l'eau' , 0.99 , 300) , ('danon' , 3.99 , 200) ;

3-
UPDATE Produits SET prix = prix * 1.1 ; 
DELETE FROM Produits WHERE stock = 0 ;


Jour 3 : SQL - Agrégats Simples 

Objectif du jour : Maîtriser l'utilisation des fonctions d'agrégation pour résumer des données. 

Questions Théoriques :

1. À quoi servent les fonctions COUNT, SUM, et AVG ? :
   
   cette function est fonctions d’agrégation pour COUNT elle sert a comter le nombre de line ou d'enregistrement dans une column ,  pour SUM eller utuluser pour calculer la somme des valeur numeruque  dans une colunn , pour AVG il est utuluser pour callculer la moyenne numeruque d'un column .
   
2. Peut-on utiliser COUNT(*) et COUNT(colonne) de manière interchangeable ? Pourquoi ? :

  Non, on (pas interchangeables). COUNT(column) compte uniquement les lignes qui contiennent une valeur ; si la valeur est NULL, elle est ignorée. Par contre, COUNT(*) compte le nombre total de lignes (rows) sans vérifier le contenu des colonnes.

3. Comment MAX et MIN peuvent-ils être utilisés sur des dates ou des chaînes de caractères ? :

  Oui, les fonctions MAX et MIN ne sont pas réservées qu'aux chiffres. Sur des dates, MAX retourne la date la plus récente et MIN la plus ancienne. Sur des chaînes de caractères, elles se basent sur l'ordre alphabétique . 

Challenges Pratiques :

1- SELECT COUNT(*) FORM commandes ; 
2- SELECT AVG(prix) FROM produits ; 
3- SELECT MAX(total) FROM commendes ; 
   
 












