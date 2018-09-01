# Méthodes de paiement

Vous devez créer des méthodes de paiement avant de pouvoir ouvrir votre boutique.

## Paramétrer une méthode de paiement

1\) Accéder à la page traitant des méthodes de paiement

Cliquez sur **Entreprises**, puis cliquez sur **Gérer**. Cliquez ensuite sur Méthodes de paiement sur le menu vertical de gauche :

![](../../.gitbook/assets/image%20%2816%29.png)

2\) Cliquez sur "**En créer une maintenant**".

3\) Si ce n'est pas le cas sélectionnez votre entreprise dans la liste déroulante des hubs. Cela signifie que la méthode de paiement qui sera créé le sera pour cette entreprise. **Vous pouvez sélectionner plusieurs entreprises**.

![](../../.gitbook/assets/image%20%2844%29.png)

4\) **Nom :** Choisissez un nom pour cette méthode de paiement. \(par exemple : "Payez par carte de crédit en utilisant Paypal" etc\). Ce nom s'affichera au moment du paiement pour l'acheteur, ainsi que dans les emails de confirmation qui lui seront envoyés.

5\) **Description :** ajoutez des détails pour la méthode de paiement. Par exemple, pour un virement, vous pouvez indiquez les détails du RIB. Cette description s'affichera au moment du paiement pour l'acheteur, ainsi que dans les emails de confirmation qui lui seront envoyés.

Un exemple de message au moment du paiement :

![](../../.gitbook/assets/image%20%2859%29.png)

 6\) **Active :** Indiquez si vous souhaitez que cette méthode soit visible et utilisable

7\) **Tags :** Utilisez les tags si vous souhaitez rendre certaines méthodes de paiements accessibles ou non pour certains types d'acheteurs \(voir [la page suivante](customized-shopping-experience.md#customer-tagging) pour l'utilisation de cette fonctionnalité\).

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

![](../../.gitbook/assets/image%20%2899%29.png)

**Serveur :** Indiquez " live "sans les guillemets à la place de "sandbox".

**Solution :** Ce champ détermine si les utilisateurs devront avoir un compte paypal pour payer ou non. Laissez "Mark" si l'utilisateur doit avoir un compte paypal, indiquez "Sole" si vous souhaitez le contraire.

**Landing Page :** vous pouvez sélectionner la page d'accueil une fois les utilisateurs redirigés vers paypal pour leur achat. Si vous avez sélectionné "Mark" avant, il vaut mieux indiquer "Login". Si non, "Billing" les renverra directement vers un écran leur permettant d'indiquer leur numéro de carte bleue.

### MasterCard Internet Gateway Service \(MIGS\)

Ce paramétrage ne peut être fait que via votre banque.

### Stripe

[Stripe ](https://stripe.com/au)est une plateforme de paiement en ligne similaire à PayPal. Cette plateforme acceptera les paiements par carte bleue également.

Contrairement à Paypal, l'acheteur final n'a pas besoin de compte. 

Si vous souhaitez utiliser la fonctionnalité d'**abonnements**, la seule méthode de paiement possible est d'utiliser Stripe \(aucun autre ne permet le règlement d'abonnements\).

#### Paramétrage

**Connecter avec Stripe**

Avant d'utiliser Stripe, il faut le connecter. Cliquez sur ce bouton \(menu Entreprises &gt; Gérer &gt; Méthode de paiements\) :

![](../../.gitbook/assets/image%20%2819%29.png)

Vous serez redirigé vers un formulaire : soit vous avez déjà un compte Stripe et il suffit de vous connecter, soit vous devrez vous créer un compte.

Les informations demandées incluent votre pays, votre activité, votre numéro SIREN, de TVA, votre adresse...

**Créer une nouvelle méthode de paiement**

Une fois connecté avec Stripe, créer votre méthode de paiement comme indiqué ci-dessus.

Sélectionnez Stripe dans la liste des fournisseurs

**Stripe Account Owner :** sélectionnez l'entreprise avec laquelle vous avez créé le compte Stripe ou réalisé la connexion.

Si vous sélectionnez une entreprise qui n'a pas de compte Stripe connecté, vous aurez le message d'erreur ci-dessous. Soit cliquez sur "En connecter un", soit répétez les opération ci-dessusà partir du bouton "connecter avec stripe"

![](../../.gitbook/assets/image%20%283%29.png)

#### Les paiements stripe pour les acheteurs

Quand les acheteurs utilisent Stripe, il peuvent cocher une case pour que leur carte de crédit soit enregistrée pour leurs prochains paiements \(seulement s'ils sont connecté à OFF\). Dans leur profil, ils peuvent également ajouter une carte ou en supprimer une.

## Commissions sur les méthodes de paiements

![](../../.gitbook/assets/image%20%2895%29.png)

Vous pouvez associer une marge ou une commission à une méthode de paiement. Généralement c'est utilisé pour répercuter les frais des plateformes de paiement à l'acheteur. Sélectionnez un calculateur et indiquez un montant \(voir description ci-dessous\). 

_Remarque : les commissions sur les méthodes de paiement n'incluent pas les taxes._

### Le calculateur

**Pourcentage net** – Cette marge s'applique en pourcentage du montant total de la commande.

**Taux net \(par commande\)** – Cette marge s'applique de manière standard à toutes les commandes, quelque soit leur taille ou leur unité.

**Taux flexible** – Ce calcul est utilisé pour les remises promotionnelles \(quand vous appliquez une marge réduite lorsque le consommateur achète en gros\).

* ‘Coût du premier item’ : La marge appliquée au premier produit
* ‘Coût d'item additionnel’ : La marge appliquée aux produits suivants
* ‘Nombre maximum d'objets’ : Le nombre maximum d'objets sur lesquels la marge va s'appliquer. Les objets après ce nombre n'auront pas de marge associée.

![](../../.gitbook/assets/image%20%2810%29.png)

Exemple :  Si la marge du premier est de 2€, celle de l'objet supplémentaire 1 € et le nombre maximum d'objet est de 3. Si un client en commande 5, il paiera 2 € pour le premier, 1€ pour le second et aucune commission pour les objets 3 et 4.

**Taux net \(par item\)** – Cette marge est constante et s'applique uniquement aux produits vendus à la pièce \(et non ceux vendus au poids\).

**Price Sack** – Cette marge est utilisée pour appliquer une marge réduite à partir du moment où la commande atteind un certain montant.

* ‘Montant minimal’ : Si la commande est en-dessous de ce montant, le consommateur devra payer le ‘Montant normal'.
* ‘Montant de la réduction’ : Si la commande est égale ou supérieure au montant minimal, le consommateur devra payer le ‘Montant de la réduction’.
* 'Currency' : La monnaie utilisée \(généralement "EUR"\).

