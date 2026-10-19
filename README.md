# Artificial Inquiries --- Exercice 13

## 1. Présentation de l'exercice

L'exercice **Ex13 -- Setting Up the Example** consiste à choisir un
travail professionnel exemplaire, à expliquer son contexte et à évaluer
les caractéristiques qui le rendent pertinent. Les deux supports fournis
sont :

-   **Ex13a -- Mapping Exemplary Patterns / Playground** : évaluation du
    document ou travail choisi à l'aide de huit critères notés de 1 à 5,
    puis représentation des notes sous la forme d'un graphique radar.
-   **Ex13b -- Fill in the Blanks** : rédaction d'un paragraphe
    justifiant le caractère exemplaire du travail choisi.

Pour ce dépôt, l'exemple retenu est **Wikipédia**, considéré comme un
exemple de documentation collaborative et de partage de connaissances.
L'analyse porte sur le fonctionnement de l'encyclopédie et sur les
pratiques de rédaction, de vérification et de collaboration qu'elle
illustre.

## 2. Objectifs

1.  Décrire le contexte et l'intérêt de l'exemple retenu.
2.  Évaluer cet exemple selon huit critères communs.
3.  Visualiser l'évaluation avec un graphique radar.
4.  Rédiger une justification structurée de son caractère exemplaire.
5.  Décrire les données dans un modèle de classes réutilisable.
6.  Préparer un environnement Omeka S local pour organiser et documenter
    les ressources du projet.

## 3. Critères d'évaluation

Chaque critère reçoit une note entière de **1 à 5**. Les notes
ci-dessous sont une **proposition initiale à discuter et à ajuster**, et
non des résultats mesurés ou imposés par le formulaire.

  ------------------------------------------------------------------------
  Critère               Signification                        Note proposée
  --------------------- --------------------- ----------------------------
  Frequency             Fréquence à laquelle                             5
                        ce type de document   
                        est produit ou        
                        consulté              

  Professional Stakes   Conséquences d'une                               4
                        réussite ou d'un      
                        échec pour la         
                        réputation            
                        professionnelle       

  Expertise Required    Niveau de                                        3
                        connaissances et de   
                        compétences           
                        spécialisées requis   

  Effort and Resources  Temps, effort et                                 4
                        outils nécessaires    

  Collaboration         Importance du travail                            5
                        collectif             

  Error Tolerance       À quel point                                     5
                        l'absence d'erreur    
                        est essentielle       

  Standardisation       Degré de                                         4
                        standardisation du    
                        type de document      

  Professional Pride    Contribution au                                  4
                        sentiment             
                        d'accomplissement     
                        professionnel         
  ------------------------------------------------------------------------

Les valeurs doivent être revues par l'étudiant à partir de l'exemple
concret retenu. Pour le critère **Error Tolerance**, une note élevée
signifie que les erreurs sont peu tolérées.

## 4. Proposition de paragraphe pour Ex13b

> Wikipédia est un exemple intéressant parce qu'il contribue à la
> production et au partage de connaissances accessibles. Il s'inscrit
> dans le domaine de la documentation et de la médiation de
> l'information, où la fiabilité et la clarté sont essentielles. Il
> répond au problème de la diffusion de connaissances à grande échelle
> en proposant des articles modifiables et consultables en ligne. Son
> fonctionnement se distingue par la collaboration entre contributeurs,
> la possibilité de corriger les contenus et l'utilisation de références
> pour étayer les informations. Il reflète des valeurs professionnelles
> telles que la transparence, la vérifiabilité, la coopération et
> l'amélioration continue. Je souhaite m'inspirer de sa structuration de
> l'information, de la traçabilité des contributions et de ses
> mécanismes de correction, car ces pratiques favorisent une
> documentation compréhensible et réutilisable.

Ce paragraphe est une base à personnaliser : il faut préciser ce que
vous souhaitez réellement reproduire et justifier ce choix avec votre
propre analyse.

## 5. Solutions techniques envisagées

### GitHub

Le dépôt versionne les fichiers du projet, permet de documenter les
choix et facilite le travail collaboratif. Le dépôt demandé est
`ArtificialInquiries_13`.

### Mermaid

