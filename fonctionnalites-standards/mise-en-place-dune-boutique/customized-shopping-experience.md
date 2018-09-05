# Gestion des tags et comptes clients

Tous les acheteurs ayant passé une commande sur votre boutique se trouvent sur la page **Acheteurs** \(menu principal sur l'interface d'adminsitration\).

Vous pouvez également ajouter manuellement un acheteur via le bouton "nouvel acheteur". Seul les acheteurs dans cette liste peuvent avoir un tag associé.

![](../../.gitbook/assets/image%20%2877%29.png)

## Adresse de facturation et de livraison par défaut

Chaque acheteur peut avoir une adresse de livraison et facturation par défaut. Ainsi le processus d'achat en ligne peut être plus rapide : en effet les champs vont se remplir automatiquement à partir du profil de l'acheteur \(il en va de même pour l'administrateur [s'il créer lui même la commande dans le système](../commandes/manual-orders.md)\).

Si un acheteur change d'adresse, ils peuvent aussi modifier cette adresse par défaut durant la commande en cochant la case "Sauvegarde comme adresse par défaut" :

![](../../.gitbook/assets/image%20%288%29.png)

## Gestion des tags

Un tag vous permet de réaliser les opérations suivantes :

* Rendre certaines variantes disponibles ou indisponibles
* Rendre des méthodes de livraison disponibles ou indisponibles
* Rendre des méthodes de paiement disponibles ou indisponibles
* Rendre des cycles de vente visibles ou invisibles

Le plus souvent cette fonctionnalité sera utilisée par les entreprises ayant une segmentation de leurs acheteurs bien définie \(membres vs non-membres par exemple\).

Utiliser la fonctionnalité se réalise en deux étapes :

1. Taguer un acheteur
2. Paramétrer une règle de tag

### 1. Taguer un acheteur

Pour ajouter un tag, il vous suffit de taper un tag dans la colonne dédiée \(menu **Acheteurs**\). Un acheteur peut avoir plusieurs tags et bien évidemment un tag peut être lié à plusieurs acheteurs. Pour ce deuxième point, la seconde fois où vous taperez le tag dans la colonne correspondante, il vous sera suggéré via une liste déroulante. Faites bien attention à le sélectionner dans cette liste \(les tags sont sensibles à la casse\).

![](../../.gitbook/assets/image%20%2826%29.png)

Notez que les tags apparaissent également dans vos rapports. Vous pouvez donc les utilisez lors des exports excel pour filtrer rapidement les données.

### 2. Paramétrer une règle de tag

Paramétrer une règle de tag va vous permettre de définir le rôle du tag \(permettre à certaines variantes d'être invisibles pour les membres tagués etc\). Rendez-vous sur le menu **Entreprises** &gt; **Gérer** &gt; R**ègles de tag**

![](../../.gitbook/assets/image%20%2832%29.png)

#### Par défaut

Par défaut, tout est visible pour tout le monde, tagué ou pas. Ajouter un tag va réaliser des exceptions à cette règle. Si vous souhaitez changer la règle par défaut, vous pouvez cliquer sur "Ajouter une règle par défaut". Ainsi les règles ajoutés ensuite, seront des exceptions à cette règle par défaut.

![](../../.gitbook/assets/image%20%286%29.png)

![](../../.gitbook/assets/image%20%2871%29.png)

#### Les règles de tags

Attention, lorsque vous ajoutez une règle par défaut pour les variantes ou les cycles de ventes, il faut que vous taguiez la variante en question avec le même tag. Pour le cycle de vente, le tag s'ajoute dans la partie "sortante".

#### 



