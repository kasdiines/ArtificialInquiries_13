# Diagramme de classes --- Ex13

Le diagramme ci-dessous représente les données nécessaires pour
documenter l'exemple choisi, saisir les huit notes de l'exercice Ex13a
et conserver la justification rédigée pour Ex13b.

``` mermaid
classDiagram
    class ExempleProfessionnel {
        +int id
        +string titre
        +string description
        +string domaine
        +string urlReference
    }

    class Evaluation {
        +int id
        +date dateEvaluation
        +string commentaireGeneral
        +calculerScoreMoyen()
    }

    class Critere {
        +int id
        +string nom
        +string description
        +string echelle
    }

    class NoteCritere {
        +int id
        +int valeur
        +string commentaire
    }

    class Justification {
        +int id
        +string contributionPrincipale
        +string domaineProfessionnel
        +string problemeTraite
        +string solutionProposee
        +string valeursProfessionnelles
        +string elementAEmuler
    }

    class RessourceDocumentaire {
        +int id
        +string titre
        +string type
        +string uri
        +string description
    }

    ExempleProfessionnel "1" --> "0..*" Evaluation : est évalué dans
    Evaluation "1" *-- "8" NoteCritere : contient
    Critere "1" --> "0..*" NoteCritere : définit
    Evaluation "1" --> "0..1" Justification : possède
    ExempleProfessionnel "1" --> "0..*" RessourceDocumentaire : documenté par
```

## Règles de gestion

-   Une évaluation porte sur un exemple professionnel.
-   Une évaluation comporte une note pour chacun des huit critères.
-   Une note est comprise entre **1 et 5**.
-   Chaque note est associée à un critère unique.
-   Une évaluation peut posséder une justification textuelle.
-   Un exemple peut être documenté par plusieurs ressources.

## Critères à initialiser

Les huit critères à créer sont : `Frequency`, `Professional Stakes`,
`Expertise Required`, `Effort and Resources`, `Collaboration`,
`Error Tolerance`, `Standardisation` et `Professional Pride`.

## Lien avec Omeka S

Ce diagramme est un modèle conceptuel pour expliquer les données de
l'exercice. Il ne signifie pas que ces classes doivent être créées
automatiquement comme tables MySQL dans Omeka S. Dans Omeka S, les
exemples et les ressources peuvent être représentés par des **items**,
avec des métadonnées et des vocabulaires adaptés. Une extension ou un
développement spécifique serait nécessaire pour automatiser la saisie
des notes et le calcul du graphique radar.
