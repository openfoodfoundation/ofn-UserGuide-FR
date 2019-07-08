---
description: >-
  Cette page vous permet de découvrir la fonctionnalité d'import de produits ou
  de cataogue : en quelques clis, créez ou mettez à jour plusieurs produits en
  une seule fois !
---

# Import produits et catalogue

{% hint style="info" %}
Cette fonctionnalité arrive bientôt !
{% endhint %}

Cet outil vous permet de téléverser un fichier csv pour ajouter ou mettre à jour votre stock.

Pour vous rendre sur la fonctionnalité, cliquez sur le menu principal **Produits** puis le sous-menu **import produit**. 

Les 4 fonctionnalité principales de l'outil :

1. Importer de nouveau produits
2. Mettre à jour des caractéristiques produits existantes
3. Importer un nouveau catalogue
4. Mettre à jour les caractéristiques d'un catalogue

Dans chacun des cas, il vous faudra télécharger un exemple de fichier csv sur la plateforme, le remplir et le téléverser ensuite sur la plateforme.

{% hint style="info" %}
**Important** : Microsoft Excel ne permet pas l'ouverture "directe" d'un tableur en csv. Si vous le pouvez, nous vous conseillons d'utiliser les tableurs libres de LIbres Office [https://www.libreoffice.org/download/download/](https://www.libreoffice.org/download/download/) Avec Libre Office Calc, vous pourrez ouvrir directement le fichier csv et l'enregistrer au bon format d'encodage UTF-8. Si vous préférez tout de même utiliser Microsoft Excel, veuillez suivre la procédure suivante pour ouvrir un fichier csv: [https://support.office.com/fr-fr/article/Importer-ou-exporter-des-fichiers-texte-txt-ou-csv-5250ac4c-663c-47ce-937b-339e391393ba](https://support.office.com/fr-fr/article/Importer-ou-exporter-des-fichiers-texte-txt-ou-csv-5250ac4c-663c-47ce-937b-339e391393ba)
{% endhint %}

## Importer de nouveaux produits <a id="import-new-products"></a>

Tout d'abord, téléchargez le modèle sur la page d'import et ouvrez-le avec Libre Office \(ou Excel ou équivalent\).

Le modèle indique les colonnes à remplir pour réussir l'import. Consultez les informations ci-dessous pour bien remplir le fichier.

{% hint style="info" %}
**Attention à la casse** : il faut utiliser par exemple mL et non ml !
{% endhint %}

Par ailleurs, certains champs ne sont pas encore disponibles via l'import produit \(les images, les labels...\).

| Titre de colonne | Obligatoire? | Description | Exemple |
| :--- | :--- | :--- | :--- |
| producer | Oui | Le nom du producteur des produits que vous souhaitez importer | La belle ferme |
| sku | Non | La référence produit | AD001265 |
| name | Oui | Le nom du produit | Carotte |
| display name | Non | Ce champ s'applique uniquement si vous importez des variantes \(voir plus bas\). Dans le cas contraire vous pouvez le laisser vide. | Carotte rouge |
| category | Oui | Les catégories disponibles sont listées sur la page d'import produit. Veuillez indiquer ici la catégorie du produit | Poisson |
| units | Oui | Le poids, le volume ou la quantité | 500 |
| unit\_type | Oui | Sous quelle unité est vendu le produit ? \(grammes, litres,... ?\) S'il est vendu en tant que lot, laissez vide | g |
| variant\_unit\_name | ? | Si le produit est vendu en lot, indiquez le type de lot ici | Botte |
| price | Oui | Le prix du produit TTC | 3.70 |
| on\_hand | Non | Si le stock du produit est limité, indiquez la limite ici, sinon laissez vide et renseingez la colonne on\_demand | 40 |
| available\_on | Non | Laissez vide | ​ |
| on\_demand | Non | Si vous avez un stock infini du produit, indiquez 1 et si vous utilisez la colonne on\_hand laissez vide | 1 |
| shipping\_category | Oui | Les catégories de livraison disponibles sont listées sur la page d'import produit. Veuillez indiquer ici la catégorie de livraison du produit \(réfrigéré, ...\) | ​ |
| tax\_category | Non | Si le prix de votre produit inclus de la TVA, indquez TVA sinon laissez vide | TVA |
| description | Non | Vous pouvez créer une description mais pas la mettre à jour pour l'instant. | Ces carottes sont lavées par nos soins avant la livraison |

### Les variantes <a id="variants"></a>

​[Les variantes](product-variants.md) peuvent être distinguée par les unitées \(par exemple un produit vendu par 500 g ou 1 kg\) ainsi que le champ display\_name \(exemple : Yaourt à la myrtille, fraise...\). Chaque variante est regroupée sous le même nom produit. Exemple :