Le fichier `diagram_class.md` contient un diagramme de classes Mermaid.
Il modélise l'exemple étudié, ses critères, les évaluations, les notes
et la justification textuelle. Le diagramme peut être prévisualisé ou
testé sur [Mermaid Live Editor](https://mermaid.live/).

### Omeka S

Omeka S peut servir à organiser les ressources documentaires associées à
l'exercice et à leur ajouter des métadonnées. Il ne calcule pas
automatiquement le graphique radar par défaut : celui-ci peut être
produit par un script ou une interface dédiée, puis associé à une
ressource Omeka S.

### Architecture locale

-   **Apache** : serveur HTTP local.
-   **PHP** : environnement d'exécution d'Omeka S.
-   **MySQL** : base de données.
-   **Omeka S** : gestion des ressources et de leurs métadonnées.
-   **Mermaid** : représentation du modèle de données.
-   **Git/GitHub** : versionnement et collaboration.

Les versions exactes de PHP, MySQL et des extensions requises doivent
être vérifiées dans la documentation officielle d'Omeka S avant
l'installation.

## 6. Installation et test d'Omeka S

1.  Installer Apache, PHP, MySQL et les extensions PHP requises par la
    version d'Omeka S choisie.
2.  Télécharger Omeka S depuis le site officiel et placer les fichiers
    dans le répertoire servi par Apache.
3.  Créer une base de données MySQL et un utilisateur dédié à Omeka S.
4.  Configurer le fichier de configuration de la base de données selon
    la documentation officielle.
5.  Ouvrir l'adresse locale du site dans un navigateur et suivre
    l'assistant d'installation.
6.  Créer le compte administrateur et terminer la configuration.
7.  Se connecter à l'interface d'administration, créer un premier
    contenu de test et vérifier qu'il est enregistré et consultable.
8.  Documenter les versions installées, les étapes effectuées et les
    éventuels messages d'erreur.

Documentation officielle : https://omeka.org/s/docs/user-manual/install/

### Critères de validation

-   La page d'accueil locale d'Omeka S s'affiche.
-   L'accès à l'administration fonctionne.
-   Un contenu de test peut être créé et enregistré.
-   Les métadonnées du contenu sont visibles.
-   Les étapes et les résultats des tests sont consignés dans le dépôt.

## 7. Collaborateur GitHub

Ajouter le compte GitHub **`samszo`** dans les paramètres du dépôt :
**Settings → Collaborators** (ou **Collaborators and teams**) → **Add
people**. Sélectionner le bon compte et envoyer l'invitation. L'ajout
n'est effectif qu'après l'action dans GitHub et, selon le cas,
l'acceptation de l'invitation.

## 8. Fichiers du dépôt

-   `README.md` : description, modèle d'évaluation, solutions techniques
    et protocole de test.
-   `diagram_class.md` : diagramme de classes Mermaid.
-   `captures_formulaire/` : captures des formulaires papier fournis.

## 9. Références

-   Documentation d'installation Omeka S :
    https://omeka.org/s/docs/user-manual/install/
-   Syntaxe des diagrammes de classes Mermaid :
    https://mermaid.ai/open-source/syntax/classDiagram.html
-   Éditeur Mermaid : https://mermaid.live/

## 10. Captures des formulaires papier de l'exercice

Les captures ci-dessous reproduisent les pages de l'exercice fournies. Elles sont intégrées directement dans ce README avec des chemins relatifs : elles s'afficheront aussi sur GitHub tant que le dossier `captures_formulaire` est conservé dans le dépôt.

### Présentation de l'exercice — Ex13

![Ex13 – Setting Up the Example](captures_formulaire/01_ex13_setting_up_example.png)

### Ex13a — Instructions et critères d'évaluation

![Ex13a – Instructions](captures_formulaire/02_ex13a_instructions.png)

![Ex13a – Critères complémentaires](captures_formulaire/03_ex13a_criteria.png)

### Ex13a — Tableau des critères

![Ex13a – Tableau des critères](captures_formulaire/04_ex13a_table.png)

![Ex13a – Suite du tableau des critères](captures_formulaire/06_ex13a_table_continued.png)

### Ex13a — Graphique radar

![Ex13a – Graphique radar vierge](captures_formulaire/05_ex13a_radar_graph.png)

### Ex13b — Fill in the Blanks

![Ex13b – Formulaire à compléter](captures_formulaire/07_ex13b_fill_in_the_blanks.png)
