Jour 4 : PHP POO - Classes & Objets

Objectif du jour : Comprendre la syntaxe de base pour créer une classe, définir ses membres et l'instancier.

1. Quelle est la différence entre une classe et un objet ? : la differente entre les deux est le class estun blue prent pour l'object et l'object est l'instance d'un class .
2. À quoi sert le mot-clé $this ? : le mot-cle $this represent l'object .
3. Quel est le rôle du constructeur (__construct) ? : le role de construct et trvails en le temps qi nous somme creare une object a partir cette construct class .

   ● Challenges Pratiques :

1- 
Class Voiture {
  public $vitesse ; 
  public $modele ; 
  public $marque ; 


  public function accelerer() {
    $this -> vitesse += $this -> vitesse 
  }
  
}

2-
Class Voiture {
  private $vitesse ; 
  private $modele ; 
  private $marque ; 

  public function __construct($modele , $marque) {
    $this -> modele = $modele ; 
    $this -> marque = $marque ; 
  }

  public function accelerer() {
    $this -> vitesse += $this -> vitesse
  }
  
}

3-

$voiture1 = new Voiture('2020' , 'clio' ) ;
$voiture2 = new Voiture('2020' , 'dacia') ; 

$voiture1 -> accelerer ; 
$voiture2 -> accelerer ; 





