# Node API 2 Guided Project Starter Code

Guided project starter code for **Node API 2** module.

In this project we will learn how to create a very simple Web API using `Node.js` and `Express`, and cover how to use `Express Routers` to break up the application to make it more maintainable.

## Prerequisites

- a REST client like [insomnia](https://insomnia.rest/download/) or [Postman](https://www.getpostman.com/downloads/) installed.

## Project Setup

- [ ] fork and clone this repository.
- [ ] **CD into the folder** where you cloned **your fork**.
- [ ] type `npm i` to download dependencies.

Please follow along as the instructor builds the API step by step.


## Public Endpoints

- Hubs Resource: /api/hubs
- Clients: /api/clients
- Products: /api/products

Create a Product => /add_product (bad way) ---> the RESTful way is: POST /api/products
Update a Product => /update_product (bad way) ---> the RESTful way is : PATCH/PUT /api/products/:id

## Private Endpoints

- Clients: /admin/clients
- Products: /admin/products

## Query Strings

localhost:4000/api/hubs?limit=5&page=3

`?limit=5` <--- query string

? ---> the begining of the query string

limit=5 ---> key/value pair

& ---> seperates other key/value pairs

page=3 ---> another key/value pair

On the server we access the query string at `req.query`;

