# Cycle de vente pour les hubs

## Cycle de vente pour les hubs

_\*Vous êtes un producteur ? Rendez-vous sur _[_Cycle de vente pour les fournisseurs_](cycle-de-vente-pour-les-fournisseurs.md)_._

En ouvrant un cyclde de vente, vous définissez les périodes d'ouverture de votre boutique, les produits présents ainsi que les marges et commissions associées.

**Pourquoi gérer par cycle de vente ? **Certaines entreprises préfèrent avoir une ouverture en continu et répondre ainsi aux commandes au fil de l'eau. D'autres fonctionnent par périodes. Par exemple, les ventes seront ouvertes pendant deux semaines \(un cycle de vente de deux semaines\) : à la fin de ces deux semaines, toutes les commandes seront emballées et distribuées en même temps. Une fois que ce lot de commandes a été géré, un nouveau cycle de vente redémarre. Cela permet d'optimiser l'emballage et le transport.

### 1. Accéder aux cycles de ventes

Connecté en administrateur, vous pouvez vous rendre sur le menu Cycle de vente ou depuis votre tableau de bord, cliquer sur le bouton suivant :

![](../.gitbook/assets/image%20%2843%29.png)

Puis cliquez sur "Nouveau cycle de vente" :

![](../.gitbook/assets/image%20%287%29.png)

### 2. Créer un nouveau cycle de vente

* **Attention !** Vous ne pouvez pas créer de cycle de vente tant que vous n'avez pas indiqué de [méthode de livraisons ](types-de-livraisons.md)ni de[ méthodes de paiements](methodes-de-paiements.md).

La première chose à faire est de sélectionner un coordinateur pour votre cycle de vente. Cette entreprise aura toutes les permissions pour modifier et gérer le cycle de vente. Les autres entreprises impliquées dans le cycle de vente \(les fournisseurs ou les autres hubs\) auront des accès restreints. Pour plus d'informations sur les gestions des droits entre entreprises, cliquez [ici](../fonctionnalites-avancees/collaborer-avec-dautres-entreprises/e2e-powers-in-multi-enterprise-ocs.md).

![](../.gitbook/assets/image%20%2822%29.png)

**Name:**Give your order cycle a name which is meaningful to you. We recommend that you follow a consistent naming protocol e.g FoodHub\_Week27\_2014. We also recommend that you include the name of your hub in the order cycle name, so that OFN support can identify your order cycles if you need assistance.

**Orders Open:** This is the date at when your OFN store will be open, visible and start to accept orders from customers.

**Order Close: **This is the date when your OFN store will close and stop accepting orders. If you intend to have an order cycle which is continuously open, select a close date which is well into the future.

**Add Coordinator Fee:**As a hub, the coordinator is most likely you. Here you can apply your Enterprise Fee which acts as the markup. The fee will be calculated according to the calculator selected in [Enterprise Fees](frais-et-taxes.md). You can only apply an enterprise fee which has previously been created.

