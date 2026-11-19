# Shop Project

An online shop for digital products, with a blog and an admin panel. I built it between **December 2016 and January 2017** using **Laravel**, while I was learning the framework. It's based on my [Laravel blog](https://github.com/ziggymant/laravel-blog) project. To that blog I added a product catalogue, a shopping cart, Stripe payments, orders and file downloads. I've kept it here as a record of where I started, so it shows the code as it was then. It isn't maintained or production-ready.

## What it does

- Shows a shop where visitors can browse products by category, search them and open a page for each product.
- Lets logged-in users add products to a cart, remove them and see the total price.
- Takes card payments at checkout through **Stripe**, using test mode. Each payment is saved as an order.
- Lets customers see their past orders and download the digital files they bought.
- Lets customers leave reviews with star ratings, and shows each product's average score.
- Includes an admin panel for managing products, files, users, roles, blog posts, categories, photos and comments, with a rich text editor for descriptions.
- Shows a blog with posts, comments and replies, and requires new users to confirm their email address.

## Technologies used

- **PHP** with **Laravel 5.3**, including Eloquent ORM, Blade templates, migrations, resource controllers, middleware, form requests, authentication and mail
- **Laravel Cashier** and **Stripe** for payments
- **MySQL** as the database
- **Bootstrap**, **jQuery** and the **Summernote** rich text editor
- Laravel packages:
  - `laravelcollective/html` for forms
  - `cviebrock/eloquent-sluggable` for readable post addresses
  - `consoletvs/charts` for the dashboard charts
- **Gulp** with **Laravel Elixir**, **Composer**, **npm** and **Git**

## What I learned

- How to add new features to an existing project, turning a blog into a working e-shop.
- How to design the database for a shop, with tables for products, carts, cart items, orders, order items, files and reviews.
- How to connect an app to an outside payment service, Stripe, through Laravel Cashier.
- How a checkout works: adding up the cart, charging the card, creating the order and emptying the cart.
- How to keep purchased files private and only let customers who bought them download them.
- How to build a review and rating system.
- How to make steady progress by committing small, working steps.
