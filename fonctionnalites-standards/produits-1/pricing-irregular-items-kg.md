# Fixer un prix pour les produits au poids irrégulier

Un produit dit "irrégulier" est un produit dont on ne connaît pas le poids final à l'avance \(c'est le cas des pièces de viande par exemple ou morceaux de fromage à la coupe, dont le prix varie en fonction du poids, selon un prix au kg\). Cette section du guide indique différentes façons de saisir et commercialiser ce type de produits.

## Option 1 : Fixer un prix/poids moyen et gérer l'écart à la livraison

Vous pouvez faire payer un prix moyen à l'acheteur et ensuite rembourser la différence ou la facturer, ou ne faire payer le produit qu'à réception pour collecter directement le montant juste.

Lorsque vous connaissez le vrai poids des produits \(à la préparation de la commande ou au moment du retrait du colis par l'acheteur\), connectez-vous au menu "Gestion des commandes par lot" et ajoutez la colonne Poids/volume au tableau de la page. Vous pouvez ainsi modifier le poids indiqué pour chaque acheteur pour une commande donnée et un produit donné. Le prix se recalculera automatiquement en fonction de la quantité saisie. 

![](../../.gitbook/assets/image%20%2882%29.png)

N'oubliez pas de renvoyer une confirmation de commande à l'acheteur pour lui indiquer le bon prix si cela est pertinent, ou de lui indiquer l'écart au moment de la livraison.

## Option 2 : Affichez des fourchettes de prix

Même logique que dans le précédent paragraphe, simplement au lieu d'afficher un prix moyen initialement, indiquez une fourchette de prix. Cette solution à l'avantage de bien préciser à l'acheteur que le prix final est susceptible d'être modifié. Les variantes peuvent également être l'opportunité de créer des fourchettes différentes. 

Exemple 1 : Produit = Poulet \(entre 8 et 12€ selon poids, 10€kg\)   
Exemple 2 : Produit = Poulet \(10€/kg\), Variante 1 = Petit poulet \(entre 8 et 12€ selon poids réel\), Variante 2 = Gros poulet \(entre 13 et 20€ selon poids réel\)

## Option 3 : Créer des variantes par tranche de calibre à prix fixe

Vous pouvez aussi créer des variantes par tranche de calibre, avec un prix fixe pour toutes les unités appartenant à ce calibre par exemple :  
- Courge butternut 600 à 800g = 1,5€  
- Courge butternut 800g à 1kg = 2€  
- Courge butternut 1kg à 1,3kg = 2,5€  
- Courge butternut 1,3kg à 1,6kg = 3€  
- Courge butternut 1,6kg à 2kg = 3,5€

## Option 4 : Créer une variante par poids possible 

Si vous connaissez à l'avance tous les formats possibles, vous pouvez utiliser les variantes pour afficher directement les prix précis pour chaque variante possible. Exemple :

![](../../.gitbook/assets/image%20%2870%29.png)

## Offre irrégulière

Il peut être difficile pour les producteurs de viande de prévoir à l'avance le conditionnement prévu pour ses produits. Les commandes peuvent ainsi être modifiées \(ajout, modification ou suppression de produits\). pour en savoir plus consultez la rubrique [Commandes](../commandes/visualisation-des-commandes.md).

## Remboursement ou refacturation : comment ça marche ?

Lorsque la commande est réglée à réception des produits, le gestionnaire du hub aura pu modifier la commande avant paiement en fonction du poids réel et des produits effectivement livrés, il ne devrait donc pas y avoir de remboursements ou refacturations. 

Lorsque la commande est payée en ligne avant la livraison, il faut alors rembourser ou faire payer l'écart, [Cliquez ici](../commandes/ajustements-de-paiement.md) pour voir comment faire.

Une alternative serait d'utiliser un système de paiement en ligne permettant de stocker temporairement le montant "en attente" jusqu'à validation de la commande, après modifications éventuelles, permettant d'ajuster les montants avant les prélèvements effectifs. Cette fonctionnalité n'est pas encore implémentée dans Open Food Network.

Nous travaillons également à la mise en place automatisée de "crédits" permettant à un hub de rembourser sous forme d'avoirs un trop perçu, utilisable par l'acheteur pour payer en partie sa prochaine commande. 

## Informer l'acheteur sur votre politique de prix

Vous pouvez indiquer à vos acheteurs votre politique de prix, notamment le cas des produits non calibrés comme la viande, en utilisant le message d'accueil de votre boutique, dans les [paramètres](../votre-profil/parametres.md) de votre entreprise.

La description de la [méthode de paiement](../mise-en-place-dune-boutique/methodes-de-paiements.md) peut aussi être un endroit pertinent pour un rappel du type "Souvenez-vous que le prix final peut varier de 10% en fonction du poids effectivement reçu pour les produits à la pièce non calibrés".

