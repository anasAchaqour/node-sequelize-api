# CRUD API with Express and Sequelize

This CRUD API allows you to perform basic CRUD (Create, Read, Update, Delete) operations on products and reviews. The backend is built using Express.js and Sequelize ORM for interacting with the database.

## Endpoints

### Products

#### Create a Product
- **POST** `/addProduct`
  - Adds a new product to the database.
  - Controller: `productController.addProduct`

#### Get All Products
- **GET** `/allProducts`
  - Retrieves all products from the database.
  - Controller: `productController.getAllProducts`

#### Get Published Products
- **GET** `/published`
  - Retrieves all published products from the database.
  - Controller: `productController.getPublishedProduct`

#### Get One Product
- **GET** `/:id`
  - Retrieves a single product by ID from the database.
  - Controller: `productController.getOneProduct`

#### Update a Product
- **PUT** `/:id`
  - Updates an existing product's details in the database.
  - Controller: `productController.updateProduct`

#### Delete a Product
- **DELETE** `/:id`
  - Deletes a product from the database.
  - Controller: `productController.deleteProduct`

### Reviews

#### Get All Reviews
- **GET** `/allReviews`
  - Retrieves all reviews from the database.
  - Controller: `reviewController.getAllReviews`

#### Add a Review
- **POST** `/addReview/:id`
  - Adds a new review for a specific product.
  - Controller: `reviewController.addReview`

#### Get Product Reviews
- **GET** `/getProductReviews/:id`
  - Retrieves all reviews for a specific product by ID.
  - Controller: `productController.getProductReviews`

