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


Jour 5 : PHP POO - Encapsulation

Objectif du jour : Maîtriser les niveaux de visibilité (public, private, protected) et l'utilisation des getters/setters.

1. Qu’est-ce que l’encapsulation ? Quel est son but ? : L'encapsulation est un concept fondamental de la POO. Son but est de regrouper les données et les méthodes dans une classe, et de protéger l'intégrité des données en restreignant l'accès direct depuis l'extérieur.

2. Quelle est la différence entre public, private et protected ? : La différence concerne la visibilité des attributs et méthodes :

Public : Accessible de partout (tout le monde).

Private : Accessible uniquement à l'intérieur de la classe elle-même.

Protected : Accessible dans la classe et par ses sous-classes (héritage)

3. À quoi servent les getters et setters ? Est-ce toujours nécessaire d'en avoir pour chaque attribut ? : Les getters et setters servent à lire (get) et modifier (set) les attributs privés tout en contrôlant l'accès aux données. Non, ce n'est pas toujours nécessaire. On les définit seulement si on a besoin d'exposer ou de modifier un attribut depuis l'extérieur.


● Challenges Pratiques :

1-
Class Voiture {
  pricate $vitesse ; 
  private $modele ; 
  private $marque ; 

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

  public function getmodel() {
      return $this -> model ;
  }
  public function getmarque () {
      return $this -> marque ;
  }
  public function setmodel($model) {
     $this -> model = $model ; 
     
  }

  public function setmarque ($marque) {
     $this -> marque = $marque ; 
  }

}

2-

Class Voiture {
  pricate $vitesse ; 
  private $modele ; 
  private $marque ; 

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

  public function getmodel() {
      return $this -> model ;
  }
  public function getmarque () {
      return $this -> marque ;
  }
  public function setmodel($model) {
     $this -> model = $model ; 
     
  }

  public function setmarque ($marque) {
     $this -> marque = $marque ; 
  }

  public function getVitesse(){
     return $this -> vitesse ; 
  }

  public function setVitesse($v) {
     if($v >= 0) {
         $this -> vitesse = $v ; 
      }
  }

}

3- 

class CompteBancaire {

   private $solde ; 

   public function deposer($deposer) {
      $this -> deposer += $deposer ;
   }

   public function retirer($returer) {
      if($this -> solde >= 0) {
       $this -> solde -= $returer
      }
      
   }
   public double getSolde() {
        return this.solde;
    }

}
































