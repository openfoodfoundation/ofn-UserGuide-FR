# Gestion des tags et comptes clients

Tous les acheteurs ayant passé une commande sur votre boutique se trouvent sur la page **Acheteurs** \(menu principal sur l'interface d'adminsitration\).

Vous pouvez également ajouter manuellement un acheteur via le bouton "nouvel acheteur". Seul les acheteurs dans cette liste peuvent avoir un tag associé.

![](../../.gitbook/assets/image%20%2868%29.png)

## Adresse de facturation et de livraison par défaut

Chaque acheteut peut avoir une adresse de livraison et facturation par défaut. Ainsi le processus d'achat en ligne peut être plus rapide : en effet les champs vont se remplir automatiquement à partir du profil de l'acheteur \(il en va de même pour l'administrateur [s'il créer lui même la commande dans le système](../commandes/manual-orders.md)\).

Si un acheteur change d'adresse, ils peuvent aussi modifier cette adresse par défaut durant la commande en cochant la case "Sauvegarde comme adresse par défaut" :

![](../../.gitbook/assets/image%20%287%29.png)

## Gestion des tags

Un tag vous permet de réaliser les opérations suivantes :

* Rendre certaines variantes disponibles ou indisponibles
* Rendre des méthodes de livraisons disponibles ou indisponibles
* Rendre des méthodes de paiements disponibles ou indisponibles
* Rendre des cycles de vente visibles ou invisibles

Le plus souvent cette fonctionnalité sera utilisée par les entreprises ayant une segmentation de leur acheteurs bien définie \(membres vs non-membres par exemple\).

Utiliser la fonctionnalité se réalise en deux étapes :

1. Taguer un acheteur
2. Paramétrer une règle de tag

### 1. Taguer un acheteur

Pour ajouter un tag, il vous suffit de taper un tag dans la colonne dédiée \(menu **Acheteurs**\). Un acheteur peut avoir plusieurs tags et bien évidemment un tag peut être lié à plusieurs acheteurs. Pour ce deuxième point, la seconde fois où vous taperez le tag dans la colonne correspondante, il vous sera suggéré via une liste déroulante. Faites bien attention à le sélectionner dans cette liste \(les tags sont sensibles à la casse\).

![](../../.gitbook/assets/image%20%2822%29.png)

Notez que les tags apparaissent également dans vos rapports. Vous pouvez donc les utilisez lors des exports excel pour filtrer rapidement les données.

### 2. Paramétrer une règle de tag

Once you have tagged your customers you can define how certain feature will apply to customers with different tags. Currently you can use tags to change four elements:

* Making particular variants available/unavailable
* Making certain shipping methods available/unavailable
* Making certain payment methods available/unavailable
* Making order cycles visible/invisible

To set up your tags go to Edit your Enterprise interface and select **Tag Rules**.

#### Par défaut

By default, all items will be visible to all customers whether they are tagged or not. The general approach is to then create a rule dictating that certain items \(variant, shipping/payment methods or order cycles\) will be invisible to certain customers who are tagged. However, if you wish to change this default, such that tagged items are ‘not visible’ until a rule is setup reversing this, you can do so by changing your ‘By Default’ rules.

The example below shows that my shipping methods tagged ‘wholesale’ will now be invisible by default. If I then wish to make these shipping methods available to customers tagged wholesale I’ll need to set up a Tag Rule below overriding this default.

![Default tags](https://openfoodnetwork.org/wp-content/uploads/2015/10/Default-tags.png)

#### Les règles de tags

Keeping in mind your default setting above, you can now apply rules to vary the default settings for certain customers.

Firstly, you’ll need to select which tag your new tag rule will apply to. To do this type the tag into the ‘for customers tagged:’ field.

Next you can select which condition your rule is based on.

![Rule Types](https://openfoodnetwork.org/wp-content/uploads/2015/10/Rule-Typess.png)

#### **Show or Hide Variants in my shopfront**

This rule lets you make particular variants visible/invisible to tagged customers. For this rule to operate you need to have tagged the customer and the product variant **in your inventory** with the same tag. The screenshot below shows that my 10kg apple variant is tagged ‘wholesale’ in inventory.

![Inventory tagged](https://openfoodnetwork.org/wp-content/uploads/2015/10/Inventory-tagged.png)

* **Invisible:**

   If by default your variants are visible, you can select to make them invisible for customers with a particular tag.

* **Visible:**

   If by default your variants are invisible, you can select to make them visible for customers with a particular tag.

The example below shows that my wholesale variants are invisible by default. A rule has been created so that variants tagged wholesale are made visible just for customers tagged ‘wholesale’.

![Inventory tagged](https://openfoodnetwork.org/wp-content/uploads/2015/10/Inventory-taggedd.png)

#### **Show/Hide shipping methods**

This rule lets you make particular shipping methods specifically available or unavailable to certain customers. For this rule to operate you need to have tagged the customer and the shipping method with the same tag. To tag a shipping method, go to **edit shipping method** and apply the relevant tag. E.g. the shipping method below has been tagged ‘wholesale’.

![Tagging a shipping method](https://openfoodnetwork.org/wp-content/uploads/2015/10/Tagging-a-shipping-method.png)

* **Invisible:**

   If by default your shipping methods are visible, when you set the rule where ‘shipping methods tagged\_are invisible’ shipping methods with the tag will be hidden from customers with a matching tag when they checkout. Untagged shipping methods will still be visible to these customers.

* **Visible:**

  If by default your tagged shipping methods are invisible, you can make them visible to particular customer by setting a ‘shipping methods tagged\_are visible’ tag rule.  Customer without tags or with different tags will still be unable to see this shipping method at checkout.

#### **Show/Hide payment methods**

This rule lets you make particular payment methods specifically available or unavailable to particular customers. For this rule to operate you first need to have tagged the customer and the payment method with the same tag. To tag a shipping method, go to **edit payment method** and apply the relevant tag. E.g. the payment method below has been tagged ‘wholesale’.

![Tagged payment method](https://openfoodnetwork.org/wp-content/uploads/2015/10/Tagged-payment.png)

* **Invisible:**

   If by default your payment methods are visible, when you set the rule where ‘payment methods tagged\_are invisible’ payment methods with the tag will be hidden from customers with a matching tag when they checkout. Untagged payment methods will still be visible to these customers.

* **Visible:**

  If by default your tagged payment methods are invisible, you can make them visible to particular customer by setting a ‘payment methods tagged\_are visible’ tag rule.  Customer without tags or with different tags will still be unable to see this payment method at checkout.

#### **Show/Hide order cycles at my shopfront**

This rule lets you make certain order cycles visible to certain customers only. For this rule to operate you need to have tagged the customer and the order cycle with the same tag. To tag an order cycle, see the Tags tab in the outgoing section of an order cycle \(see below\).

![Tag OC in Outgoing](https://openfoodnetwork.org/wp-content/uploads/2015/10/Outgoing.png)

* **Invisible:**

   If by default your order cycles are visible, when you set the rule where ‘Order cycles tagged\_are invisible’ order cycles with the tag will be hidden from customers with a matching tag. Untagged order cycles will still be visible to these customers.

* **Visible:**

  If by default your order cycles are invisible, you can make them visible to particular customer by setting a ‘order cycles tagged\_are visible’ tag rule.  Customer without tags or with different tags will not see this order cycle.



