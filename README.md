Jour 1 : UML - Fondamentaux des Diagrammes de Classes
● Objectif du jour : Comprendre qu'une classe représente un concept métier avec des
données (attributs) et des actions (méthodes).

1. Qu'est-ce qu'une classe dans un diagramme de classes ? : Une classe est une représentation abstraite d'un objet. Elle définit sa structure via ses attributs et son comportement via ses méthodes .

   
2. Pourquoi est-il problématique d'avoir des classes sans méthodes ? :C'est problématique car cela viole la logique de la POO et le principe d'encapsulation. Une classe sans méthodes est équivalente à une simple structure de données . Par conséquent, les objets instanciés sont passifs et leurs attributs peuvent être modifiés directement par n'importe quelle classe externe, ce qui rend l'état de l'objet instable.

3. Expliquer le principe de responsabilité unique. : Chaque classe doit avoir une seule responsabilité et donc une seule raison de changer. Elle doit se limiter à accomplir une seule tâche


● Challenges Pratiques :
1-
<img width="210" height="158" alt="image" src="https://github.com/user-attachments/assets/d2055b1c-1687-48e4-962b-265c7600cbc1" />

2-
<img width="231" height="333" alt="image" src="https://github.com/user-attachments/assets/09ac92ca-1621-41d8-bb78-810d6b562395" />

3-
<img width="512" height="179" alt="image" src="https://github.com/user-attachments/assets/b703399c-957f-4959-af5f-a096c77029b9" />

Le choix est justifié par la sémantique de l'action. C'est l'étudiant qui est l'acteur principal  qui effectue l'action de s'inscrire. Par conséquent, la méthode inscriptionAuCours appartient naturellement à la classe Etudiant.
