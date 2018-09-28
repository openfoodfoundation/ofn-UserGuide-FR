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

​[Les variantes](product-variants.md) peuvent être distinguée par les unitées \(par exemple un produit vendu par 500 g ou 1 kg\) ainsi que le champ display\_name \(exemple : Yaourt à la myrtille, fraise...\). Chaque variante est regroupée sous le même nom produit. Exemple :

| name | display\_name | price | units | unit\_type |
| :--- | :--- | :--- | :--- | :--- |
| Farine de sarasin | ​ | 3.50 | 500 | g |
| Farine de sarasin | ​ | 5.50 | 750 | g |
| Yaourt | Fraise | 4 | 200 | g |
| Yaourt | Myrtille | 4 | 200 | g |

Pour rappel exemple d'affichage pour l'acheteur d'un produit avec 3 variantes :

![](../../.gitbook/assets/image%20%2889%29.png)

### Exemple d'unités {#variants-1}

Un exemple d'import avec des unités différentes :

| supplier | **name** | **category** | **price** | **units** | **unit\_type** | **variant\_unit\_name** |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Producteur A | Patate douce | Légumineuses | 3.50 | 500 | g |  |
| Producteur B | Bar | Poisson | 3.50 | 300 | ml |  |
| Producteur C | Pommes | Fruits & légumes | 9.50 | 5 | kg |  |
| Producteur D | Persil | Herbes & épices | 3.00 | 1 |  | botte |

## Mettre à jour des caractéristiques produits existantes {#update-existing-product-details}

Comment mettre à jour des produits existants ?

Le processus est similaire à la création de produit.  6 champs sont obligatoires pour que l'import fonctionne et seul 5 champs sont modifiables via l'import :

| Champs obligatoires \(non modifiables\) | Champs modifiables | Champs non modifiables et non obligatoires |
| :--- | :--- | :--- |
| supplier | sku | variant\_unit\_name |
| name | display\_name | tax\_category |
| category | price | shipping\_category |
| units | on\_hand | ​ |
| unit\_type \(if applicable\) | on\_demand | ​ |
| variant\_unit\_name \(if applicable\) | ​ | ​ |

## Importer un catalogue {#import-new-inventory}

A compléter

## Mettre à jour un catalogue produit existant {#update-existing-inventory-details}

A compléter

