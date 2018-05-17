# Permissions inter-entreprises

## Permissions inter-entreprises

Ce sont des permissions nécessaires avant qu'une entreprise deviennent fournisseur d'une autre ou inversement qu'une entreprise ne puisse distribuer les produits d'une autre.

Cette page détaille les différentes permissions possibles et la manière de les allouer. Ensuite deux paragraphes vont plus loin en présentant les permissions depuis deux points de vue différents :

* [**Celui du hub**](e2e-permissions.md#E2Es-from-a-hubs-perspective)
* [**Celui du producteur**](e2e-permissions.md#E2Es-from-a-producers-perspective)

### Les différentes permissions

Il existe 4 différentes permissions. Elles peuvent se combiner de différentes manières afin de donner aux entreprises plus ou moins de droits suivant leurs profils. 

**Permission d'ajouter un cycle de vente**

Le fournisseur permet au hub d'ajouter ses produits à leurs cycle de vente

**Permission d'ajouter un catalogue boutique**

Le fournisseur permet au hub d'ajouter ses produits au catalogue boutique du hub.

**Permission de gérer les produits**

Le fournisseur permet à une entreprise \(hub ou producteur\) de créer, supprimer et modifier ses produits en ligne.

**Permission de modifier le profil**

Une entreprise permet à une autre de modifier ses détails de profils \(coordonnées, adresse, description, ...\)

### Donner et gérer les permissions {#grantingandmanagingE2Es}

Pour modifier, ajouter ou supprimer des permissions, rendez-vous sur l'interface d'administration puis dans le menu **Entreprises**, puis sous-menu **Permissions inter-entreprises** \(voir capture ci-dessous\).

Si vous avez besoin qu'une autre entreprise vous donne des permissions, vous devez les contacter par email ou téléphone. Il n'y a pas de fonctionnalité en ligne pour contacter une autre entreprise à ce sujet.

**Attention** : vous ne pouvez pas gérer les permissions de votre entreprises si vous n'êtes pas administrateur ou manager du profil de votre entreprise.

**Donner une permission**

Dans la première colonne, sélectionner votre entreprise et dans la seconde l'entreprise à qui vous donnez des droits. Cliquez ensuite sur le type de permissions que vous souhaitez ajouter. Vous pouvez sélectionner plusieurs permissions ou les sléectionner toutes en cliquant sur "TOUT".

Puis cliquez sur "Créer". Notez que vous pouvez supprimer ou modifier ces permissions à tout moment.

![](../../.gitbook/assets/image%20%2872%29.png)

### Les permissions générées automatiquement

Lorsqu'un utilisateur administre plusieurs entreprises sur la plateforme, les permissions sont créées automatiquement entre chaque entreprises. 

Ce n'est pas le cas entre des entreprises administrées par des utilisateurs différents.

## E2Es from a hub’s perspective

The following scenarios demonstrate the E2Es structures required in different circumstances.

#### 1\) I have created profiles for my supplying producers, what E2Es do I need before I can stock their products in my shop?

The system is configured so that hubs creating producer profiles will have the correct permissions installed as default, so that they can start adding products and trading with these producer profiles right away.

If a user owns a hub enterprise, and then creates a producer enterprise, automatically the new producer will grant the hub P-OC and P-I.

Similarly, if a users owns a producer enterprise, and then creates a hub, the producer will automatically grant the hub P-OC and P-I.

_Do you distribute through buying groups? If so make sure to check out the E2E requirements for buying groups below._

#### 2\) I want to stock the products of a producer who is already on the OFN in my shop, what E2Es do I need?

To start stocking the products of a producer who is already on the OFN, you must get the following E2E permissions from them.

* At a minimum, to stock a producer’s products in your store, you’ll need P-OC to add them to your order cycles.
* If you wish to modify the producer’s price or stock level, you’ll need them to grant you P-I.
* If you, or the producer want you to be able to manage \(add, edit, delete\) the producer’s products, you’ll need the producer to grant you P-P
* If the producer is happy for you to have permission to edit their profile, they can also grant you P-OC.

_Do you distribute through buying groups? If so make sure to check out the E2E requirements for buying groups below._

#### 3\) My hub distributes through buying groups, what E2Es will the buying group need with my hub, and my producers?

For a hub to designate a buying group as a distributor in an order cycle, they must have P-OC from that buying group enterprise.

* If the user who owns the hub also owns the buying group, P-OC will automatically be granted to the hub.
* If the hub and buying group are owned by different users, the buying group owner will need to grant P-OC to the hub, so that they can act as a distributor.

Further, buying groups must have P-OC from all producers, of any products that will be distributed through the buying group.

* If the user who owns the producers also owns the buying group, P-OC will automatically be granted to the buying group.
* If the producers and buying group are owned by different users, the producer owner will need to manually grant P-OC to the buying group, allowing them to distribute their products.

## E2Es from a producers perspective

When a producer wants to start selling their products through other enterprises \(hubs or buying groups\) the must establish the appropriate E2E permissions. There are different levels of permission that a producer can grant, depending on how much power they want to give the hub to manage their products and profile \(see top of page\).

Use the following examples to explore your options.

#### 1\) I’m a producer and I stock my products through a hub. What E2Es do I need? What are my options?

* Essential- For the hub to add your products to their shopfront, you’ll need to grant them P-OC. This allows the hub to stock your existing products.
* Optional- In addition to P-OC, you might also want to give the hub permission to manage your products \(P-P\), to edit your profile \(P-Profile\) or to add to

  [Inventory ](../produits/inventory-tool.md)

  \(P-I\).

#### 2\) A hub that I supply to distributes through buying groups, do I need to give them permission?

* Yes, if a hub you supply distributes products through buying groups, or other hubs, you’ll also need to grant them P-OC. Otherwise they won’t be able to stock your products in their unique buying group shopfronts. Again you can choose to also grant these buying groups P-P, P-Profile or P-I if you wish.

#### 3\) I run my own shopfront and also stock through a hub. The hub wants me to give them P-P so they can change my stock levels and product prices. But this will impact on how I run my shop. What should I do?

The scenario described can be solved by granting P-I \([**Add to Inventory**](../produits/inventory-tool.md)\). This allows the hub to stock your products in their shop, but to set their own prices and inventory levels. When you stock your own shop with your products, they will continue to reflect the prices and stock levels that you have set.



