# Five-Guys
Second Group Project

# User story

Client:
As a restaurant owner
When a client visits my website I want them to be able to log in.
Once they have logged in, I want them to be able to view my menu.
When they click on a menu item it's added to their order.
When the customer logs out and reopens the page later, I want the page to remember their incomplete order.
If a customer wants, they should be able to 'favorite' orders.
When a customer completes an order, they need to select whether it's for delivery or pickup
If it's for delivery they need to enter their address.
I want the customer to be able to either pay with a credit card online, or select "pay in cash".


# Database structure
This doesn't have to be how it's implemented, this is just an idea.

- User
    - id
    - Email
    - Hashed password
    - cart_id (references a cart id)

- Menu Items
    - id
    - name
    - description
    - price

- Cart
    - id
    - user_id
    - menu_item_id

Many menu items belong to many users through Cart.
