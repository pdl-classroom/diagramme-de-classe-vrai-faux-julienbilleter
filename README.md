# Diagramme de classe

![Classes](uml/classes.png)

## Vrai ou faux

Etant donné le diagramme de domaine ci-dessus, les assertions suivantes sont-elles vraies ou fausses ? 
- Etudiant est une classe d’association : FAUX car Etudiant est une classe normale (conceptuelle) selon le diagramme
- Un étudiant peut participer à autant de cours qu’il veut : VRAI car la cardinalité est * du côté de la relation Cours-Etudiant
- Plusieurs professeurs peuvent enseigner la même discipline : FAUX car pour une Discipline il y a 1 enseignant (côté Enseignant la cardinalité est 1)
- Un professeur peut enseigner plusieurs disciplines : VRAI car la cardinalité du côté Discipline est *
- Un cours peut être enseigné à 2 étudiants : FAUX car la cardinalité du côté Etudiant est 5..30
- Un cours peut être enseigné à 20 étudiants : VRAI car la cardinalité du côté Etudiant est 5..30

## Question ouverte

Représentez la même association avec la notation UML « petit losange » 

- Quelles informations perd-on par rapport au diagramme ci-dessus ? 