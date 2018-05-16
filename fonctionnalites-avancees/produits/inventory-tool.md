# Catalogue boutique

## Introduction

La page catalogue permet d'aller plus loin dans la gestion des produits. 

Les 3 avantages principaux de la page :

1. **Ecraser les caractéristiques par défaut du produit**

   Cela peut être intéressant si vous souhaitez modifier les prix pour certains produits par exemple. La page catalogue permet aux entreprises de modifier des détails produits et de les appliquer à leur boutique uniquement. Toutes caractéristique présente en catalogue sera prioritaire aux caractéristiques produits présentent dans le listing produit. Cependant, si d'autres entreprises vendent également ce produit, le changement effectué en catalogue ne changera pas. 

2. **Masquer des produits.**

   La page catalogue permet de masquer des produits, soit volontairement soit par défaut de considérer qu'ils ne sont pas visible tant que le hub ne les a pas approuvé.

3. **Gérer les stocks "à volonté" pour chaque produit et en masse.** 

   C'est idéal pour tous les produits dont le stock se renouvelle rapidement et régulièrement.

### Permissions nécessaires

Les entreprises doivent obtenir les bonnes [permissions inter-entreprises](../collaborer-avec-dautres-entreprises/e2e-permissions.md) de la part de leurs fournisseurs avant de pouvoir voir les catalogues produits des fournisseurs sur cette page.

## 1\) Les paramètres de votre catalogue

Pour y accéder, rendez-vous sur **Entreprises**, puis "**gérer**" et enfin "**Catalogue boutique**" dans le menu vertical de gauche :

![](../../.gitbook/assets/image%20%2841%29.png)

Vous avez deux options : soit vous choisissez l'option selon laquelle les nouveaux produits ajoutés par vos fournisseurs doivent être préalablement ajoutés à votre catalogue \(de cette manière vous pourrez choisir de les ajouter ou non à vos cycles de vente en cours\), soit - si vous ne pensez pas utiliser le catalogue - sélectionnez l'option recommandée. Les produits ajoutés par les fournisseurs seront ainsi ajoutés directement à votre boutique en ligne.

## 2\) Accéder au catalogue boutique

Cliquez sur le menu **Produits** dans l'interface d'administration, puis sur **Catalogue** **boutique** dans le sous menu vert. SI vous gérer plusieurs boutiques, il vous sera demandé d'en sélectionner une car chaque catalogue est géré indépendemment.

![](../../.gitbook/assets/image%20%2824%29.png)

Lors de votre première visite, un message vous alertera sur le fait que vous avez de nouveaux produits disponible à l'ajout dans votre catalogue. Tant que ce ne sera pas fait, il resteront dans la catégorie "**Nouveau produits**".

![](../../.gitbook/assets/image%20%2812%29.png)

En cliquant sur "**vérifier maintenant**" vous serez redirigé vers la liste des **nouveaux produits**.

## Nouveaux produits

![](../../.gitbook/assets/image%20%2816%29.png)

Les nouveaux produis peuvent être soit **ajoutés** à votre catalogue, soit **masqués**. Si vous souhaitez écraser les caractéristiques d'un produit de la liste ou indiquer le niveau du stock, vous devrez l'ajouter à votre catalogue. S'il s'agit d'un produit que vous ne voudrez jamais vendre dans votre boutique ou en tout cas pas à court terme, vous pouvez choisir de le masquer.

Pour rappel, si l'option choisie dans les [paramètres](inventory-tool.md#1-les-parametres-de-votre-catalogue) est l'option selon laquelle les produits doivent être ajoutés à votre catalogue pour apparaitre sur le boutique en ligne, tous les produits que vous laissés dans la liste "nouveaux produits" seront par défaut masqués, c'est-à-dire absent de la boutique en ligne. Dans l'autre cas ils apparaitront automatiquement dans le cycle de vente en cours. 

Poursuivez la lecture pour comprendre le traitement manuel du masquage et de l'ajout.

## Produits du Catalogue Boutique

![](../../.gitbook/assets/image%20%2849%29.png)

Via le bouton colonnes, si vous affichez toutes les colonnes, toutes les fonctionnalités du catalogue s'afficheront à vous.

![](../../.gitbook/assets/image%20%2838%29.png)

### Ecraser des caractéristiques produits

Vous pouvez modifier les caractéristiques produits sur cette page. Toutes les modifications que vous ferez ici seront visibles sur votre boutique. Vous pouvez modifier les champs suivants \(mais pas les autres, c'est-à-dire le nom du produits, les conditionnements, ou encore la description ou l'image\) :

* **Référence produit**

  – vous pouvez ici indiquer une autre référence produit que celle du producteur

* **Prix**

  – Le prix est modifiable mais n'oubliez pas que les quantités unitaires associées ne le sont pas

* **En stock**

  – Vos produits ne seront plus visibles une fois que cette valeur atteint zéro \(tous les quantités indiquées ont été vendues\)

* **A volonté**

  – Vous pouvez sélectionner si le produit est vendu à la demande ou suivant un stock défini

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

