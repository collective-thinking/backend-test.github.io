# SQl

## 1. Requêtages SQL

![]( ../../images/schema-sql.jpg)

A. Ecrivez la requête qui permet de récupérer les séjours qui ont des prédictions ordonnées par leur score décroissant et dont les dates de softDelete (deleted_at) sont NULL.

B. Ecrivez la requête qui permet de compter le nombre de documents par type de documents (même ceux qui n’en ont pas) et dont les dates de softDelete (deleted_at) sont NULL.

C. Ecrivez la requête qui permet de récupérer un séjour qui a une prédiction et dont la date de sortie (end_date) est comprise entre le début et la fin de cette année et dont les dates de softDelete (deleted_at) sont NULL, limiter le nombre de résultat à 50.

D. Ecrivez la requête qui permet de récupérer les identifiants de séjour (stay_id) qui ont au moins 2 documents et dont les dates de softDelete (deleted_at) sont NULL.

E. Ecrivez la requête qui permet de récupérer le nombre de documents moyen par séjour.

F. Ecrivez la requête qui permet de récupérer les identifiants de séjour (stay_id) et les dates de séjour (start_date, end_date) qui ont un identifiant de séjour qui commence par 192 OU qui qui ont une date de sortie avant la fin de cette année et dont les dates de softDelete (deleted_at) sont NULL.


## 2. Architecture SQL

![]( ../../images/schema-sql-colonne.jpg)
<pre>
SELECT first_name,last_name,gender,ipp FROM patient WHERE gender = 'male';
</pre>
Considérant le schéma et la requête ci-dessus, quelles optimisations sont possibles pour améliorer la rapidité de la requête.