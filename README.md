# html-table-fusion-columns

> HTML exercise about tables

* * *

**html-table-fusion-columns** is an educational project, which will be used for HTML courses.

**Note:** the school where the course is given, the [HEPL](http://www.provincedeliege.be/hauteecole) from Liège, Belgium, is a french-speaking school. From this point, the instruction will be in french. Sorry.

* * *

## Exercice sur les tableaux

Complétez le fichier `index.html` avec les bonnes balises afin d'arriver au résultat *très kitsch* suivant :

![Résultat attendu](assets-starter/rendu.png)

L’objectif de cet exercice est de réaliser une table avec des fusions de colonnes.

### Aides

1. Commencez par baliser la table comme s’il n’y avait pas de fusions ;
2. Ajoutez les attributs `colspan` nécessaires pour fusionner les colonnes ;
3. Ajoutez les attributs d’accessibilité pour lier les cellules de données et les cellules de titre (vous devez ici,
   obligatoirement, travailler avec les attributs `id`/`headers` car il y a des fusions de colonnes dans le
   tableau) ;
4. N’oubliez pas les entités pour les caractères spéciaux ;
5. N’oubliez pas non plus de valider régulièrement votre code ;
6. Liez la feuille de styles et ajouter les attributs *éventuellement* nécessaires pour obtenir le rendu final (pour obtenir le même rendu que sur l'image,  il faut notamment ajouter la _classe_ `vide` sur les cellules en question).

### Astuce

Pour autant que l’extension *Emmet* soit installée dans votre éditeur de texte, vous pouvez utiliser, comme vu aux
séances de TPs, des raccourcis pour générer plus rapidement des patterns de lignes qui se répètent.

Voici, pour rappel, les symboles utiles et leur signification :

- `>` : enfant direct (quand on souhaite imbriquer une balise à l’intérieur d’une autre) ;
- `+` : frère adjacent (quand on souhaite imbriquer une balise à la suite d’une autre à l’intérieur du même parent) ;
- `[]` : pour ajouter un attribut dans une balise ;
- `*` : pour répéter un pattern ;
- `()` : pour regrouper des patterns qui doivent se répéter.

Exemple :

`(tr>th[id=""]+(td[headers=""]*3))*8` + `TAB`

va générer 8 lignes (8 balises `tr`) qui contiennent toutes un `th`avec un attribut `id`et 3 `td` avec chacun un attribut `headers` comme ceci :

```html 
<tr>
	<th id=""></th>
	<td headers=""></td>
	<td headers=""></td>
	<td headers=""></td>
</tr>
<tr>
	<th id=""></th>
	<td headers=""></td>
	<td headers=""></td>
	<td headers=""></td>
</tr>
<tr>
	<th id=""></th>
	<td headers=""></td>
	<td headers=""></td>
	<td headers=""></td>
</tr>
<tr>
	<th id=""></th>
	<td headers=""></td>
	<td headers=""></td>
	<td headers=""></td>
</tr>
<tr>
	<th id=""></th>
	<td headers=""></td>
	<td headers=""></td>
	<td headers=""></td>
</tr>
<tr>
	<th id=""></th>
	<td headers=""></td>
	<td headers=""></td>
	<td headers=""></td>
</tr>
<tr>
	<th id=""></th>
	<td headers=""></td>
	<td headers=""></td>
	<td headers=""></td>
</tr>
<tr>
	<th id=""></th>
	<td headers=""></td>
	<td headers=""></td>
	<td headers=""></td>
</tr>
```
