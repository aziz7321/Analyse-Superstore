# Analyse des Performances d'une Chaîne de Magasins de Fournitures de Bureau (Superstore)

## Description du Projet
Ce projet vise à analyser les performances commerciales d'une chaîne de magasins de fournitures de bureau (Superstore) aux États-Unis. L'objectif est de fournir des indicateurs de performance clés (KPI) et des visualisations pour aider à la prise de décision stratégique. En tant que débutant, ce projet me permet de mettre en pratique mes compétences en analyse de données, de la préparation des données à la création de tableaux de bord interactifs.

Ce tableau de bord permet de suivre et d'analyser :
*   Les ventes et les profits par région.
*   La performance des catégories et sous-catégories de produits.
*   La rentabilité par segment de clientèle.
*   L'évolution des ventes au fil du temps (tendance temporelle).

## Jeu de Données
Le jeu de données utilisé est le jeu de données public "Sample - Superstore". Il contient plus de 9900 commandes, réparties sur 4 ans (2014-2017). Il inclut des informations détaillées sur :
*   **Commandes** : ID de commande, dates, mode de livraison.
*   **Clients** : Nom, segment, région.
*   **Produits** : Catégorie, sous-catégorie, nom du produit.
*   **Financier** : Ventes, quantité, remise, profit.

## Contexte et Problématique
L'entreprise cherche à comprendre les dynamiques de son marché pour optimiser ses stocks, améliorer sa rentabilité et cibler ses efforts marketing. Les questions auxquelles ce projet tente de répondre sont :
*   Quelles sont les régions les plus performantes ?
*   Quelles catégories de produits génèrent le plus de ventes et de profits ?
*   Certains segments de clientèle sont-ils plus rentables que d'autres ?
*   Y a-t-il une tendance saisonnière dans les ventes ?

## Méthodologie et Outils
L'analyse a été réalisée en plusieurs étapes :

1.  **Exploration et Compréhension des Données** : Analyse de la structure du fichier Excel, identification des différentes feuilles de calcul et de leur contenu (commandes détaillées, tableaux récapitulatifs).
2.  **Nettoyage et Préparation des Données (Data Wrangling) avec Excel** :
    *   Vérification de la cohérence des données (types de données, valeurs manquantes).
    *   Création de nouvelles colonnes calculées, telles que la **Marge Nette** (Profit / Sales) et l'**Année** extraite de la date de commande.
3.  **Analyse Exploratoire des Données (EDA) avec Excel (Tableaux Croisés Dynamiques - TCD)** :
    *   Création de TCD pour synthétiser les ventes par Région, Catégorie/Sous-Catégorie, Segment de clientèle et Année (comme vu dans les premières feuilles du fichier).
4.  **Création d'un Tableau de Bord (Dashboard)** :
    *   Conception d'une feuille de synthèse ("TCD_KPI") reprenant les KPI globaux (Ventes totales, Profit total, Nombre de commandes).

### Outils Utilisés
*   **Microsoft Excel** : Pour le stockage des données, le nettoyage, l'analyse avec les tableaux croisés dynamiques et les formules.

## Résultats et Analyse

*   **Performance Globale** : Sur la période, le Superstore a réalisé un chiffre d'affaires total de **2 295 274 €** et un bénéfice total de **285 988 €** pour un total de **9 988 commandes**.
*   **Performance par Région** : La région **West** est la plus performante en termes de ventes (725 457 €) et de profit (108 418 €), suivie de près par la région **East**. La région **South** génère le moins de ventes, indiquant un potentiel de croissance.
   ![Performance par région](./image/Performance%20par%20region.png)
*   **Performance par Catégorie de Produits** :
    *   La catégorie **Technology** est celle qui génère le plus de ventes (834 227 $), avec les **Phones** comme sous-catégorie phare.
    *   Les **Tables** dans la catégorie **Furniture** semblent être un point d'attention, avec des ventes importantes mais probablement des marges plus faibles, suggérées par des remises élevées.

    ![Performance par catégorie](./image/Performance%20par%20categorie%20et%20sous%20categorie%20.png)

*   **Rentabilité par Segment de Clientèle** : Le segment **Consumer** est le plus important, générant près de la moitié du profit total (134 017 $), suivi par **Corporate** et **Home Office**.
*   **Tendance Temporelle** : Les ventes sont en constante augmentation de 2014 à 2017, passant de 483 722 $ à 732 514 $. Cette croissance annuelle est un très bon signe pour l'entreprise.
    
    ![Tendance Temporelle](./image/Tendance%20temporelle.png)

## Comment utiliser ce projet
1.  **Cloner le dépôt** :
    ```bash
    git clone [https://github.com/aziz7321/Analyse-Superstore.git](https://github.com/aziz7321/Analyse-Superstore.git)
    ```
2.  **Ouvrir le fichier de données** : Le fichier principal est `Sample - Superstore.csv.xlsx`. Tu peux l'ouvrir avec Excel (ou tout autre tableur).
3.  **Explorer l'analyse** :
    *   La feuille **`Sample - Superstore`** contient les données brutes.
    *   Les autres feuilles ( `Performance par Région`, `Analyse de la Rentabilité (Marg`, etc.) sont les résultats de l'analyse via des tableaux croisés dynamiques.
    *   Tu peux recréer ces TCD ou en créer de nouveaux pour explorer d'autres pistes (par exemple, performance par mode de livraison, impact des remises sur les ventes, etc.).

## Auteur
*   **Abdoulaziz Keita**

## Licence
Ce projet est sous licence MIT - voir le fichier [LICENSE](LICENSE) pour plus de détails.