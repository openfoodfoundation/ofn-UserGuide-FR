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

The product and inventory import tool lets you upload a csv file to add and update your stock.

The product and inventory import tool can be found by clicking **Products** in the horizontal blue menu, and **product import** in the green menu.

Product import can be used in relation to [products](https://guide.openfoodnetwork.org/basic-features/products) and [inventory](https://guide.openfoodnetwork.org/advanced-features/products/inventory-tool). There's four ways you can use the tool:

1. Import new products
2. Update existing product details
3. Import new inventory
4. Update existing inventory details

In all cases the process involves downloading a csv template, filling in the fields and then uploading your csv file back into OFN.

## Import New Products {#import-new-products}

Use these instructions if you want to add new products to a producer's profile.

Firstly, download the **Product List Template CSV** file from the **Product Import** page and open it with excel \(or equivalent\)

You'll see that the template gives all the column headings required to successfully import a product. Below is a description of how to fill in each column.![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LLD9YyGAvDINJ-BEyZX%2F-LLCqGAxgK4IgQvi7juD%2Fimage.png?alt=media&token=4debaf15-9927-4df4-8cff-ff75b28d215a)

Note that all fields are case sensitive. E.g. you must use mL not ml , or Dairy not dairy.

| Column Title | Required? | Description | Example |
| :--- | :--- | :--- | :--- |
| supplier | Y | This is the name of the producer profile that this product will be assigned to | Four Mile Farm |
| sku | N | The SKU code for this product | AD001265 |
| name | Y | This is the name of the product | Yoghurt |
| display name | N | This field applies if you are creating variants \(see instructions below\). If you're not creating a variant leave this field blank. | Rasberry Yoghurt |
| category | Y | Which category does this product sit in? The categories available are listed on the Product Import page | Dairy |
| units | Y | The weight, volume or quantity value | 500 |
| unit\_type | Maybe | What unit is it sold in \(g, kg, T, mL, L\)? If sold as an item \(e.g. bunch\) leave blank | g |
| variant\_unit\_name | Maybe | If the product is sold as an item \(e.g loaf, bunch, pumpkin\) write the item type here | Bunch |
| price | Y | The price of the product. If the item carries tax, this must be the tax inclusive price. | 3.70 |
| on\_hand | Maybe | If you have limited stock for the product type the stock level here. If you have infinite stock available \(you can always source it\) leave this field blank and use the on\_demand column | 40 |
| available\_on | N | Leave blank | ​ |
| on\_demand | Maybe | If you have infinite stock available for this product, type 1, if you're using on\_hand leave blank | 1 |
| shipping\_category | N | Leave blank | ​ |
| tax\_category | Y | If the price of your product includes tax type GST, if not leave blank | GST |

### Variants {#variants}

​[Variants](https://guide.openfoodnetwork.org/advanced-features/products/product-variants) are distinguished by the units \(such as salad sold in 2 size variants\) and display\_name fields \(such as a yoghurt sold in multiple flavours\) and grouped by product name. The example below shows a salad that comes in 500g and 750g variants, and a yoghurt that comes in multiple flavours.

| name | display\_name | price | units | unit\_type |
| :--- | :--- | :--- | :--- | :--- |
| Salad Bag | ​ | 3.50 | 500 | g |
| Salad Bag | ​ | 5.50 | 750 | g |
| Yoghurt | Banana | 4 | 500 | g |
| Yoghurt | Strawberry | 4 | 500 | g |

Here's how these products will display in the shop:![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LMe5IWuVbnKm1KswdEL%2F-LMe6pI63pK_lVJb5Ans%2Fimage.png?alt=media&token=d46c1309-54cd-4697-8386-b863024d77db)

### Unit type examples {#variants-1}

Below are some examples to show how products with different units should be uploaded.

| supplier | **name** | **category** | **price** | **units** | **unit\_type** | **variant\_unit\_name** |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Sue's Salads | Salad Bag | Salads | 3.50 | 500 | g |  |
| Henry Orchards | Fruit Juice | Drinks | 3.50 | 300 | ml |  |
| Fernwell Produce | Potatoes | Vegetables | 9.50 | 5 | kg |  |
| Tom's Bakery | Wholemeal Bread | Baked goods | 3.00 | 1 |  | loaf |

## Update Existing Product Details {#update-existing-product-details}

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

## Import New Inventory {#import-new-inventory}

Coming soon

## Update Existing Inventory Details {#update-existing-inventory-details}

Coming soon

