---
description: >-
  Cette page vous permet de découvrir la fonctionnalité d'import de produits ou
  de cataogue : en quelques clis, créez ou mettez à jour plusieurs produits en
  une seule fois !
---

# Import de produits et catalogue

{% hint style="info" %}
Cette fonctionnalité arrive bientôt !
{% endhint %}

Cet outil vous permet de téléverser un fichier csv pour ajouter ou mettre à jour votre stock.

Pour vous rendre sur la fonctionnalité, cliquez sur le menu principal **Produits** puis le sous-menu **import produit**. 

Les 4 fonctionnalité principalses de l'outil :

1. Importer de nouveau produits
2. Mettre à jour des caractéristiques produits existantes
3. Importer un nouveau catalogue
4. Mettre à jour les caractéristiques d'un catalogue

Dans chacun des cas, il vous faudra télécharger un exemple de fichier csv sur la plateforme, le remplir et le téléverser ensuite sur la plateforme.

## Importer de nouveaux produits {#import-new-products}

Tout d'abord, téléchargez le modèle sur OFF et ouvrez-le avec Libre Office \(ou Excel ou équivalent\).

Le modèle indique les colonnes à remplir pour réussir l'import. Consultez les informations ci-dessous pour bien remplir le fichier.

Attention à la casse : il faut utiliser par exemple mL et non ml :

| Titre de colonne | Obligatoire? | Description | Exemple |
| :--- | :--- | :--- | :--- |
| supplier | Oui | Le nom du producteur des produits que vous souhaitez importer | Four Mile Farm |
| sku | Non | Le code SKU pour ce produit | AD001265 |
| name | Oui | Le nom du produit | Carotte |
| display name | Non | Ce champ s'applique uniquement si vous importez des variantes \(voir plus bas\) | Carotte rouge |
| category | Oui | Les catégories disponibles sont listées sur la page d'import produit | Poisson |
| units | Oui | Le poids, le volume ou la quantité | 500 |
| unit\_type | ? | Sous quelle unité est vendu le produit ? \(grammes, litres,... ?\) S'il est vendu en tant que lot, laissez vide | g |
| variant\_unit\_name | ? | Si le produit est vendu en lot, indiquez le type de lot ici | Botte |
| price | Oui | Le prix du produit TTC | 3.70 |
| on\_hand | ? | Si le stock du produit est limité, indiquez la limite ici, sinon laissez vide et renseingez la colonne on\_demand | 40 |
| available\_on | Non | Laissez vide | ​ |
| on\_demand | ? | Si vous avez un stock infini du produit, indiquez 1 et si vous utilisez la colonne on\_hand laissez vide | 1 |
| shipping\_category | Non | Laissez vide | ​ |
| tax\_category | Oui | Si le prix de votre produit inclus de la TVA, indquez TVA sinon laissez vide | TVA |

### Les variantes {#variants}

​[Variants](https://guide.openfoodnetwork.org/advanced-features/products/product-variants) are distinguished by the units \(such as salad sold in 2 size variants\) and display\_name fields \(such as a yoghurt sold in multiple flavours\) and grouped by product name. The example below shows a salad that comes in 500g and 750g variants, and a yoghurt that comes in multiple flavours.

| name | display\_name | price | units | unit\_type |
| :--- | :--- | :--- | :--- | :--- |
| Salad Bag | ​ | 3.50 | 500 | g |
| Salad Bag | ​ | 5.50 | 750 | g |
| Yoghurt | Banana | 4 | 500 | g |
| Yoghurt | Strawberry | 4 | 500 | g |

Here's how these products will display in the shop:![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LMe5IWuVbnKm1KswdEL%2F-LMe6pI63pK_lVJb5Ans%2Fimage.png?alt=media&token=d46c1309-54cd-4697-8386-b863024d77db)

### Exemple d'unités {#variants-1}

Below are some examples to show how products with different units should be uploaded.

| supplier | **name** | **category** | **price** | **units** | **unit\_type** | **variant\_unit\_name** |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Sue's Salads | Salad Bag | Salads | 3.50 | 500 | g |  |
| Henry Orchards | Fruit Juice | Drinks | 3.50 | 300 | ml |  |
| Fernwell Produce | Potatoes | Vegetables | 9.50 | 5 | kg |  |
| Tom's Bakery | Wholemeal Bread | Baked goods | 3.00 | 1 |  | loaf |

## Mettre à jour des caractéristiques produits existantes {#update-existing-product-details}

The instructions below relate to updating the details of an existing product.

This tool is intended as a quick way to update product prices and stock levels.

The process for updating product details is similar to uploading new products. The first step is to download the **Product List Template** and fill in the product names and the supplier. If you have this spreadsheet on hand from a previous upload even better.

The system requires six fields, which it uses to locate the correct product to update. There are also 6 fields which can be updated. Some fields cannot be updated with the upload tool.

| Required fields \(you can't update\) | Fields you can update | Fields that won't update and aren't required |
| :--- | :--- | :--- |
| supplier | sku | variant\_unit\_name |
| name | display\_name | tax\_category |
| category | price | shipping\_category |
| units | on\_hand | ​ |
| unit\_type \(if applicable\) | on\_demand | ​ |
| variant\_unit\_name \(if applicable\) | ​ | ​ |

The green columns are required, the orange are able to be updated, the white cannot be updated and aren't required.

What if I leave an updateable field blank? Will it become zero/erase the previous content?![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LLDUKuu6UjZDCUMXfpB%2F-LLDUOq-PTriZTyQ5JIA%2Fimage.png?alt=media&token=370263f2-b1cc-4ca4-8b53-4f75fe3f33ac)

## Importer un catalogue {#import-new-inventory}

A compléter

## Mettre à jour un catalogue produit existant {#update-existing-inventory-details}

A compléter

