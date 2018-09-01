---
description: >-
  Cette page décrit comment une boutique peut créer et gérer des commandes
  récurrentes individuelles.
---

# Création et gestion d'une commande récurrente

**Checklist des points à réaliser avant de réaliser les étapes décrites ici :**

* [Activez les commandes récurrentes dans votre profil](configuration.md#1-enable-subscriptions).​
* Vérifiez les [méthodes de paiement et de livraison](configuration.md#2-make-sure-you-have-shipping-and-payment-methods-setup)​
* [Contacter vos acheteurs pour connaitre leurs préférences et coordonnées](configuration.md#3-gather-information-from-your-customers) et afin qu'ils puissent réaliser [les étapes nécessaires de leur côté​](pour-lacheteur.md)
* [Ajoutez vos acheter à votre liste d'acheteurs](configuration.md#4-add-your-subscribers-to-your-customer-list)
* Créez au moins un [rythme d'abonnement​](configuration.md#create-a-schedule)

## 6\) Créer une commande récurrente {#6-create-subscriptions}

Allez dans le menu général "Commandes" puis cliquez sur le sous-menu vert **Subscriptions**.

![](../../.gitbook/assets/image%20%2818%29.png)

Cliquez ensuite sur "Nouvel abonnement" :

![](../../.gitbook/assets/image%20%2890%29.png)

**Acheteur :** Sélectionnez un acheteur dans la liste déroulante \(seuls les acheteurs présents dans votre liste peuvent être sélectionnés\).

**Rythme d'abonnement :** Sélectionnez le rythme correspondant pour l'acheteur en question.

**Méthode de paiement :** pour rappel seuls stripe et le paiement en espèce sont autorisés.

**Méthode de livraison :** Sélectionnez une méthode de livraison

**Commence à :** Il s'agit de la date de début de la commande récurrente. Elle peut s'appliquer à un cycle de vente en cours comme à un cycle de vente futur.

**Termine à :** Après cette date la commande récurrente ne sera plus générée. Ce champ peut être laissé vide et dans ce cas la commande se génèrera indéfiniment \(mais cela peut être modifié par la suite\).

Si la date de fin de la commande récurrente de l'acheteur se situe après la date de début d'un cycle de vente et avant la date de fin de celui-ci, il n'y aura pas de génération de commande sur ce cycle de vente. La dernière commande ne sera générée que pour le dernier cycle de vente qui ferme avant la fermeture de leur commande récurrente.

**Adresse :** Complétez les coordonnées de votre acheteur \(s'il était déjà connu de la plateforme, les champs seront pré-remplis\).

**Ajouter des produits :** Vous pouvez ajouter des produits de cycle de vente futur, si la date correspond au rythme d'abonnement.

#### Vérifier et enregitrer : reliser le tout et cliquez sur créer un abonnement ou annuler. {#summary}

{% hint style="info" %}
Attention : si vous avez un cycle de vente en cours et assigné à un rythme d'abonnement, dès la création de la commande récurrente, une commande va être générée et l'acheteur recevra un email de confirmation.
{% endhint %}

## 7\) Modifier la commande récurrente d'un acheteur {#7-edit-a-customers-subscription}

### Modifier tout l'abonnement {#edit-the-base-subscription}

Depuis la page **Subscriptions**, cliquez sur le bouton "modifier" à côté de la commande que vous souhaitez modifier.

A partir de là vous pouvez modifier quels produits sont dans l'abonnement, la méthode de livraison ou de paiement, ainsi que les dates de début et de fin. 

**Vous ne pouvez pas modifier le rythme d'abonnement**. Pour cela vous devez recrez une commande récurrente avec unnouveau rythme et supprimer l'ancienne.

### Modifier une commande en particulier {#edit-one-specific-order}

Dans la colonne "commandes", cliquez sur le numéro. Vous accéderez ainsi à la liste de toutes les commandes et vous pourrez en modifier une en particulier.

### Supprimer une commande récurrente {#delete-a-subscription}

Depuis la page **subscription**, cliquez sur la croix à côté de la commande récurrente. Cela supprimera définitivement la commande.

Si vous supprimer une commande alors qu'un cycle de vente toujours ouvert, un message vous avertira afin de vous laisser l'option de garder la commande liée ou de la supprimer également.

### Mettre en pause une commande récurrente {#pause-a-subscription}

From the subscriptions page, click on the **pause** button next to the subscriptions you wish to pause. This will prevent all future orders in the subscription from being generated, until it is activated again. To un-pause a subscriptions, click on the play button.

 If you pause a subscription while an order cycle is still open, you'll be asked whether you'd like to keep the current order or not.

If you un-pause a subscription while an OC is open an order will be generated for this customer if they're subscribed to that schedule.![](https://blobscdn.gitbook.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-L9rgoFPNHO-1OtFNdJD%2F-L9rgzEM-l1yT3rWCm0s%2FPause%20subscription?generation=1523500449629468&alt=media)

## 8\) How subscriptions are processed {#8-how-subscriptions-are-processed}

So once subscriptions are setup, how are they processed each time an order cycle opens and closes?

**1\) An OC within a schedule opens:**

* This triggers the creation of subscription orders for your customers who are subscribed to the schedule.

**BEWARE! The moment you open an order cycle within a schedule, an order will be created for each of your subscribers and they'll be emailed, so make sure you're ready! Double check you've setup your OC correctly and have updated your product availability before you open an order cycle.**

* The stocks level will be deducted accordingly at this time
* Each customer with a subscription order will get an email telling them that their order has been prepared.
* An email will be sent to the shop's notification email summarising how many subscription orders there are, and how many had issues \(e.g. insufficient stock\).
* During the time when the OC is open the customers may be able to edit their order \(depending on your [shop preferences](https://guide.openfoodnetwork.org/basic-features/enterprise-settings#shop-preferences)\)

Note, if you create a subscription while there's an open order cycle in the schedule, an order will be immediately created for that subscriber.

**2\) The OC closes**

* When the Order cycle closes the subscription orders will be confirmed.
* If customers are paying with Stripe, their credit card will be billed at this time
* The customer will receive an email confirming that their order is complete.
* The shop notification email will get an email confirming how many subscription orders were processed. It will also mention any errors - such as a credit card that couldn't be billed.

### Planning for future subscriptions {#planning-for-future-subscriptions}

There's two ways for planning the opening and closing of order cycles in your schedules.

Regardless of which option you use, remember that the frequency that you create order cycles in your schedule will dictate how often the subscription reoccurs. E.g. If you create an order cycle for each week opening on a Monday, your customers will get weekly subscriptions.

**Manual option**

You can create order cycles in your schedule\(s\) on a one by one basis. How this would work is that when you're ready to open and order cycle you'll check that you've updated everything outside of order cycles, such as your product availability, and any shipping method descriptions etc.

Then, you're ready you create the order cycle, either by cloning an existing one or creating a new one. You'll add in the product range and check the text fields of the order cycle \(such as the 'ready for' date\). Also check that you've updated product availability. Then you can create the open order cycle.

**Automatic option**

You can create future order cycles in advance, and set their opening and closing dates to correspond with each subscription date. To do this you can create a series of order cycles through cloning, and adjusting the opening/closing dates, and the text fields \(such as the 'ready for' dates\).

Then, as time passes your order cycles will open and close, triggering the creation and confirmation of your subscriptions.

Just make sure that before the opening date of each order cycle you double check your product availability etc.

