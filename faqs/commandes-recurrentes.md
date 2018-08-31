# Commandes récurrentes

**If I remove an OC from a schedule when it already has open subscription orders attached to it, what will happen to those orders? Will those subscriptions get deleted?**

Those orders will remain open. At the close of the order cycle the subscription orders will be processed like normal subscription orders. If you wanted to cancel all subscription orders that were attached to that order cycle you would need to [delete each subscription order individually](https://guide.openfoodnetwork.org/advanced-features/subscriptions/subscriptions-creating-and-managing-orders#edit-one-specific-order).

**If I add a new subscription in the middle of an open order cycle, will there be a subscription generated for that customer?**

Yes, if you create a subscription while there is an open order cycle in that schedule, an order will be generated for that customer. If you don't want the subscription to apply to the current open order cycle you'll need to set the start date of the subscription to be after the close of that order cycle.

**What if part of the stock is available but not all? Which customers get the limited stock?**

In the case that a product’s stock on hand value is not adequate to meet all subscription orders, the limited stock won’t be allocated evenly across customers, instead it will fulfill customers orders with available stock until it runs out. Some customers will receive their full order, others will receive none.

**What if I change the subscription while it’s ‘open’?**

Any changes you make to the core subscription, while an OC is open, will carry on to the open subscription order. The second email confirmation going to the customer at the close of the order cycle will reflect the changes you make. If you don’t want the changes to apply to the open order, you’ll need to edit the subscription after the close of the order cycle.

**What if there’s limited stock, but then a customer cancels their order, will this stock get automatically allocated to other subscribers who wanted that product but couldn’t have it due to insufficient stock?**

No, if a customer cancels their subscription order or removes a product from it, that stock will be returned to the products's on hand value. It won't automatically be allocated to other customers, but you could now add this stock to another customer's order manually by editing their order.

