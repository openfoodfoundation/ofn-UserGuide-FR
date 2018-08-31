# Configuration

## 1\) Activez les commandes récurrentes {#1-enable-subscriptions}

Pendant la durée du mode béta, contactez-nous si vous souhaitez utiliser le module pour que nous puissions l'activer sur votre profil.

Activez le module en vous rendant sur les paramètres de votre profil :

![](../../.gitbook/assets/image%20%2876%29.png)

**Abonnements :** Pour activer, sélectionnez "Activée".

**Commandes des invités** : Nous vous recommandons de désactiver cette option afin de ne pas risquer des doublons de commandes.

**Modifier la commande** : 

* Si vous permettez à l'acheteur de modifier la commande il va pouvoir modifier les quantités achetées et retirer des produits. Pour en ajouter, il devra faire une nouvelle commande
* Dans le cas contraire, ils devront vous contacter pour réaliser des modifications. Ils pourront cependant toujours réaliser une nouvelle commande.

## 2\) Vérification des méthodes de paiement et de livraison {#2-make-sure-you-have-shipping-and-payment-methods-setup}

Lorsque vous créez une commande récurrente pour un achteur, il faut que vous indiquez la méthode de paiement et de livraison choisie.

#### **Méthodes de livraison** {#shipping-methods}

Il n'y a pas de restriction sur les méthodes de livraison utilisées. Pour la configuration des méthodes consultez[ la page suivante](../mise-en-place-dune-boutique/types-de-livraisons.md). 

#### **Méthode de paiement** {#payment-methods}

**Vous pouvez utiliser que deux méthodes de paiement pour les commandes récurrentes**. Consultez [cette page](configuration.md#payment-methods) pour la configuration des méthodes de paiement.

**1\) Méthode manuelle** : Espèce ou virement.

**2\) Stripe :** Stripe est un outil de paiement par carte bancaire équivalent à Paypal \(l'obligation de créer un compte pour l'acheteur en moins\). A chaque commande, la carte bancaire va être débitée du montant de la commande \(modifications incluses\), à l'exception faite d'une commande mise en pause ou annulée.

