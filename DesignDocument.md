# Dukaan

Seller, Buyer and System will be three separate microservices.

***Microservices***

* Seller
    1) Add Product
    2) Edit Product
    3) Delete Product

* Buyer
    1) Search Product(s)
        -by name
        -by category
        -by brand
    2) Add Product to cart
    3) Remove Product from cart
    4) Update Product quantity in cart
    5) Checkout items in cart
    6) Place Order
    7) Make payment
    8) Track Order
    9) Cancel Order

* System
    1) Send notifications to subscribers when Product becomes available
    2) Send notifications to users when OrderStatus changes

***ENUMS***

```enum OrderStatus {
    PENDING,
    PROCESSING,
    SHIPPED,
    COMPLETE,
    CANCELLED
}```


***Classes and Interfaces***

```Product {
    String name;
    String id;
    String imageUrl;
}```