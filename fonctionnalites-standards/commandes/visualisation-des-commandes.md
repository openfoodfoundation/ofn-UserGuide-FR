# Gestion des commandes

Le menu commandes est divisé en deux sous menu sur Open Food France \(OFF\) : la page "commandes" et la page "gestion des commandes par lot". Cette partie du guide traite des deux pages.

## Listes des commandes

Cette page liste toutes les commandes passées sur la plateforme pour votre compte. A partir de cette page, vous pouvez accéder aux détails de chaque commande, modifier les commandes et suivre leur statut \(du paiement à l'envoi\). Pour consulter la manière de créer une nouvelle commande, cliquez [ici](manual-orders.md).

Les filtres présents sur la page peuvent vous aider à accéder plus rapidement à la commande désirée. Vous pouvez filtrer par date, statut ou via l'email ou le nom du client

![](../../.gitbook/assets/image%20%2833%29.png)

**Distributeur:** L'entreprise à qui appartient la boutique sur laquelle la commande a été passée.

**Sélection de dates** **:** Vous permet de filtrer les commandes par date de création

**Numéro de facture :**  Dans le listing, si un petit panneau apparait avec un point d'exclamation à côté de ce numéro, cela signifie qu'un client a inclut un message avec sa commande. Passez votre souris sur le logo pour afficher la note.

**Région :**

* Valider - le client a terminé son parcours d'achat
* Annuler - cela signifie que l'administrateur a choisi de l'annuler
* Panier - le client a démarré son parcours d'achat mais ne l'a pas finalisé

**Statut du paiement** **:**

* Solde dû - pour tout type de paiement à l'exception de paypal, ce statut s'affiche tant que l'administrateur n'a pas confirmé la bonne réception du paiement
* Payé - Ce statut apparait suite à une commande via paypal ou une action de l'administrateur
* Credit Owed - Si quelqu'un a payé pour sa commande mais que vous modifiez la commande en supprimant un des produits, une dette reste présente.

**Statut de livraison :**

* En attente - Lorsque le statut du paiement est "solde dû", le statut de livraison sera en attente \(tant que le paiement n'est pas reçu, la livraison ne peut pas démarrer\)
* Prêt - Lorsque le paiement est reçu, ce statut s'affiche. 
* Envoyé - Lorsque le produit a été modifié et que son statut à été passé à "envoyé", le statut envoyé s'affiche sur la commande. 

_Remarque_ _: Vous ne pouvez pas indiquer une commande à "envoyée" si le statut de paiement n'est PAS "Payé"._

![](../../.gitbook/assets/image%20%2866%29.png)

**Email acheteur** **:** L'email du client. Une liste complète des emails clients peut être téléchargée dans les [rapports](https://github.com/ofnuserguidefr/guide-utilisateur-open-food-france/tree/f72c4e0a78bb6dc0c5b39249e706b0dbac84df5f/reports.md).

**Total :** La valeur totale de la commande.

### **Modifier le statut de paiement ou de livraison d'une commande**

Sur la colonne de droite, vous pouvez consulter les boutons suivants :

Le bouton lié au paiement :

![paid](https://openfoodnetwork.org/wp-content/uploads/2015/05/Tick.png)

  
Le bouton lié à la livraison :

![Shipped button](https://openfoodnetwork.org/wp-content/uploads/2015/05/Shipped.png)

  
Le bouton de modification générale \(voir paragraphe suivant\) : 

![Edit order button](https://openfoodnetwork.org/wp-content/uploads/2015/05/Edit-order.png)

Pour modifier le statut de livraison ou de paiement, cliquez simplement sur le bouton associé.

### **Modifier une commande**

En cliquant sur le bouton modifier vous êtes amener à consulter la page suivante :

![](../../.gitbook/assets/image%20%2830%29.png)

_Remarque_ _: Vous pouvez également modifier le statut de paiement et de livraison via cette page. Consultez les paragraphes suivants pour les autres fonctionnalités._

#### **Ajouter et supprimer des produits d'une commande**

Vous pouvez ajouter un produit en sélectionnant la bonne variante. Pour le supprimer, il suffit de cliquer sur le petit icône poubelle à côté de la ligne du produit. Vous pouvez aussi modifier les quantités commandées. N'oubliez pas de bien cliquer sur le bouton "**mettre à jour et recalculer les frais"** pour sauvegarder vos modifications.

**Renvoyer l'email de confirmation**

Si vous avez modifié des informations sur une commande, c'est une bonne pratique de renvoyer un email de confirmation ensuite

![](../../.gitbook/assets/image%20%2815%29.png)

**Imprimer la facture**

En cliquant sur cette ligne, la plateforme va générer un PDF, qui vous suffira d'imprimer.

**Envoyer la facture**

Pour envoyer la facture, il suffit de cliquer sur "envoyer la facture" \(menu actions\). Cela enverra un email au client avec la facture correspondante. Exemple de facture générée :

![](../../.gitbook/assets/image%20%2843%29.png)

**Annuler une commande**

Cliquez sur le bouton "annuler" depuis la page de modification d'une commande.

**Détails clients**

Cliquez sur "détails clients" dans la liste en bas à droite pour accéder à toutes les coordonnées :

![](../../.gitbook/assets/image%20%2878%29.png)

**Ajouter ou supprimer un montant à la commande**

Cliquez sur "ajustements" \(cf capture ci-dessus\). Sur cette page vous pouvez ajouter ou supprimer des commissions. Pour ajouter, cliquez sur "nouvel ajustement".

## Gestion des commandes par lot

La liste des commandes présente les commandes alors que cette page liste les produits commandés. Cela permet de modifier en masse plusieurs commandes qui contiennent le même produit \(changement de quantité, produit en rupture, etc\). La page se présente la manière suivante :

![](../../.gitbook/assets/image%20%2870%29.png)

**Date de début et de fin** **:** Vous pouvez filtrer l'affichage des produts en fonction des dates de commandes.

**Producteur :** Vous pouvez filtrer sur un producteur en particulier.

**Boutique** **:** Vous pouvez filtrer sur une boutique en particulier \(comme sur la capture ci-dessus\).

**Cycle de vente** **:** Vous pouvez filtrer sur un cycle de vente en particulier.

**Quick Search :** Sans aller jusqu'à l'utilisation des filtres, vous pouvez aussi tout simplement taper un mot-clé dans ce champ \(cela peut être un nom, un produt, une boutique, un numéro de commande..\).

**Actions :** En cochant les cases à côté de chaque produit, vous pouvez appliquer des modifications en masse en passant par le bouton action \(ex : vous souhaitez supprimer toutes les commandes liées à un produit\).

**Colonnes :** Vous pouvez gérer vous-même l'affichage des colonnes et des champs que vous voyez ou non.

![](../../.gitbook/assets/image%20%2854%29.png)

Notez que vous pouvez également trier chaque colonne en cliquant sur son titre. Un clic pour un ordre de A à Z, un second pour l'ordre inverse.

\*Remarque : La colonne prix indique le prix TTC. Les marges et commission sont recalculées à chaque modification de la commande. 

### Quelques exemples de la gestion de commandes par lot :

#### Exemple 1: Vous avez un problème de stokage de vos fromages de chèvres, il n'est donc pas possible d'en vendre

Vous avez donc besoin d'identifier les clients ayant commandé du fromage de chèvre et modifier leurs commandes.

Les étapes seront les suivantes :

1. Vous filtrez la page gestion des commandes par lot en fonctionde la date ou du cycle de vente en cours
2. Tapez "chèvre" en mot-clé et toutes les commandes avec du fromage de chèvre apparaitront.
3. CLiquez sur "fromage de chèvre" dans la colonne "produit : unité"
4. Un message apparaitra en haut de page avec la quantité totale commandée :

![](../../.gitbook/assets/image%20%2847%29.png)

Vous pouvez alors ajuster la quantité, dans la colonne quantité. Le total affiché au-dessus se modiefiera automatiquement en conséquence. A ce moment, il est intéressant d'envoyer une alerte email aux clients : **la plateforme ne génère pas automatiquement une alerte lors de la modification d'une commande**.

#### **La case à cocher "ressource partagée"**

Cette case à cocher permet d'appliquer les modifications à toutes les variantes des produits. En la laissant décochée vous pouvez modifier variante par variante.

#### Exemple 2: Modifier le poids des produits.

C'est particulièrement vrai lorsque vous vendez de la viande ou certains légumes : vous ne savez pas à l'avance le poids final qui sera vendu avant la commande.

Nous allons prendre l'exemple d'une caisse de viande de 10 kg :

1. Filtrez par date ou cycle de vente
2. Recherchez le produit désiré
3. Rendez les colonnes "Poids/Volume" et "Price" visiblent
4. Modifiez les valeurs de poids \(le prix changera automatiquement\)
5. Cliquez sur "mettre à jour".

![](../../.gitbook/assets/image%20%28102%29.png)



