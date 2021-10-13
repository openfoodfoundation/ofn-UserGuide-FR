# Ajouter des produits

Cette fonctionnalité permet d'ajouter des produits un par un à votre catalogue. Pour un ajout de produit en masse par import de fichier, consultez la page "[Import produits en masse](import-de-produits-et-catalogue.md)" Une fois connecté sur l'interface d'administration, cliquez sur le menu **Produits**, puis sur le bouton **Nouveau Produit**.

![](<../../.gitbook/assets/image (15).png>)

Vous serez redirigé vers la page suivante :

![](../../.gitbook/assets/ajouter_un_produit.png)

** Fournisseurs : **Sélectionnez le fournisseur à l'origine du produit.

> Si vous êtes producteur, il faut vous sélectionner vous-même. Si vous êtes un hub, n'oubliez pas que vous pouvez uniquement ajouter des produits pour les producteurs pour lesquels vous avez créé un profil ou qui vont ont donné les droits de modification de leurs produits.

**Nom du produit : ** C'est le nom du produit qui sera affiché dans la boutique.

{% hint style="info" %}
L'ordre d'affichage par défaut des produits est alphabétique. Vous pouvez modifier cet affichage à l'aide du champ "ordre d'affichage des catégories" dans [**Préférences boutique**](https://ofn-user-guide.gitbook.io/guide-utilisateur-open-food-network/fonctionnalites-standards/votre-profil/parametres#preferences-boutique)** **
{% endhint %}

**Unités de mesure : **Indiquez via quelle unité le produit sera vendu (L, kg, pièces...).

> Si vous choisissez g et saisissez ensuite 1000, le produit sera affiché comme 1kg pour l'acheteur. Gardez en tête que le choix de l'unité de mesure va impacter le fonctionnement de certains frais et marges et commissions. Par exemple, un frais fixe au poids ne pourra s'appliquer que sur les produits paramétrés au kg. Vous pouvez dans ce cas saisir des nombres d'unité non entières, comme 0.2 kg et le produit s'affichera comme 200 g mais sera bien traité au kg dans les rapports et pour le calcul des frais.

**Nombre d'unités :** Par exemple si c'est 100 g, il faudra indiquer ici 100.

**Unité affichée** **:** Ce champ affiche automatiquement de quelle manière les champs unité de mesure et nombre d'unités vont être affichés, une fois les deux champs complétés (exemple, si vous avez indiqué kg, puis 2, le champ affichera 2kg). Vous pouvez "forcer" l'affichage d'une unité différente en écrivant par dessus la proposition automatique.

> Remarque : Si votre unité est en pièces (boite, bouquet...) ce champ se changera en "**unité**". Complétez ce champ avec le nom de la pièce (boite, bouquet, pot...).

**Catégorie de produit** **:** Sélectionnez la catégorie la plus appropriée pour le produit. Ces catégories faciliteront la recherche de certains produits par les acheteurs, qui pourront filtrer les produits par catégorie de produit.

**Prix :** Indiquez le prix pour le produit tel que précédemment renseigné (pour ce conditionnement spécifique donc).

> Remarque : il s'agit du prix de base du producteur. Les marges et les commissions sont renseignées dans le menu marges et commissions du paramétrage de l'entreprise, et appliquées au moment de la création du cycle de vente pour s'imputer sur le prix du produit tel qu'affiché dans la boutique. 

****\
**Prix unitaire: **Ce prix n'est pas modifiable, il est calculé automatiquement en fonction du nombre d'unités vendues.\
****\
**En stock** **:** Indiquez le stock de produit disponible à la vente.

> Utilisez ce champ si vous voulez suivre votre stock. Lorsque les acheteurs réaliseront des commandes, le niveau du stock se réduira automatiquement et lorsqu'il atteindra 0 le produit ne sera plus visible dans votre boutique. Si vous ne souhaitez pas gérer votre stock dans la plateforme, ou si le produit est disponible à la demande (autant que souhaité), cochez "à volonté" (paragraphe suivant).

**A volonté** **:**  Si vous cochez cette case, la boutique indiquera que le produit est toujours disponible. La plateforme ne vérifie donc plus les stocks, et considère que le produit est toujours en stock.

**Photo :** Téléchargez une photo du produit.

![](<../../.gitbook/assets/Capture d’écran 2020-10-28 à 16.33.15.png>)

