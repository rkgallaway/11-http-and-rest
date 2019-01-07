# LAB: HTTP and REST

## Overview
The goal for this lab is to get your hands dirty in using an API, setting up a simple server that can attach to it and fetch data, and begin the building of a REST client tool that you can use during and after the course.

## Before you begin
* You'll need to initialize this lab folder as a new node module, install your dependencies, setup your npm script commands, and pull in your config files

## Assignments
### JSON API Server
* Implement an API server for a storefront, using json-server
  * Create a new repository called "simple-api"
  * Create a folder called `data` with a `db.json` file
  * Start your json-server from within the `simple-api` folder and "watch" your database file
  * Data models should contain the following fields:
    * `categories`
      * `_id`, `name`, `display_name`, `description`
    * `products`
      * `_id`, `category`, `name`, `display_name`, `description`
  * Your api should respond to the following endpoints:
    * `/categories`  GET, POST
    * `/categories/:id/` PUT, DELETE
    * `/products`  GET, POST
    * `/products/:id/` PUT, DELETE
    
### Swagger Documentation
  * Within your API, Create a folder called `docs`
  * Write and publish swagger documentation for your API
    * Compose with [Swagger Editor](https://swagger.io/tools/swagger-editor/) or [Swagger Hub](https://swagger.io/tools/swaggerhub/)

### Stretch Goal
Implement a Web Server with express and ejs
  * Static routes and assets served from the public folder
  * Use 'ejs' as your 'view engine'
  * Implement your page views as you see fit
  * Implement 2 get routes that will use `superagent` to fetch data from your API
  * /
    * Home Page
        * Lists each category and draws a link to a detail page (/category/:name)
  * /category/:name
    * Lists the products in the category


### Testing
**No automated testing is required for this assignment**
Run your server against someone else's API


###  Documentation
Complete the README.md file included in the lab folder
