![CF](http://i.imgur.com/7v5ASc8.png) LAB 11
=================================================

## Lab 11 HTTP and ReST

### Author: Ryan Gallaway collaborated with Fletcher LaRue

### Links and Resources

[![Build Status](https://www.travis-ci.com/rkgallaway/11-http-and-rest.svg?branch=master)](https://www.travis-ci.com/rkgallaway/11-http-and-rest)

* [repo](https://github.com/rkgallaway/11-http-and-rest)
* [travis](https://www.travis-ci.com/rkgallaway/11-http-and-rest)
* [back-end](https://lab-11-http-and-rest-rg-fl.herokuapp.com)

### Modules
#### `server.js`
##### Exported Values and Methods

## Overview
The goal for this lab is to get your hands dirty in using an API, setting up a simple server that can attach to it and fetch data, and begin the building of a REST client tool that you can use during and after the course.

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


### Setup
#### `.env` requirements
* `PORT` - port defined in env

#### Running the app
* `npm i` to install dependencies 
* `npm start`

#### Tests
* `npm run lint`
* testing not required for this lab