{% hint style="warning" %}
Nous recommandons d'uitiliser des photos de bonne qualité, sur un format carré. De préférences de vraies photos de vos produits plutôt que des images internet, ce qui rend le produit plus attractif pour le consommateur (pensez à vérifier les droits si vous utilisez des images du web)
{% endhint %}



**TVA applicable :** Sélectionnez la TVA applicable dans la liste déroulante. La TVA dépend de la nature du produit, la plupart des produits alimentaires sont soumis en Belgique par exemple à une TVA de 6%. 

> Attention cela n'a pas d'impact sur le fait que la TVA sera collectée ou pas sur le montant de vente TTC par une entreprise. Cette fonctionnalité dépend du [paramétrage de l'entreprise, rubrique "juridique"](../votre-profil/parametres.md#juridique), "Soumis à la TVA?"

**Description du produit :** Ce champ vous permet de décrire le produit vendu, pour donner plus d'informations à l'acheteur final. N'hésitez pas raconter l'histoire de la variété de la tomate, etc. Vous pouvez aussi ajouter un lien hypertexte, vers un certificat de labellisation par exemple.

{% hint style="info" %}
N'oubliez pas de bien cliquer sur le bouton "créer" ou "créer et ajouter nouveau" une fois tous les champs obligatoires renseignés (ceux indiqués par une astérisque rouge).
{% endhint %}

Lorsque vous créez un produit, vous êtes redirigé sur la page "produits" où vous retrouvez tous vos produits :

![](<../../.gitbook/assets/image (18).png>)

### Créer un produit similaire / une déclinaison du produit

Si vous créez deux produits similaires dont seul le prix ou la taille ou les ingrédients varient, le mieux est de créer une "variante" du produit plutôt qu'un deuxième produit entier. Pour créer une variante, veuillez suivre le processus indiqué [ici](product-variants.md). Vous avez aussi la possibilité de dupliquer un produit en cliquant sur le pictogramme des deux petites feuilles à droite de la ligne du produit concerné (pictogramme du milieu).

{% hint style="success" %}
Les variantes sont un gain de temps, par exemple si vous vendez des citrons individuelement et par pack de 5 et de 10, vous aurez un produit à 3 variantes plutôt que 3 produits.
{% endhint %}

Si vous souhaitez créer un produit similaire, vous pouvez le copié / coller le produit initial puis modifier le nouveau grâce aux icones à droite de celui-ci.

![](<../../.gitbook/assets/Capture d’écran 2020-10-28 à 17.18.16.png>)

### Affiner les attributs des produits

Vous pouvez ajouter des **propriétés/labels** à vos produits par soucis de transparence pour l'acheteur, pour mettre en valeur les qualités de vos produits, et permettre les recherches basées sur ce critère. Cliquez [ici](product-properties.md) pour en savoir plus.

Pour les** produits "irréguliers"** type viande, vous trouverez [ici](pricing-irregular-items-kg.md) quelques conseils sur la façon de saisir et gérer ces produits.

Pour les **achats groupés **de produits vendus en gros lots, un paramétrage et une fonctionnalité dédiée vous aide à organiser les achats groupés pour tomber pile poil sur la quantité du lot. Cliquez [ici](group-buy-for-bulk-ordering.md) pour en savoir plus.

### Recherche par mots clés

L'acheteur peut filtrer les produits par catégorie de produit depuis la vue boutique (à droite de la vue produit). Il peut également effectuer une recherche par mot clés depuis l'encart "rechercher..." (en haut de la vue produit).

![](<../../.gitbook/assets/Capture d’écran 2020-10-28 à 18.16.31.png>)

Les champs suivants peuvent être recherchés depuis l'encart "rechercher.."\
\- Nom du produit\
\- Nom de la variante\
\- Nom du producteur\
\- Mot clé de recherche

Vous pouvez définir des **mots clés de recherche** en vous rendant dans **produits > modifier > rechercher. **Les mots clés renseignés dans l'encart rouge sont examinés par la plateforme si l'acheteur utilise ce mot clé lors de sa recherche. Ceux renseignés dans l'encart vert sont examinés par des moteurs de recherche externes sur internet (ex : Google) 

![](<../../.gitbook/assets/Capture d’écran 2020-10-28 à 18.29.06.png>)
