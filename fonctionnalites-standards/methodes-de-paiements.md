# Méthodes de paiements

Vous devez créer des méthodes de paiements avant de pouvoir ouvrir votre boutique.

## Paramétrer une méthode de paiement

1\) Accéder à la page traitant des méthodes de paiement

Cliquez sur **Entreprises**, puis cliquez sur **Gérer**. Cliquez ensuite sur Méthodes de paiement sur le menu vertical de gauche :

![](../.gitbook/assets/image%20%2812%29.png)

2\) Cliquez sur "**En créer une maintenant**".

3\) Si ce n'est pas le cas sélectionnez votre entreprise dans la liste déroulante des hubs. Cela signifie que la méthode de paiement qui sera créé le sera pour cette entreprise. **Vous pouvez sélectionner plusieurs entreprises**.

![](../.gitbook/assets/image%20%2833%29.png)

4\) **Nom :** Choisissez un nom pour cette méthode de paiement. \(par exemple : "Payez par carte de crédit en utilisant Paypal" etc\). Ce nom s'affichera au moment du paiement pour l'acheteur, ainsi que dans les emails de confirmation qui lui seront envoyés.

5\) **Description :** ajoutez des détails pour la méthode de paiement. Par exemple, pour un virement, vous pouvez indiquez les détails du RIB. Cette description s'affichera au moment du paiement pour l'acheteur, ainsi que dans les emails de confirmation qui lui seront envoyés.

Un exemple de message au moment du paiement :

![](../.gitbook/assets/image%20%2844%29.png)

 6\) **Active :** Indiquez si vous souhaitez que cette méthode soit visible et utilisable

7\) **Tags :** Utilisez les tags si vous souhaitez rendre certaines méthodes de paiements accessible ou non pour certains types d'acheteurs \(voir [la page suivante](../fonctionnalites-avancees/mise-en-place-dune-boutique/customized-shopping-experience.md#customer-tagging) pour l'utilisation de cette fonctionnalité\).

8\) **Fournisseurs** : Sélectionnez celui qui concerne la méthode que vous créez

Vous pouvez accepter les paiements de 5 façons :

* Cash/EFT/etc. \(dans ce cas pas de validation automatique\)
* MasterCard Internet Gateway Service \(MIGS\)
* PayPal Express
* Pin Payments **\(ne fonctionne pas en France\)**
* Stripe

Si vous avez séletionné ‘Cash/EFT/etc..’, cliquez sur **Créer** en base de page.

Pour les autres méthodes, les instructions sont dans les paragraphes ci-dessous.

### PayPal Express

