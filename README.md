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



