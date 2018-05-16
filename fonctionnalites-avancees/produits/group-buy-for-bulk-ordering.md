# Option d'achat par lot

Cette fonctionnalité est à destination des entreprises qui achètent une partie de leur stock par lot. Cette décision dépend souvent de la quantité demandée par l'acheteur final \(est-elle suffisante pour justifier l'achat par lot ?\). Ce choix peut être justifié par des réductions de prix en fonction du volume ou des frais de livraisons \(plus faibles avec des quantités plus grandes\).

Lorsqu'un produit est lié à une fonctionnalité d'achat par lot, la colonne quantité sera affichée différemment dans la boutique. Exemple ci-dessous avec deux produits, seul le premier est lité à la fonctionnalité d'achat par lot :

![](../../.gitbook/assets/image%20%2837%29.png)

Les acheteurs doivent indiquer :

* La quantité minimum qu'ils souhaitent idéalement pour ce produit
* La quantité maximum qu'ils sont prêts à acheter

En gros, cela signifie que l'acheteur final indique le montant maximum qu'il est prêt à acheter afin de bénéficier de réduction lié à l'achat par lot.

Dans le menu de [gestion des commandes par lot](../../fonctionnalites-standards/visualisation-des-commandes.md), vous pouvez observer les quantités minimales et maximales par produits, pour tous les acheteurs. Vous pouvez ainsi décider d'augmenter les commandes jusqu'au seuil maximal ou toutes les supprimer si le minimum de commandes n'est pas atteint.

## Activer l'option d'achat par lot

SUr l'interface d'administration, aller dans le menu Produits, modifiez un produits existants puis rendez-vous sur le sous-menu vertical "option d'achat par lot" :

![](../../.gitbook/assets/image%20%2843%29.png)

Sélectionnez "oui". La quantité totale du lot est le montant minimal que la commande collective doit atteindre **en GRAMMES pour les produits vendus au poids et en LITRES pour les produits vendus au volume.**

## Ajuster les commandes

Dans le menu commandes &gt; gestion des commandes par lot :

1. Sélectionnez le cycle de vente ou les bonnes dates
2. Recherchez votre produit \(dans notre exemple la caisse de viande\)
3. Veillez à bien afficher la colonne **Maximum** pour connaitre le consentement maximal à payer des acheteurs finaux
4. Next, click on Almonds in the Product:Unit column, to display the orders total box. Here I can see the cumulative minimum and maximum orders. In this case, the

   **total quantity ordered**

   is 4kg, which falls short of my bulk order quantity. But the

   **max quantity ordered**

   is 6kg, which shows that some customers are willing to raise their orders.

5. Next, I can look at each customer’s max value, and raise their order

   **Quantity**

   , until the 5kg threshold is reached. Note: any changes to quantity will will be automatically captured in the price column.

6. Sauvegardez vos modifications

![Bulk order management and group buy](https://openfoodnetwork.org/wp-content/uploads/2015/06/BOM-almonds.png)

What does Current Fulfilled Orders and Max Fulfilled Order tell me?

**Current Fulfilled Orders** divides your total quantity ordered by the group buy unit size. If this figure is greater than 1, it tells you that the existing customer order satisfy or exceed your required group buy unit size. If this figure is less than 1, existing customer orders don’t meet that threshold. As you raise the quantity of customer orders, this figure will raise.

**Max Fulfilled Order** takes the sum or all of the customer’s MAX order quantities and divides this by the Group Buy Unit Size. If the number is over 1, then you know that the total of your MAX orders exceeds the required group buy quantity. If it’s below zero, it means that even the MAX order quantities won’t reach the threshold.

### Group Buy Report

The “Bulk Co-op – Totals By Suppliers Report” provides a summary of your bulk products including how many bulk sizes to order, how much remaining stock will be left over and how much extra stock customers are willing to purchase to help the group reach the bulk order size. For details of how to use this report, see the bottom of [this page](https://github.com/ofnuserguidefr/guide-utilisateur-open-food-france/tree/f72c4e0a78bb6dc0c5b39249e706b0dbac84df5f/reports.md).