{% hint style="info" %}
Pour que l'acheteur soit correctement débité, il est nécessaire qu'il dispose d'une compte sur la plateforme Open Food France, qu'il ait enregistré une carte de crédit par défaut et donné l'autorisation à votre boutique de réaliser des prélèvements automatiques. Pour plus d'informations consultez la page [Pour l'acheteur](pour-lacheteur.md).
{% endhint %}

Egalement, si vous utilisez Stripe, pensez à bien nommer cette méthode de paiement dans votre interface d'administration.

Par exemple, au lieu de l'appeler "Paiement par carte bancaire", vous pouvez l'appeler "paiement automatique pour commande récurrente". Une description possible à ajouter : "Votre carte de crédit par défaut sera utilisée pour chaque commande récurrente non mise en pause ou annulée".

## 3\) Collectez les informations sur les acheteurs {#3-gather-information-from-your-customers}

Pour créer un abonnement pour vos acheteurs, vous allez avoir besoin de certaines de leurs informations :

**Nom**, **numéro de téléphone** et **adresse e-mail.** Comme précisé dans le paragraphe suivant, tout acheteur souhaitant bénéficier de commandes récurrentes, ont l'obligation de se créer un compte sur OFF. Pour créer leur compte, vous aurez besoin de ces informations.

**Adresse de facturation et de livraison**

**Produits :** pour quels produits souhaitent-ils bénéficier d'une commande récurrente ?

**Méthode de livraison** 

**Méthode de paiement** 

**Dates** la date de début et de fin de la commande récurrente. Pour rappel, les dates de début peuvent être situées avant ou après la date de début du cycle de vente, en revanche les dates de fin doivent obligatoirement se situer après la date de fin du cycle de vente.

## 4\) Ajoutez les nouveaux acheteurs à votre liste {#4-add-your-subscribers-to-your-customer-list}

Avant de démarrer une commande récurrente pour un utilisateur, vous devez l'ajouter à votre liste d'acheteurs. 

**Une fois ajouté à votre liste,** demandez-leur de se créer un compte sur OFF. Toutes les étapes à réaliser de leur côté sont disponibles à la page [Pour l'acheteur](pour-lacheteur.md).

Vous pouvez aussi les ajouter à votre liste une fois leur compte créé. Dans tous les cas, il est nécessaire pour l'acheteur de disposer d'un compte sur la plateforme est de valider son adresse email. Par ailleurs, si vous utilisez Stripe en tant que méthode de paiement, il est nécessaire de les ajouter à votre liste d'acheteurs **AVANT qu'ils autorisent votre boutique à réaliser des prélèvements**.

## 5\) Les rythmes d'abonnement {#5-schedules}

If you are new to OFN we encourage you to get familiar with setting up [order cycles](https://guide.openfoodnetwork.org/advanced-features/order-cycles) before setting up schedules.

### A propos {#about-schedules}

Subscriptions are setup so that every time a shop opens an order cycle, orders are automatically generated for customers who have a subscription with that shop. However, the system has the added flexibility of allowing shops to decide _which_ order cycles the subscription will apply in. This allows shops to have some order cycles which trigger subscription orders to be created, and some which do not.

Which order cycles trigger subscriptions is controlled through an additional element in the Order Cycle setup process, called ‘schedules’. Schedules are groups that order cycle can be assigned to. Once a schedule has been created, customer subscriptions are applied to the schedule, so that an order for their subscription will only be generated for new order cycles in that schedule.

Let’s clarify with some examples:

**Exemple 1**

Harvest Hub runs weekly order cycles. Customers are able to subscribe to either a weekly, or fortnightly order.

In this case there will be two schedules. One that contains all order cycles- the weekly subscribers will have their subscription assigned to this schedule. The second schedule will contain only every second order cycle- the fortnightly subscribers will have their subscription assigned to this schedule.

#### Exemple 2 {#example-2}

Delta Farm runs two order cycle a week, one for a Monday delivery and one for a Thursday delivery.

Most of their customers subscribe to one delivery a week, but some of their hospitality customers subscribe to both the Monday and Thursday delivery.

In this case there will be two schedules, one for the Monday customers and one for the Thursday customers. Those customers who want a subscription on both days can have a subscription applied to both schedules.

### Créer un rythme {#create-a-schedule}

Once you have [enabled the subscription feature](https://guide.openfoodnetwork.org/advanced-features/subscriptions/subscriptions-configuration#1-enable-subscriptions), you will see the Schedule functionality in the order cycle interface. To create a schedule click on the **+ New Schedule** button.![](https://openfoodnetwork.org/wp-content/uploads/2017/02/New-order-cycle.png)

Note: You must have at least one order cycle that can be added to the schedule before you create it.![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-L9rgoFPNHO-1OtFNdJD%2F-L9rgw9U6xoWDx7jf9NH%2FNew%20Schedule?generation=1523500443050782&alt=media)

**Name:** Give the schedule a logical name which describes this group of order cycles. E.g. ‘weekly’, ‘monthly’, ‘Tuesday Deliveries’, ‘wholesale’ or ‘retail’. This name is only visible to you in the backend, not to customers.

You can add existing order cycles into and out of the new schedule by clicking the &lt; and &gt; buttons.

Click **create** when you are finished.

### Modifier ou supprimer un rythme {#edit-or-delete-a-schedule}

To edit or delete a schedule, click on the schedule’s name next to a corresponding order cycle, in the ‘schedules’ column.

Note: This column may need to be made visible in the columns setting dropdown.![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-L9rgoFPNHO-1OtFNdJD%2F-L9rgw9h4IRkrIIfpU8i%2FShow%20Schedules?generation=1523500442468990&alt=media)

You can change the name of the schedule, add/remove order cycles from it or delete the schedule.![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-L9rgoFPNHO-1OtFNdJD%2F-L9rgw9mfT7_QlTdUE33%2FDelete%20Schedule?generation=1523500442452875&alt=media)

> Note: You cannot delete a schedule if there are subscriptions associated with it.

### Ajouter ou supprimer un cycle de vente d'un rythme d'abonnement {#adding-or-removing-order-cycles-from-schedules}

You can add and remove order cycles from schedules by either editing the schedule \(above\), or by editing the order cycle and adding/removing the schedule in the ‘schedules’ field \(below\).![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-L9rgoFPNHO-1OtFNdJD%2F-L9rgw9tiISA0a818ILu%2FOC%20Schedule?generation=1523500443109929&alt=media)

Order cycles may be in more than one schedule. For instance, in the Harvest Hub example above, every second order cycle will be in both the weekly schedule and the fortnightly schedule.

