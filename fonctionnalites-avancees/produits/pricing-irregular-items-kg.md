# Fixer un prix pour les produits irréguliers au kg

Un produit dit "irrégulier" est un produit dont on ne connait pas le poids final à l'avance \(c'est le cas des pièces de viandes par exemple ou des produits vendus en vrac, dont le prix varie en fonction du poids\). Cette section du guide traite donc la gestion des prix pour ce type de produit.

## Fixer un prix moyen et gérer la différence ensuite

Vous pouvez faire payer un prix moyen à l'acheteur et ensuite rembourser la différence ou la facture

Lorsque vous connaissez le vrai poids des produits, connectez-vous au menu "Gestion des commandes par lot" et ajoutez la colonne Poids/volume au tableau de la page. Vous pouvez ainsi modifier le poids indiqué pour chaque acheteur. Le prix se recalculera automatiquement en fonction de la quantité. 

![](../../.gitbook/assets/image%20%2859%29.png)

N'oubliez pas de renvoyer une confirmation de commande à Claire pour lui indiquer le bon prix.

Pour gérer les remboursements ou les tarifications supplémentaires, rendez-vous dans le chapitre [suivant](pricing-irregular-items-kg.md#reimbursing-or-collecting-additional-payment-on-the-ofn).

## Affichez des fourchettes de prix

Même logique que dans le précédent paragraphe, simplement au lieu d'afficher un prix moyen initialement, indiquez une fourchette de prix. Cette solution à l'avantage de bien préciser à l'acheteur que le prix final est succeptible d'être modifié. Les variantes peuvent également être l'opportunité de créer des fourchettes différentes. 

## Créer une variante par poids possible \(cas des produits congelés\)

Si vous connaissez à l'avance tous les formats possible, vous pouvez utiliser les variantes pour afficher directement les prix précis. Exemple :

![](../../.gitbook/assets/image%20%2851%29.png)

## Offre irrégulière

Il peut être difficile pour les producteurs de viande de prévoir à l'avance le conditionnement prévu pour ses produits. Les commandes peuvent ainsi être modifiées \(ajout, modification ou suppression de produits\). pour en savoir plus consultez la rubrique [Commandes](../../fonctionnalites-standards/visualisation-des-commandes.md).

## Remboursement ou refacturation : comment ça marche ?

Ce cas est très simple à gérer lorsque la méthode de paiement est le liquide à la réception de la commande.

Une alternative reste de faire payer directement en ligne 80% de la commande à l'acheteur et les 20% restant uniquement lorsque vous confirmez la commande. Ces 20% restant pouvant varier en fonction du montant final de la commande. En revanche, la plateforme n'est pas encore automatisée pour ce point. IL faut donc indiquer cette stratégie dans les descriptions à disposition dans la [méthode de paiement](../../fonctionnalites-standards/methodes-de-paiements.md) et être préparé au fait que les acheteurs manqueront peut-être de le lire.

Nous travaillons à la mise en place automatisée de cette partie, qui permettra également l'émission de bons de réductions à la palce de remboursement monétaires.

## Informer l'acheteur sur sa politique de prix

Pour indiquer à l'acheteur final votre politique de prix et notamment le cas des produits en vrac ou de la viande, rendez-vous [ici](../../fonctionnalites-standards/parametres.md#preferences-boutique).

La description de la méthode de paiement est un bon endroit pour réaliser un rappel du type "le prix final peut varier de 10% en fonction des arrivages, nous vous contacterons si la variation du prix peut être plus importantes". Le tutoriel pour placer ce message se trouve [ici](https://github.com/ofnuserguidefr/guide-utilisateur-open-food-france/tree/f72c4e0a78bb6dc0c5b39249e706b0dbac84df5f/payment-methods-2.md).

