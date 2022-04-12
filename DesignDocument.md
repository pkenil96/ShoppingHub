# ShoppingHub

Seller, Buyer and System will be three separate microservices

***Microservices***

* Seller
    1. Add Product
    2. Edit Product
    3. Delete Product

* Buyer
    1. Search Product(s)
        -by name
        -by category
        -by brand
    2. Add Product to cart
    3. Remove Product from cart
    4. Update Product quantity in cart
    5. Checkout items in cart
    6. Place Order
    7. Make payment - 3rd party integrations (Stripe, Paypal, Venmo)
    8. Track Order
    9. Cancel Order
	10. Subscribe to a seller - User gets notified whenever a given seller adds a product
	11. Chat support - Buyer can reach out to the customer support to report issues with purchase

* System
    1. Send notifications to subscribers when Product becomes available
    2. Send notifications to users when OrderStatus changes
	3. Show recommended items in the cart when user checks out

Other Features
    1. Buyer: Every information about the buyer except the id should be encrypted
    2. Seller: Every information about the seller except the id and produts should be encrypted

Implementation Details

***Classes, Interfaces, Enum***

Product (Class)

* Attributes
  -name
  -productId
  -imageUrl
  -weight
  -price
* Methods

OrderStatus (Enum)
 -PENDING
 -PROCESSING
 -SHIPPED
 -COMPLETE
 -CANCELLED
