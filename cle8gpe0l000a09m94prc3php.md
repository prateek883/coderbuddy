# Medusa - a Shopify Alternative

## Introduction

A [medusa](https://medusajs.com/) is an open-source composable commerce engine built for developers. Out of the box, it offers a large portion of Shopify's basic features. When a company demands change, its open abstraction-based architecture allows for adaptations and simple maintenance, making it a wonderful fit for creating unique and scalable solutions.

One of the world's fastest-growing open-source initiatives, Medusa has surpassed well-known options like WooCommerce and Magento to become the most starred Javascript e-commerce platform on GitHub. The technology already serves websites that sell more than $100 million a year and is in use worldwide.

## Architecture of Medusa

The **admin panel**, **the store front**, and the **Medusa server** make up the entire system.

### Medusa server

The Medusa server is a Node. js-based headless backend. This is the core element that contains all of the store's logic and data. REST APIs are used by your admin dashboard and storefront to communicate with the backend and retrieve, create, and edit data.

All of the Medusa server's checkout-related features will be available to you. This covers user management, shipping and payment processors, cart management, and other things. Also, you can specify your store's region, tax laws, promotions, gift cards, and more.

### Admin Dashboard

Operators of stores can access the [admin dashboard](https://demo.medusajs.com/). The admin dashboard allows store owners to see, edit, and amend data, including orders and products.

You can use the lovely admin dashboard that Medusa provides right away. The admin dashboard for Medusa has many tools for managing your store, including control of orders, products, users, and more.

### Storefront

The Storefront is used by your customers to browse your inventory and place orders. Two shops, one created with Next.js and the other with Gatsby, are offered by Medusa. With the Storefront REST APIs, you are also free to build your own storefront.

## Features of Medusa

* **Orders, exchanges, and returns** - Medusa offers a simple and automatic method for handling swaps, returns, and claims.
    
* **Customers and Customer Groups** - Customers should be managed and assigned to customer groups.
    
* **Products and Collections** - Add items with a lot of personalization options, then group them into collections.
    
* **Region** - From a single platform, configure and manage various currencies and locations.
    
* **Plugins** - It is simple to combine notification services, fulfilment services, payment systems, and many more unique tools and third-party services.
    

## Install Medusa using the create-medusa-app

Learn how to use create-medusa-app to construct a Medusa project using the three key elements of Medusa in this tutorial.

The materials and tools needed to set up each of the three components independently are provided by Medusa. Because they can select any framework for the storefront and administrative dashboard, this guarantees that developers have complete choice in selecting their tech stack.

Instead of making each component independently, you can use the `create-medusa-app` command if you want to use Medusa's beginnings for the three parts.

The `create-medusa-app` command will simultaneously install a Medusa server, Medusa admin, and optionally a shop.

Before, going further you need to have [node.js](https://nodejs.org/en/) installed and [Git](https://git-scm.com/).

## Creating a Medusa Project

The server, storefront, and admin are the three components of a Medusa project.

By using the following command, you can create the medusa project.

`npx create-medusa-app`

### Project Directory Name

The name of the directory where you wish the project to be installed will then be requested of you. You can provide a new name or leave the default value, `my-medusa-store`.

### Choose the Medusa Server starter

You will then be prompted to select the Medusa server starting. A beginning template is used to develop the Medusa Server. It is produced by default using the `medusa-starter-default` template.

You can select the Contentful starter, the default Medusa server starter, or enter a starter URL by selecting `Other`:

? `Which Medusa starter would you like to install?` …

❯ `medusa-starter-default`

`medusa-starter-contentful`

`Other`

### Choose the Storefront server

After selecting the Medusa starter, terminal will asked to choose the storefront starter. You can choose one of the starters in the list included or choose `None` to skip installing a storefront:

? `Which storefront starter would you like to install?`

❯ `Gatsby Starter Next.js Starter`

[`medusa.express`](http://medusa.express) `(Next.js)`

[`medusa.express`](http://medusa.express) `(Gatsby)`

`Gatsby Starter (Simple)`

`None`

### Dependency Installation

After selecting one of the beginnings listed above, the installation of each component and any related dependencies will start. You'll see instructions for starting each component after the installation is complete.

`Your project is ready. The available commands are:`

`Medusa API`

`cd my-medusa-store/backend`

`yarn start`

`Admin`

`cd my-medusa-store/admin`

`yarn start`

`Storefront`

`cd my-medusa-store/storefront`

`yarn develop # for Gatsby storefront`

`yarn dev # for Next.js storefront`

## Conclusion

In this blog, we learned about the medusa a shopify-alternative which means developers can use this great technology to built the custom ecommerce application.

Thanks for reading!