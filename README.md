# E-commerce Website Back End

## E-commerce Website Back End
Description
This is a back end for an e-commerce website that uses the latest technologies. It is built with Express.js and uses Sequelize as an ORM to interact with a MySQL database. It provides API endpoints for categories, products, and tags that can be accessed through GET, POST, PUT, and DELETE requests.

## Installation
Clone the repository.
Install dependencies by running  `npm install`.
Create a .env file in the root directory of the project and set the following environment variables:

```
DB_NAME=<database_name>
DB_USER=<mysql_username>
DB_PASSWORD=<mysql_password>
```
Run `npm run` seed to create a development database and seed it with test data.
Run `npm start` to start the server and sync the Sequelize models with the MySQL database.

## Usage
API routes can be accessed using Insomnia Core or any other API client.

## GET Routes
To get all categories, send a GET request to /api/categories.
To get a specific category by ID, send a GET request to /api/categories/:id.
To get all products, send a GET request to /api/products.
To get a specific product by ID, send a GET request to /api/products/:id.
To get all tags, send a GET request to /api/tags.
To get a specific tag by ID, send a GET request to /api/tags/:id.

## POST Routes

To add a new category, send a POST request to /api/categories with the following JSON data:

```
{
    "category_name": "New Category"
}
```
To add a new product, send a POST request to /api/products with the following JSON data:

```
{
    "product_name": "New Product",
    "price": 10.99,
    "stock": 10,
    "category_id": 1,
    "tagIds": [1, 2, 3]
}
```
To add a new tag, send a POST request to /api/tags with the following JSON data:
```
{
    "tag_name": "New Tag"
}
```

## PUT Routes
To update a category, send a PUT request to /api/categories/:id with the following JSON data:

```
{
    "category_name": "Updated Category"
}
```

To update a product, send a PUT request to /api/products/:id with the following JSON data:
```
{
    "product_name": "Updated Product",
    "price": 12.99,
    "stock": 5,
    "category_id": 2,
    "tagIds": [4, 5]
}
```
To update a tag, send a PUT request to /api/tags/:id with the following JSON data:

```
{
    "tag_name": "Updated Tag"
}
```

## DELETE Routes
To delete a category, send a DELETE request to /api/categories/:id.
To delete a product, send a DELETE request to /api/products/:id.
To delete a tag, send a DELETE request to /api/tags/:id.

### Credits: Naz Yasar