Pour permettre un paiement par Paypal, vous devez avoir un compte Paypal professionnel au préalable. Vous pouvez en créer un [ici](https://www.paypal.com/fr/home). Ensuite il est nécessaire de paramétrer l'API. C'est elle qui vous permettra de connecter votre compte Paypal à Open Food France \(OFF\).

1. Connectez-vous à votre compte Paypal
2. Cliquez sur Tools / Outils puis API credentials / Paramètres :

![Paypal tools API credentials](https://openfoodnetwork.org/wp-content/uploads/2015/05/Paypal-tools-API-credentials.png)

1. Cliquez sur "Voir la signature API" :

![API Access](https://openfoodnetwork.org/wp-content/uploads/2015/05/API-Access.png)

2. Sur OFF, assurez-vous d'être connecté en tant qu'entreprise. Allez dans l'interface d'administration, puis dans le menu Entreprises et créez un méthode de paiement \(voir ci-dessus\). Sélectionnez Paypal et intégrer les informations :



![Api Signature](https://openfoodnetwork.org/wp-content/uploads/2015/05/Api-Signature.png)

**Connexion** **:** Indiquez le nom de l'API "API Username".

**Mot de passe :** Indiquez le mot de passe de l'API  "API Password".

**Signature :** Indiquez le contenu du champ Signature.

![](../.gitbook/assets/image%20%2875%29.png)

**Serveur :** Indiquez " live "sans les guillemets à la place de "sandbox".

**Solution :** Ce champ détermine si les utilisateurs devront avoir un compte paypal pour payer ou non. Laissez "Mark" si l'utilisateur doit avoir un compte paypal, indiquez "Sole" si vous souhaitez le contraire.

**Landing Page :** vous pouvez sélectionner la page d'accueil une fois les utilisateurs redirigez vers paypal pour leur achat. Si vous avez sélectionné "Mark" avant, il vaut mieux indiquer "Login". Si non, "Billing" les renverra directement vers un écran leur permettant d'indiquer leur numéro de carte bleue.

### MasterCard Internet Gateway Service \(MIGS\)

Ce paramétrage ne peut être fait que via votre banque.

### Stripe

[Stripe ](https://stripe.com/au)est une plateforme de paiement en ligne similaire à PayPal. Cette plateforme acceptera les paiements par carte bleue également.

#### Why use Stripe?

Stripe is simple to setup for shop owners, and is reasonably priced. The fees charged by Stripe vary in each country; Australia, USA, Canada, France, UK.

Stripe is also easy for customers to use. Unlike Paypal, when the customer checks out, they don’t need to login with Paypal to place their order, rather they just need to enter their card details and then complete their order.

Stripe is the recommended payment method for shops who wish to use **subscriptions** on OFN, as Stripe allows customers to give permission to a shop to automatically bill their credit card for future subscription orders. This isn’t offered by Paypal, Pin or MIGS payment platforms.

#### Setup

**Connect with Stripe**

Before you can setup a payment method that uses Stripe, you’ll need to Connect with Stripe. To do this, click on the ‘Connect with Stripe’ button.

![Connect with Stripe](https://openfoodnetwork.org/wp-content/uploads/2017/08/Connect-with-Stripe.png)

You’ll be taken to a form to fill in your details. If you already have an account with Stripe, you can login, if not, fill in the form to create a Stripe account.

The information you’ll be asked for includes: country, a description of your business, your Business address and ABN, your personal details and your bank account \(where received payments will be deposited\).

**Create a New Payment Method**

Once you’ve connected with Stripe, you can then create a payment method which will work with your connected account.

Treat the **Name**, **Description**, **Active** and **Tags** fields as you would with any payment method.

**Provider:** Select Stripe.

Once you select Stripe, ‘Provider Settings’ will be shown.

**Stripe Account Owner:**

Select the enterprise that has a Stripe account connected.

If you select an enterprise that is not Connected to Stripe \(see above\), you will get the error shown below. Either click ‘Connect One’ or return to your Payment Methods tab to Connect with Stripe. See instructions above.

![Stripe connect error message](https://openfoodnetwork.org/wp-content/uploads/2017/08/Stripe-connect.png)

#### Stripe Payments for Customers

When customers checkout in a shop and pay with a Stripe payment method, they’ll have the options of selecting a tickbox allowing their credit card details to be stored against their account \(if they are logged in\).

Customer can also save a credit card in their Account, or delete saved ones.

![Add saved credit card](https://openfoodnetwork.org/wp-content/uploads/2017/08/Add-card.png)

When the customer next shops with an OFN shop offering Stripe as a payment method, they’ll be able to select from their saved credit cards.

## Commissions sur les méthodes de paiements

![](../.gitbook/assets/image%20%2873%29.png)

Vous pouvez associer une marge ouune commission à une méthode de paiement. Généralement c'est utilisé pour répercuter les frais des plateformes de paiement à l'acheteur. Sélectionnez un calculateur et indiquez un montant \(voir description ci-dessous\). 

_Remarque : les commissions sur les méthodes de paiement n'incluent pas les taxes._

### Le calculateur

**Pourcentage net** – This fee is charged as a percentage of the total amount charged in the order.

**Taux net \(par commande\)** – Cette marge s'applique de manière standard à toutes les commandes, quelque soit leur taille ou leur unité.

**Taux flexible** – Ce calcul est utilisé pour les remises promotionnelles \(quand vous appliquez une marge réduite lorsque le consommateur achète en gros\).

* ‘Coût du premier item’ : La marge appliquée au premier produit
* ‘Coût d'item additionnel’ : La marge appliquée aux produits suivants
* ‘Nombre maximum d'objets’ : Le nombre maximum d'objets sur lesquels la marge va s'appliquer. Les objets après ce nombre n'auront pas de marge associée.

![](../.gitbook/assets/image%20%286%29.png)

Exemple :  Si la marge du premier est de 2€, celle de l'objet supplémentaire 1 € et le nombre maximum d'objet est de 3. Si un client en commande 5, il paiera 2 € pour le premier, 1€ pour le second et aucune commissions pour les objets 3 et 4.

**Taux net \(par item\)** – Cette marge est constante et s'applique uniquement aux produits vendus à la pièce \(et non ceux vendus au poids\).

**Price Sack** – Cette marge est utilisée pour appliquer une marge réduite à partir du moment où la commande atteind un certain montant.

* ‘Montant minimal’ : Si la commande est en-dessous de ce montant, le consommateur devra payer le ‘Montant normal'.
* ‘Montant de la réduction’ : Si la commande est égale ou supérieure au montant minimal, le consommateur devra payer le ‘Montant de la réduction’.
* 'Currency' : La monnaie utilisée \(généralement "EUR"\).

