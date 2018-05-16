# Cycle de vente pour les hubs

## Cycle de vente pour les hubs

_\*Vous êtes un producteur ? Rendez-vous sur_ [_Cycle de vente pour les fournisseurs_](cycle-de-vente-pour-les-fournisseurs.md)_._

En ouvrant un cyclde de vente, vous définissez les périodes d'ouverture de votre boutique, les produits présents ainsi que les marges et commissions associées.

**Pourquoi gérer par cycle de vente ?** Certaines entreprises préfèrent avoir une ouverture en continu et répondre ainsi aux commandes au fil de l'eau. D'autres fonctionnent par périodes. Par exemple, les ventes seront ouvertes pendant deux semaines \(un cycle de vente de deux semaines\) : à la fin de ces deux semaines, toutes les commandes seront emballées et distribuées en même temps. Une fois que ce lot de commandes a été géré, un nouveau cycle de vente redémarre. Cela permet d'optimiser l'emballage et le transport.

### 1. Accéder aux cycles de ventes

Connecté en administrateur, vous pouvez vous rendre sur le menu Cycle de vente ou depuis votre tableau de bord, cliquer sur le bouton suivant :

![](../.gitbook/assets/image%20%2866%29.png)

Puis cliquez sur "Nouveau cycle de vente" :

![](../.gitbook/assets/image%20%289%29.png)

### 2. Créer un nouveau cycle de vente

* **Attention !** Vous ne pouvez pas créer de cycle de vente tant que vous n'avez pas indiqué de [méthode de livraisons ](types-de-livraisons.md)ni de[ méthodes de paiements](methodes-de-paiements.md).

La première chose à faire est de sélectionner un coordinateur pour votre cycle de vente. Cette entreprise aura toutes les permissions pour modifier et gérer le cycle de vente. Les autres entreprises impliquées dans le cycle de vente \(les fournisseurs ou les autres hubs\) auront des accès restreints. Pour plus d'informations sur les gestions des droits entre entreprises, cliquez [ici](../fonctionnalites-avancees/collaborer-avec-dautres-entreprises/e2e-powers-in-multi-enterprise-ocs.md).

![](../.gitbook/assets/image%20%2831%29.png)

**Nom :** Choississez un nom pou le cycle. Il sera visible uniquement pour vous, donc indiquez quelque chose qui vous permettra de le retrouver facilement ensuite. Par exemple vous pouvez choisir un protocole du type _Commandesemaine26\_2018._

**Commandes à partir de :** La date à laquelle votre boutique commencera à accepter des commandes.

**Orders Close :** La date à laquelle la boutique arrêtera d'accepter des commandes. Si vous souhaitez laisser votre boutique ouverte en continue, indiquer une date dans un futur très lointain.

**Ajouter commission coordinateur :** En tant que Hub, le coordinateur est certainement vous. La marge sera calculée en fonction du calculateur sélectionné précédemment, voir guide [Marges et commissions](frais-et-taxes.md).

### 3. Produits entrants

Ici vous pouvez sélectionner les producteurs et les produits qui seront accessibles durant le cycle de vente. Les producteurs visibles dans la liste déroulante sont uniquement les producteurs vous [ayant donné accès à leur catalogue](../fonctionnalites-avancees/collaborer-avec-dautres-entreprises/). Cliquez bien sur "ajouter un fournisseur" pour voir les produits associés à ce fournisseur. Cohez les produits que vous souahitez ajouter \(vous pouvez aussi les sélectionner tous\). **Attention** : les produits qui on une valeur "à volonté" à 0 s'afficheront également. Faites bien attention au stock disponible en les ajoutant. 

Les **détails de livraison produits Details** sont facultatifs. 

Le bouton pour ajouter une marge ou commission vous permet de l'ajouter par fournisseur. Sélectionnez le nom de l'entreprise, puis le nom de la marge comme dans l'exemple ci-dessous. 

Cette marge s'appliquera à tous les produits du fournisseur.La marge sera calculée en fonction du calculateur sélectionné précédemment, voir guide [Marges et commissions](frais-et-taxes.md).

![Apply enterprise fee to incoming supplier](https://openfoodnetwork.org/wp-content/uploads/2015/05/Enterprise-Fee.png)

### 4. Produits sortants

Le distributeur sélectionné dans cette catégorie aura une boutique ouverte avec ce cycle de vente. Dans un modèle simple, il n'y a qu'un seul distributeur, le hub. IL suffit de le sélectionner puis de sélectionner tous les produits associés. Dans un modèle plus complexe avec plusieurs hubs, vous avez ainsi la possibilité de sélectionner des produits différent pour chaque hub. 

Les **tags** vous permettent de taguer le cycle de vente \(voir [Gestion des tags et comptes clients](../fonctionnalites-avancees/mise-en-place-dune-boutique/customized-shopping-experience.md)\).

**Le message lié aux instructions de réception de la commande** sera inclut dans l'email de confirmation de commande envoyé au client, jsute en-dessous de la méthode de livraison. Ils seront les seuls à obtenir cette information donc vous pouvez y inclure des informations comme des adresses ou numéros de téléphone.

**Ajouter une marge** **:** A nouveau une marge peut être associée au hub.

### 5. Ouvrir la boutique

Cliquez sur "créer" pour créer le cycle de vente.

\*Remarque : lorsque vous créez un cycle de vente, si une des deux dates indiquées se situe dans le moment présent, la boutique sera automatiquement ouverte sur la plateforme. Si vous n'êtes pas prêt à ouvrir tout de suite, indiquez des dates dans le passé, que vous pourrez changer ensuite. 

Si votre cycle de vente se répête de manière périodique et régulière, vous pouvez duppliquer un cycle de vente passé afin d'aller plus vite \(bouton orange sur la capture, attention il n'est pas orange sur la plateforme\) :

![](../.gitbook/assets/image%20%2819%29.png)

Les cycles de vente sont présentés en vert lorsqu'ils sont actifs, jaune lorsqu'ils sont indiqués pour une date dans le futur et gris lorsqu'ils sont fermés. Un mois après la fermeture d'un cycle de vente, il n'apparaitra plus dans cette liste, il faudra cliquer sur "voir plus" pour voir tous vos cycles de vente.

## **Notifier les producteurs**

En utilisant ce bouton, tous les producteurs liés à ce cycle de vente seront notifiés d'un email contenant une liste des produits commandés pour ce cycle de vente.

## **Fonctionnalités avancées**

Ces fonctionnalités sont à destination descycles de vente avec plusieurs hubs. Rendez-vous sur la page [Catalogue](../fonctionnalites-avancees/produits/inventory-tool.md) pour plus de détails.

* [Créer des cycles de vente en affichage seul](../fonctionnalites-avancees/cycles-de-vente/display-only-order-cycles.md)
* [Gestions des droits pour les cycles de vente à plusieurs entreprises](../fonctionnalites-avancees/collaborer-avec-dautres-entreprises/e2e-powers-in-multi-enterprise-ocs.md)



