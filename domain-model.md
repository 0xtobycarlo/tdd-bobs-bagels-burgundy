
| Object | Properties                   | Method      | Input                                   | Output                         |
| ------ | ---------------------------- | ----------- | --------------------------------------- | ------------------------------ |
| Menu   |                              | getMenu{}   |                                         | menu object                    |
|        |                              |             |                                         |                                |
| Basket | basket = [], basket-size = # | getBasket() |                                         | basket [array]                 |
|        |                              | addItem()   | item name(str), item quantity(#)        | no output                      |
|        |                              | removeItem()| item name(str)                          | basket [array] or error (str)  |
|        |                              | basketcapacity|                                       | items in basket (#), < error   |
|        |                              | priceChecker| item name(str)                          |                                |
|        |                              | basketTotal |                                         | total price (#)                |

-=+=-

** User Stories

Part I
------------
As a member of the public
So I can order a bagel when I want to
I'd like to add an item to my basket.

As a member of the public,
So that I can change my order
I'd like to remove an item from my basket.

Methods:
----------------
addItemToBasket() (addItemToBasket = .push[basketItems]) => invoke isBasketFull() method
removeItemFromBasket()


Part II
------------
As a member of the public,
So that I can not overfill my small bagel basket
I'd like to know when my basket is full when I try adding an item beyond my basket capacity.

As a Bob's Bagels manager,
So that I can record more sales
I’d like to create baskets with larger capacity when I need to.

As a member of the public
So that I can maintain my sanity
I'd like to know if I try to remove an item that doesn't exist in my basket.

Methods:
----------------
isBasketFull() (return a boolean depending on capacity of basket - small 5, medium 10, large 15 items)


Part III
------------
As a member of the public,
So that I can know how much my bagels are,
I’d like to see the price of each item before I add it to my basket.

As a member of the public,
So that I can prepare to pay
When I go to checkout I'd like to know the total sum of the bagels in my basket.

Methods: 
----------------
basket.basketTotal() 