# Catalogue boutique

## Introduction

La page catalogue permet d'aller plus loin dans la gestion des produits. 

Les 3 avantages principaux de la page :

1. **Ecraser les caractéristiques par défaut du produit**

   Cela peut être intéressant si vous souhaitez modifier les prix pour certains produits par exemple. La page catalogue permet aux entreprises de modifier des détails produits et de les appliquer à leur boutique uniquement. Toutes caractéristique présente en catalogue sera prioritaire aux caractéristiques produits présentent dans le listing produit. Cependant, si d'autres entreprises vendent également ce produit, le changement effectué en catalogue ne changera pas. 

2. **Hiding products and assessing new products.**

    In the inventory list enterprises can hide products that they may not want to see, making the task of filtering which products go into the shopfront quicker when dealing with large amounts of products. There is also the option to have new products added by producers hidden by default, until they have been approved by you.

3. **Resting stock ‘on hand’ levels.** 

   Enterprises who have stock that is regularly  restocked to a certain quantity can define this recurring on hand stock level for each product, and reset levels quickly en mass.

### Permissions Requirements

Enterprises must get the appropriate [E2E permission](../collaborer-avec-dautres-entreprises/e2e-permissions.md) from the supplying producer before they can view an producer’s products in Inventory.

* A hub must have E2E-Inventory \(P-I\) permission from the producer to view their products in Inventory.
* A hubs distributors also needs E2E-Inventory \(P-I\) from the supplying producer if they are to stock the product at according to the hub’s inventory. Without this permission, they will inherit all master product details.

## Your inventory settings

Before using the inventory tool, it’s important to understand your inventory setting, as these will impact on how the inventory lists effects product management.

To view your inventory settings, go to **Manage Enterprise**, and select **Inventory Settings**.

You can select whether new products added by your suppliers need to be added to your inventory before they can be stocked. If you don’t plan to use the inventory tool, select to have any new products able to be added to your shopfront \(recommended\). This way if you create new products for your suppliers, or if your supplier adds products, they’ll immediately be available to be added to your shop. If you are using the inventory page, you may wish to have ‘new’ products withheld from your order cycles until you have chosen to stock them. If this setting applies to you, select the second option below.