![New order cycle fields](https://openfoodnetwork.org/wp-content/uploads/2015/05/New-order-cycle-3.png)

#### Incoming: select producer and produce

The incoming section is where you can select the producers, and their produce, which will be available in this order cycle. In the dropdown menu you will see all producers who have granted you permission to add their produce to your order cycle \(See _Relationships with Producers_ section for details\). After selecting a supplier and clicking **Add Supplier** all of the products associated with that supplier will be visible. Check those products you wish to add to the store, or click **select all. **Note: Products which have an ‘on hand’ value of zero \(no stock available\) will still be visible, so be careful to check that you have adequate on hand inventory for the products selected.

![Incoming](https://openfoodnetwork.org/wp-content/uploads/2015/05/Incomiing.png)

The **Receival Details **fields are optional. If you wish to use the **Notify Produers**button, to send orders to your supplying producers, you should write your stock receival instructions here. \(more info in the Notify Producers section at the bottom of this page\).

The **Add Fee **button is where you can apply an enterprise fee, belonging to that supplier. Select the name of the enterprise in the first dropdown box, then click the name of the enterprise fee in the second dropdown box. In the example below, an enterprise fee named OrderAdmin is applied to the Producer of Fruit.

This fee will be applied to all of the Producer of Fruit’s products which are purchased. The fee is calculated according to the fee calculator which was selected when the [Enterprise Fee](frais-et-taxes.md) was created.

![Apply enterprise fee to incoming supplier](https://openfoodnetwork.org/wp-content/uploads/2015/05/Enterprise-Fee.png)

#### 4. Outgoing: select distributor

The distributor\(s\) selected in the outgoing section, will have a shopfront created from this order cycle. In simple hub models, there is only one distributor, the hub. So select the hub in the distributor column, and then select all products that should be visible in the online store during this order cycle. More complex hubs might have buying groups, in which case each is selected as a distributor, and will consequently have their own shopfront created. You then have the capacity to select specific products to be available in each buying group’s shop.

![Outgoing Section](https://openfoodnetwork.org/wp-content/uploads/2015/05/Outoging-New.png)

The **tags **column is where you can tag your order cycle \(see [Customer Accounts and Tagging](../fonctionnalites-avancees/mise-en-place-dune-boutique/customized-shopping-experience.md)\).The**‘ready for \(ie Date/Time\)’**box tells the customer when their order will be ready for either collection or delivery. If your order cycle is a perpetual one, which fulfills orders on an individual basis rather then in bulk, you should enter something like ‘Two days after order is received’. The example below shows how ‘Friday 9th’ is displayed in a store.

![ready for field](https://openfoodnetwork.org/wp-content/uploads/2015/05/Ready-for.png)

The note is also shown at check out, when the customer selects their shipping method \(see below\) and is included in the order confirmation email.

![Ready for info in email](https://openfoodnetwork.org/wp-content/uploads/2015/05/shipping-info.png)

The **Pick-Up Instructions **message will be included in the customer’s order confirmation email, below the message that corresponds to their chosen shipping method \(see below\). This note is designed to only be visible to customers, so you can include more sensetive information like addresses, or phone numbers etc. See below for an example of the order confirmation email.

![collection details message](https://openfoodnetwork.org/wp-content/uploads/2015/05/Collection-details.png)

**Add Fee: **Again, a previously created enterprise fee can be assigned to this distributor.

#### 5. Open the shopfront

Click Create to save this order cycle.

![](http://openfoodfoundation.org/sites/default/files/create.png)

.

**\*\* When you create an order cycle, and the opening and closing dates fall either side of the present, a shopfront will become live on the homepage. If you are not ready to have your store open, temporarily put the opening and closing dates in the past \(this can be edited when you are ready to open\).**

For periodic, repetitive order cycles, you can copy an existing order cycle and change the dates, to make the process quicker. See below.

![duplicate an order cycle](https://openfoodnetwork.org/wp-content/uploads/2015/05/copy-order-cycle.png)

Order cycles will display as green when they are active, yellow when schedules for a future date, and grey when they have closed. When an order cycle close over one month ago, it will no longer display on this list. To view all of your past order cycles click ‘show more’ at the top of the list.

**‘Notify Producers’ Button**

Some hubs use this tool as a way to notify their suppliers of which items have been ordered, in what quantities and also to give them receival instructions. Clicking this button will send the following email to the contact email of the producer’s profile. It is sent to all producers included in this order cycle and will sum all of the orders placed in that order cycle.

Dear**&lt;Producer’s Name&gt;**,

We now have all the consumer orders for next food drop.

Stock pickup/delivery instructions: **&lt;Receival instructions&gt;**.

## Orders summary

Here is a summary of the orders for your products:

**&lt;Total products orders in this order cycle \(example below\)&gt;**  
– Producer of Meat – Leg of Lamb \(Frozen\) \(1.5kg\) \(QTY: 1\) @ $22.50 = $22.50  
– Producer of Meat – Sausages \(100g\) \(QTY: 3\) @ $3.00 = $9.00

Thanks and best wishes,

**&lt;Hub Name, address, phone number, email&gt;**

**Advanced Settings**

These settings are relevant for multi distributor order cycles. See [Inventory](../fonctionnalites-avancees/produits/inventory-tool.md) for details of these settings.

**Related advanced features:**

* [Creating ‘display only’ order cycles](../fonctionnalites-avancees/cycles-de-vente/display-only-order-cycles.md)
* [Permissions in multi-enterprise order cycles](../fonctionnalites-avancees/collaborer-avec-dautres-entreprises/e2e-powers-in-multi-enterprise-ocs.md)