| name | display\_name | price | units | unit\_type |
| :--- | :--- | :--- | :--- | :--- |
| Farine de sarasin | ​ | 3.50 | 500 | g |
| Farine de sarasin | ​ | 5.50 | 750 | g |
| Yaourt | Fraise | 4 | 200 | g |
| Yaourt | Myrtille | 4 | 200 | g |

Pour rappel exemple d'affichage pour l'acheteur d'un produit avec 3 variantes :

![](../../.gitbook/assets/image%20%2892%29.png)

### Exemple d'unités <a id="variants-1"></a>

Un exemple d'import avec des unités différentes :

| supplier | **name** | **category** | **price** | **units** | **unit\_type** | **variant\_unit\_name** |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Producteur A | Patate douce | Légumineuses | 3.50 | 500 | g |  |
| Producteur B | Bar | Poisson | 3.50 | 300 | ml |  |
| Producteur C | Pommes | Fruits & légumes | 9.50 | 5 | kg |  |
| Producteur D | Persil | Herbes & épices | 3.00 | 1 |  | botte |

#### Import the CSV

Une fois votre fichier csv prêt, vous pouvez le téléverser sur Open Food Network.

Allez sur **Produits** &gt; **Import produit**

**Sélectionnez "import catalogue produit"**

**Sélectionnez votre fichier.**

Cliquez sur **Importer**.

Avant que l'import ne se lance, vous verrez un récapitulatif. C'est le moment de vérifier si une erreur ne s'est pas glissée dans votre fichier !

## Mettre à jour des caractéristiques produits existantes <a id="update-existing-product-details"></a>

Comment mettre à jour des produits existants ?

Le processus est similaire à la création de produit.  6 champs sont obligatoires pour que l'import fonctionne et seul 5 champs sont modifiables via l'import :

| Champs obligatoires \(non modifiables\) | Champs modifiables | Champs non modifiables et non obligatoires |
| :--- | :--- | :--- |
| producer | sku | variant\_unit\_name |
| name | price | tax\_category |
| category | on\_hand | shipping\_category |
| units | on\_demand | ​description |
| unit\_type \(si applicable\) |  | ​ |
| variant\_unit\_name \(si applicable\) | ​ | ​ |
| display\_name |  |  |

## Importer un catalogue ou le mettre à jour <a id="import-new-inventory"></a>

Tout d'abord, téléchargez le modèle sur la page d'import et ouvrez-le avec Libre Office \(ou Excel ou équivalent\).

Le modèle indique les colonnes à remplir pour réussir l'import. Consultez les informations ci-dessous pour bien remplir le fichier.

{% hint style="info" %}
**Attention à la casse** : il faut utiliser par exemple mL et non ml !
{% endhint %}

Par ailleurs, certains champs ne sont pas encore disponibles via l'import produit \(les images, les labels...\).

| Titre de colonne | Obligatoire? | Description | Exemple |
| :--- | :--- | :--- | :--- |
| producer | Oui | Le nom du producteur des produits que vous souhaitez importer | La belle ferme |
| distributor | Oui | Le nom du hub qui va vendre le produit | Hub demo |
| sku | Non | La référence produit | AD001265 |
| name | Oui | Le nom du produit | Carotte |
| display name | Non | Ce champ s'applique uniquement si vous importez des variantes \(voir plus bas\). Dans le cas contraire vous pouvez le laisser vide. | Carotte rouge |
| category | Oui | Les catégories disponibles sont listées sur la page d'import produit. Veuillez indiquer ici la catégorie du produit | Poisson |
| units | Oui | Le poids, le volume ou la quantité | 500 |
| unit\_type | Oui | Sous quelle unité est vendu le produit ? \(grammes, litres,... ?\) S'il est vendu en tant que lot, laissez vide | g |
| variant\_unit\_name | Oui | Si le produit est vendu en lot, indiquez le type de lot ici | Botte |
| price | Oui | Le prix du produit TTC | 3.70 |
| on\_hand | Non | Si le stock du produit est limité, indiquez la limite ici, sinon laissez vide et renseingez la colonne on\_demand | 40 |
| available\_on | Non | Laissez vide | ​ |
| on\_demand | Non | Si vous avez un stock infini du produit, indiquez 1 et si vous utilisez la colonne on\_hand laissez vide | 1 |

#### Import the CSV

Une fois votre fichier csv prêt, vous pouvez le téléverser sur Open Food Network.

Allez sur **Produits** &gt; **Import produit**

**Sélectionnez "import catalogue produit"**

**Sélectionnez votre fichier.**

Cliquez sur **Importer**.

Avant que l'import ne se lance, vous verrez un récapitulatif. C'est le moment de vérifier si une erreur ne s'est pas glissée dans votre fichier !

