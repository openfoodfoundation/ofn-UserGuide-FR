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

8\) **Payment providers**: Select the one which is relevant to the payment method you are creating.

You can accept payment via 5 payment options:

* Cash/EFT/etc. \(Use this for payments which occur after checkout, externally to OFN such as cash or bank transfers\)
* MasterCard Internet Gateway Service \(MIGS\)
* PayPal Express
* [Pin Payments](https://pin.net.au/)
* Stripe

If you have selected ‘Cash/EFT/etc..’ as the provider, click **Create** to end the process.

For MasterCard, Paypal and Pin Payments additional instructions are below.

### PayPal

%accordion%Paypal%accordion%

To setup a PayPal payment method, you need a PayPal business or merchant account. You can create one [here](https://www.paypal.com/au/webapps/mpp/merchant). Once you have that, you can set up ‘API access’ within PayPal, which will enable OFN to connect customers directly with your PayPal account.

1. Login to your PayPal Account
2. Click Tools and then select API credentials

![Paypal tools API credentials](https://openfoodnetwork.org/wp-content/uploads/2015/05/Paypal-tools-API-credentials.png)

1. Click on ‘View API Signature’  and you will see the API details you’ll need to set up Paypal in OFN.

![API Access](https://openfoodnetwork.org/wp-content/uploads/2015/05/API-Access.png)

![Api Signature](https://openfoodnetwork.org/wp-content/uploads/2015/05/Api-Signature.png)

1. In OFN, make sure you are logged in as your Enterprise User. Go to an Enterprise and create a Payment Method. Select PayPal and fill in the details from the PayPal site.

**Login:**Type the API Username.

**Password:**Type the API Password.

**Signature:**Type the Signature in this field.

![New Payment Paypal](https://openfoodnetwork.org/wp-content/uploads/2015/05/New-Payment-Paypal-1.png)

**Server**

Change the ‘server’ field to ‘live’ – this is case sensitive.

**Solution**

Solution determines whether or not a user needs a PayPal account to check out.

Type “Mark” if you do want users to have a paypal account, or “Sole” if they can checkout without a Paypal account \(with credit card\).

**Landing Page**

You can select which page to show customers once they’re redirected to PayPal.

Type “Login” to direct customer to the login form for PayPal \(if you selected “Mark” above\). Or type “Billing” to show show customers a form where they can enter their credit card data and possibly sign up for a PayPal account \(if you selected “Sole” above\).

%/accordion%

### MasterCard Internet Gateway Service \(MIGS\)

%accordion%MIGS%accordion%

Set up of this service needs to be done through your bank. So far it has been tested with Bendigo Bank.

%/accordion%

### Stripe

%accordion%Stripe%accordion%

[Stripe ](https://stripe.com/au)is an online payment platform similar to Paypal. It will allow you to accept credit card payments from your customers. Stripe is a global platform, but is only available on certain OFN instances. Contact your [local OFN team](https://openfoodnetwork.org/ofn-local/) to see whether it’s available on your OFN.

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

## Fees on Payment Methods

![Calculator](https://openfoodnetwork.org/wp-content/uploads/2015/05/Calculator.png)

You can attach a fee to payment methods. Most commonly this is used to pass on a platform's fees to the customer, such as Paypal fees. 1. Select a fee calculator \(full descriptions below\) 2. Enter the value.

_Note: Payment method fees do not include tax._

#### Fee Calculators

**Flat Percent:**  This fee is charged as a percentage of the total amount charged in the order.

**Flat Rate \(per order\):** This fee is applied as standard fee to all orders, regardless of the size of the order.

**Flexible Rate:** This calculator is typically used for promotional discounts where you charge a reduced fee as the customer makes more purchases of that item. This fee applies to items and products listed per kg or L.

* ‘First Item Cost’: The fee charged for the first item in the order.
* ‘Additional Item Cost’: The fee charged for aditional items beyond the first.
* ‘Max Items’: The maximum number of items on which the fee will be applied. Items purchased beyond this amount will be not be charged the fee.

> For example: If the first cost is $2, Additional Item Cost is $1 and the maximum items is three. If a customer orders 5 of the item, they will be charged $2 for the first item, $1 for the second and third, and no fee for the fourth and fifth.

**Flat Rate \(per item\):** This fee is a constant fee, applied to products listed as ‘items’. \(it will not be applied to products listed as per kg, or per L\)

**Price Sack:** This fee is used to charge a discount on fees for orders which exceed a certain dollar amount.

* ‘Minimum Amount’: If the order’s total is below this amount, they will be charged the ‘Normal Amount’.
* ‘Discount Amount’: Orders which are equal to or greater than the minimum amount will be charged the ‘Discount Amount’.

