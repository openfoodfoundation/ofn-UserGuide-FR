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

Depuis la page **subscription**, cliquez sur le bouton pause. Cela stopera les commandes récurrentes jusqu'à ce que vous cliquiez sur le bouton play \(qui a remplacé le bouton pause une fois que vous avez cliqué dessus\).

Si vous mettez en pause une commande alors qu'un cycle de vente est toujours ouvert, un message vous avertira afin de vous laisser l'option de garder la commande liée ou de la mettre en pause également. Et inversement si vous relancer la commande récurrente alors qu'un cycle de vente est ouvert.

## 8\) Comment sont gérées les commandes récurrentes ? {#8-how-subscriptions-are-processed}

Une fois la mise en place effectuée, que se passe-t-il ?

**1\) Un cycle de vente compatible avec un rythme d'abonnement est ouvert :**

* Une commande est générées pour tous les acheteurs liés à ce rythme d'abonnement. Un email de confirmation de la commande leur est adressé.
* Le stock des produits commandés va diminuer
* Un email résumant toutes les commandes passés ainsi que celle qui on eu des problème \(stock insuffisant\) est envoyé au responsable de la boutique en ligne
* Les acheteurs peuvent modifier leur commande si vous leur en avez laissé la possibilité dan vos [paramètres de boutique](../votre-profil/parametres.md#preferences-boutique).

**2\) Un cycle de vente ferme**

* Les commandes seront confirmées
* Si l'acheteur paye par carte de crédit il sera débité
* L'acheteur reçoit un email de confirmation
* Le responsable de la boutique reçoit un email récapitulatif des commandes et des erreurs qui ont pu avoir lieu comme par exemple des carte de crédit qui n'ont pas pu être débtées

### Plannier les commandes récurrentes {#planning-for-future-subscriptions}

Il y a deux manières de plannifier les commandes récurrentes. Quelque soit celle choisie n'oubliez pas que la fréquence à laquelle vous ouvrez un nouveau cycle de vente avec commande récurrente correspondra à la fréquence à laquelle les commandes seront générées.

**De manière manuelle**

Vous pouvez créer des commandes par rythme d'abonnement une à une en ouvrant un cycle de vente à chaque besoin.

**De manière automatique**

Vous pouvez créer vos cycles de vente en avance et faire correspondre les dates à chaque date de commande. Vous pouvez utiliser la fonction de clonage d'un cycle de vente pour aller plus vite.

Pensez cependant à vérifier les stocks de vos produits régulièrement pour qu'il n'y ait pas de problème de disponibilité.