![Inventory Settings](https://openfoodnetwork.org/wp-content/uploads/2015/06/Inventory-Settings.png)

## Accessing Inventory

Click on **Products** in the horizontal blue menu and then **Inventory** in the green menu. You will be prompted to select the shopfront that your Inventory will apply to \(if you operate more than one shopfront\). Remember, each shopfront has it’s own Inventory page, and settings in the Inventory page will only be applied to one shopfront. If you have more than one shopfront, you can set different inventory details for each.

![Accessing Inventory](https://openfoodnetwork.org/wp-content/uploads/2015/06/Accessing-Inventory-1.png)

When you first visit the Inventory page, you will see an alert that you have ‘new products available to add to your inventory’. Until you add your products to your Inventory list, they’ll remain in the **New Products** list.

![New products alert](https://openfoodnetwork.org/wp-content/uploads/2015/06/New-products-alert.png)

Clicking on**Review Now**will take you to your**New Products** list.

## New Products

![New Products](https://openfoodnetwork.org/wp-content/uploads/2015/06/New-Products.png)

New products can be either **Added** to your inventory list or **Hidden**. If there is a product in the list for which you would like to override details, or apply a recurring stock level to, you’ll need to **add** it to your inventory list. If there is a product which you never want to sell in your shop, or at least don’t want to stock in the near future, you can choose to **hide** it \(see **Hidden Products** section below\).

Remember, if your **Inventory Settings** are set so that ‘new products must be added to my inventory before they can be put in my shopfront’, any products you leave in the New Product list will effectively be hidden. If your Inventory setting is ‘new products can be put in my shopfront’ then products in your New Products list will still show in your order cycle.

## Inventory Products

![Viewing Inventory Settings](https://openfoodnetwork.org/wp-content/uploads/2015/06/Viewing-Inventory-Settings.png)

Your inventory products list is where you can override product details, set up stock level resetting, and hide products. When you select to view all columns, all of the functionalities of the Inventory List become visible.

![Inheriting product](https://openfoodnetwork.org/wp-content/uploads/2015/06/Columns-1.png)

### Overriding product details

You can change product details in the Inventory Page. Any changes you make will over-ride the master product details, and your shopfront and reports will reflect these over-ridden values you have set. You can override the **SKU**,**Price**,**On Hand** value, and on hand/**on demand** setting. You can’t over-ride the product’s name, units, description or photograph.

* **SKU** 

  – if you wish to use an alternative SKU for a product, you can over-ride the producer’s SKU here by typing in an alternative.

* **Price**

  – You can set a different price to show in your shop. Keep in mind the units of the product will remain the same.

* **On hand**

  – You can set a different on hand value. Your shopfront will stockout when this On Hand value reaches zero.

* **On demand**

  – You can select whether to have a product set to ‘on hand’ or ‘on demand’.

### Stock Level Reset

The **enable stock level reset** column allows you to reset the On Hand amount to a **default amount,** for example at the start of each new order cycle. The **default amount** can be entered in this column next to the check box. The checkbox allows you to select those that you want to reset at any give time. If there is a value in this field and the checkbox is selected, when you hit Inventory &gt; Actions &gt; Reset Stock Levels to Defaults, all the checked products’ on hand values will return to the designated level. As an example this tool is helpful for producers who know that each month they will slaughter 2 animals, and thus have known quantities of product available for each order cycle.

### Inherit

If you have not applied any overrides to a product’s details, the **Inherit** check box will automatically be selected. This tells you that the product’s details will be drawn from the Master product list- these values are shown in grey. When you make an overrides, the check box will un-select, indicating that some product details will be taken from your **Inventory** list, rather than inherited from the **Product** list. If at any point you want to remove your overrides, you can re-select **Inherit** and that product will revert to its master settings.

![Inherited](https://openfoodnetwork.org/wp-content/uploads/2015/06/Inherited.png)

### Hide

As in the **New Products** list, you can also **hide** products from your **Inventory List**. Clicking on the hide button will shift the product to your **Hidden Products** list. This has the effect of making it disappear from your order cycle set up and thus disabling the option of adding it to your shop.

Remember to save changes 

![Save changes](https://openfoodnetwork.org/wp-content/uploads/2015/06/Save-changes.png)

## Hidden Products

![Hidden products](https://openfoodnetwork.org/wp-content/uploads/2015/06/Hidden-products.png)

This list shows any products you have chosen to hide \(this can be done from either the Inventory Product or New Products lists\). A hidden product will longer show up in your order cycle set-up interface, which can make it less cluttered for those with many products. Here you can choose to **+Add** them back to your Inventory Products list. This will make it possible to add them to Order Cycles again and to apply any inventory functions to them.

## Inventory and Order Cycles

In Order Cycle setup, under Advanced Settings, there is the option to control whether incoming inventory reads from the coordinator’s inventory, or from the master products list.

![Advanced OC settings](https://openfoodnetwork.org/wp-content/uploads/2015/06/Advanced-OC-settings.png)

If the ‘**all available products**‘ setting is selected, the incoming inventory will include all products in the master products page. This makes hidden products \(and new\) in inventory available to other distributors in the outgoing section. Note that if the coordinator is a distributor, their outgoing product selection will always be restricted by their inventory pages and settings.

If the ‘**coordinator’s inventory only**‘ setting is selected, the incoming inventory, and thus outgoing inventory to all distributors, will be restricted to the coordinator’s Inventory products. Their hidden products will not be available in the outgoing sections, nor their new products \(if their settings hide new products\). Any overridden detail in the coordinator’s invenotry will not carry through to the distributor’ shops e.g. price.

