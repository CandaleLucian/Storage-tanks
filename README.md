# Storage-tanks

Online tanks store with administrator panel

	Brief description of the system
Application allows you to add products to the tanks store through the administrative panel and the system is to enable user registration and login as well as placing orders.

	Main system function
Login panel.
Admin:
-adding categories for products
-category tree overview
-adding products
-product list + edition

User:
-registration
-list of products
-product table with pagination

	General Guidelines
Building a website using Django.
Introducing the division into models, views and controllers in the application and placing the
appropriate logic in each of them.
Securing access to the application and functionality by using django.contrib.auth.

	Basic entities
Category
-name
-parent categories and 'cildren' categories(tree placement)

User account
-login(email)
-password(hash)
-address (country, city, street, ZIP code)
-preferred communication channel (mail / email)

Product
-title
-description
-category(entity)
-price
-product type(enum)
-author(entity)

Order line
-product(entity)
-number of products
-product price

Order
-user name
-total cost
-delivery address
-user address
-date of submission
-order lines(entity)
-client(entity)
-status(enum)

Author
-name
-surname

Role
-role name

Cart(not entity)
Order lines

	Functionalities
ADMIN:
Adding a category
-category name
-parent id

	Category tree overview
-category search
-option to drag categories (change position)

	Adding a product
-name
-description
-picture url
-availability
-price
-product type(dropdown)
-category(dropdown)
-author(dropdown)

	Product list
-list of all added products with their details
-button to go to edition of the given product
-product search

USER:

	User registration
-entering data into form fields + validation of the these fields

Log in
-user login option (after prior registration)
-possibility for the user to log out

	Weather widget
-displaying weather based on the city of the currently logged user
	
	Product list
-it is possible to display products as a list or as a grid
-product search
-adding product to cart


	Table with products(using Ajax on the GET query and inserting parameters into the url)
-displaying products in a table with pagination(selection of the number of the products on the page)
-sorting products in the table
-Ajax product search
-adding products to the cart

	Cart
-displaying products added to the cart
-option to order products from the cart -> leads to a static thank you page and reduces product availability

	Additional tanks and extensions
-the ability to edit the user account (data)
-overview of user orders (from user and admin level)
-adding author in the admin panel

	Additional requirements
-it is necessary to ensure an aesthetic and fucntional way of presenting data
-data collected from the user should be pre-validated

	Main Pages:
-Home
-Products
-Contact


