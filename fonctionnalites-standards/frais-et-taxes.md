# Marges et commissions

Cette fonctionnalité est utile pour les producteurs et les hubs travaillant ensemble : cela permet d'allouer les coûts associés à l'administration, l'emballage, le transport et la vente à chacune des parties prenantes. Pour les producteurs vendant leurs propres produits en direct, ces coûts sont déjà présents dans le prix du produit, ainsi appliquer des marges ou des commissions ne semble pas nécessaire.

Lorsqu'une marge est appliquée, le consommateur est capable de voir la constitution du prix sur la boutique en cliquant sur le camembert. Exemple ci-dessous :

![](../.gitbook/assets/image%20%287%29.png)

## Accéder au menu marge et commissions

Sur l'interface d'administration, rendez-vous sur le menu **Enterprises**, puis cliquez sur **Gérer **et enfin sur "marges et commissions" dans le menu de gauche.

![](../.gitbook/assets/image%20%282%29.png)

## Ajouter des marges et commissions

![](../.gitbook/assets/image%20%2826%29.png)

**Entreprise :** Dans la première colonne, sélectionnez l'entreprise qui recevra la marge.

**Type de marge** **: **Sélectionnez le service lié à la marge \(transport, emballage...\)

**Nom : **Choisissez un nom pour la marge.

**TVA applicable : **Sélectionnez la TVA applicable. Si aucune TVA n'est appliquée, indiquez "TVA 0%".

**Calculateur : **La marge peut être calculée de différentes manières. Sélectionnez le calcul qui s'applique le mieux.

Pour finaliser, cliquez sur "Mettre à jour". Une fois que la marge a été créée, vous pouvez indiquer comment la marge sera calculée dans la colonne "Montant pour calculs".

![](../.gitbook/assets/image%20%2815%29.png)

### Le calculateur

![](../.gitbook/assets/image%20%2821%29.png)

**Pourcentage net **– This fee is charged as a percentage of the total amount charged in the order.

**Poids \(au kg\) **– cette marge s'applique aux produits vendus par kg. Elle ne s'appliquera donc pas aux produits vendus à la pièce.

**Flat Rate \(per order\) **– Cette marge s'applique de manière standard à toutes les commandes, quelque soit leur taille ou leur unité.

**Taux flexible** – Ce calcul est utilisé pour les remises promotionnelles \(quand vous appliquez une marge réduite lorsque le consommateur achète en gros\).

* ‘Coût du premier item’ : La marge appliquée au premier produit
* ‘Coût d'item additionnel’ : La marge appliquée aux produits suivants
* ‘Nombre maximum d'objets’ : Le nombre maximum d'objets sur lesquels la marge va s'appliquer. Les objets après ce nombre n'auront pas de marge associée.

![](../.gitbook/assets/image%20%284%29.png)

Exemple :  Si la marge du premier est de 2€, celle de l'objet supplémentaire 1 € et le nombre maximum d'objet est de 3. Si un client en commande 5, il paiera 2 € pour le premier, 1€ pour le second et aucune commissions pour les objets 3 et 4.

**Taux net \(par item\)** – Cette marge est constante et s'applique uniquement aux produits vendus à la pièce \(et non ceux vendus au poids\).

**Price Sack **– Cette marge est utilisée pour appliquer une marge réduite à partir du moment où la commande atteind un certain montant.

* ‘Montant minimal’ : Si la commande est en-dessous de ce montant, le consommateur devra payer le ‘Montant normal'.
* ‘Montant de la réduction’ : Si la commande est égale ou supérieure au montant minimal, le consommateur devra payer le ‘Montant de la réduction’.
* 'Currency' : La monnaie utilisée \(généralement "EUR"\).

