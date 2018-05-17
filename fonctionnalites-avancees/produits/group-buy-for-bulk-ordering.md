# Option d'achat par lot

Cette fonctionnalité est à destination des entreprises qui achètent une partie de leur stock par lot. Cette décision dépend souvent de la quantité demandée par l'acheteur final \(est-elle suffisante pour justifier l'achat par lot ?\). Ce choix peut être justifié par des réductions de prix en fonction du volume ou des frais de livraisons \(plus faibles avec des quantités plus grandes\).

Lorsqu'un produit est lié à une fonctionnalité d'achat par lot, la colonne quantité sera affichée différemment dans la boutique. Exemple ci-dessous avec deux produits, seul le premier est lité à la fonctionnalité d'achat par lot :

![](../../.gitbook/assets/image%20%2848%29.png)

Les acheteurs doivent indiquer :

* La quantité minimum qu'ils souhaitent idéalement pour ce produit
* La quantité maximum qu'ils sont prêts à acheter

En gros, cela signifie que l'acheteur final indique le montant maximum qu'il est prêt à acheter afin de bénéficier de réduction lié à l'achat par lot.

Dans le menu de [gestion des commandes par lot](../../fonctionnalites-standards/visualisation-des-commandes.md), vous pouvez observer les quantités minimales et maximales par produits, pour tous les acheteurs. Vous pouvez ainsi décider d'augmenter les commandes jusqu'au seuil maximal ou toutes les supprimer si le minimum de commandes n'est pas atteint.

## Activer l'option d'achat par lot

SUr l'interface d'administration, aller dans le menu Produits, modifiez un produits existants puis rendez-vous sur le sous-menu vertical "option d'achat par lot" :

![](../../.gitbook/assets/image%20%2854%29.png)

Sélectionnez "oui". La quantité totale du lot est le montant minimal que la commande collective doit atteindre **en GRAMMES pour les produits vendus au poids et en LITRES pour les produits vendus au volume.**

## Ajuster les commandes

Dans le menu commandes &gt; gestion des commandes par lot :

1. Sélectionnez le cycle de vente ou les bonnes dates
2. Recherchez votre produit \(dans notre exemple la caisse de viande\)
3. Veillez à bien afficher la colonne **Maximum** pour connaitre le consentement maximal à payer des acheteurs finaux
4. Cliquez sur la valeur de la colonne Produit : unité pour afficher l'encart ci-dessous
5. Grâce à l'information dans la colonne "nombre max d'unité commandées", vous pouvez augmenter le max de chaque commande
6. Sauvegardez vos modifications

![](../../.gitbook/assets/image%20%2879%29.png)



**Nombre d'unité commandées** divise ****le total des quantités commandées par la quantité max des paramètres d'achat par lot. Si le nombre est supérieur à 1, cela signifie que la commande de l'acheteur est équivalente ou supérieure au maximum d'unité de l'option d'achat par lot. A l'inverse, cela signifie que vous pouvez augmenter les quantités. Plus vous augmentez, plus ce nombre augmentera également. 

**Nombre max d'unités commandées** récupère la somme de toutes les quantités maximales pour les acheteurs et divise par la quantité max des paramètres d'achat par lot. SI le nombre est supérieur à 1, vous sacez que le nombre de commande dépasse le seuil maximum. S'il est inférieur à 0 cela signifie que la quantité maximale n'atteindra pas le seuil. 

