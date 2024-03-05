# Diagramme de classe

![Classes](uml/classes.png)

## Vrai ou faux

Etant donné le diagramme de domaine ci-dessus, les assertions suivantes sont-elles vraies ou fausses ? 
- Etudiant est une classe d’association : FAUX, la classe `Etudiant` n'est pas est une classe d'association (liée à une association) selon le diagramme UML
- Un étudiant peut participer à autant de cours qu’il veut : VRAI car la cardinalité est `*` du côté `Cours` de l'association `Cours`-`Etudiant`
- Plusieurs professeurs peuvent enseigner la même discipline : FAUX car la cardinalité est de `1` du côté `Professeur` de l'association `Professeur`-`Discipline`
- Un professeur peut enseigner plusieurs disciplines : VRAI car la cardinalité est `*` du côté `Discipline` de l'association `Professeur`-`Discipline`
- Un cours peut être enseigné à 2 étudiants : FAUX car la cardinalité du côté `Etudiant` est `5..30` (minimum 5, maximum 30, 2 <= 5) de l'association `Etudiant`-`Cours`
- Un cours peut être enseigné à 20 étudiants : VRAI car la cardinalité du côté `Etudiant` est `5..30` (minimum 5, maximum 30, 5 <= 20 <= 30) de l'association `Etudiant`-`Cours`

## Question ouverte

Représentez la même association avec la notation UML « petit losange » : voir le fichier uml.puml

- Quelles informations perd-on par rapport au diagramme ci-dessus ? On perd la valeur des cardinalités `*` du côté `Cours` de toutes les associations avec la classe `Cours` puisque `Cours` devient la relation ternaire entre `Professeur`, `Discipline`, et `Etudiant`. 