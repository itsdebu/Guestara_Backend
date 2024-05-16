Certainly! Below is a README file for your Menu Management App:

---

# Menu Management App

This is a menu management application built with Express.js for handling various operations related to categories, subcategories, and items.

## Running the Server

To run the server, use the following command:

```bash
npm run dev
```

## Routes

### Admin Routes

- **POST /api/admin/signup**: Register a new admin.
- **POST /api/admin/login**: Log in as an admin.

### Category Routes

- **POST /api/category/create**: Create a new category. (Requires authentication)
- **POST /api/category/edit/:categoryId**: Edit an existing category. (Requires authentication)
- **GET /api/category/get**: Get all categories or filter by name or ID.

### Subcategory Routes

- **POST /api/subcategory/create**: Create a new subcategory. (Requires authentication)
- **POST /api/subcategory/edit/:subId**: Edit an existing subcategory. (Requires authentication)
- **GET /api/subcategory/get**: Get all subcategories or filter by name, ID, or category ID.

### Item Routes

- **POST /api/item/create**: Create a new item. (Requires authentication)
- **POST /api/item/edit/:itemId**: Edit an existing item. (Requires authentication)
- **GET /api/item/get**: Get all items or filter by name, subcategory ID, category ID, or item ID.

## Authentication

Authentication is required for certain routes. It is implemented using JWT tokens. To access routes that require authentication, include a valid token in the request headers.

## API Usage

### Category

- To get all categories, send a GET request to `/api/category/get`.
- To get a category by name, send a GET request to `/api/category/get?catname=your_category_name`.
- To get a category by ID, send a GET request to `/api/category/get?catId=your_category_id`.

### Subcategory

- To get all subcategories, send a GET request to `/api/subcategory/get`.
- To get a subcategory by name, send a GET request to `/api/subcategory/get?subname=your_subcategory_name`.
- To get a subcategory by ID, send a GET request to `/api/subcategory/get?subid=your_subcategory_id`.
- To get subcategories by category, send a GET request to `/api/subcategory/get?catid=your_category_id`.

### Item

- To get items by name, send a GET request to `/api/item/get?itemname=your_item_name`.
- To get items by subcategory, send a GET request to `/api/item/get?subid=your_subcategory_id`.
- To get items by category, send a GET request to `/api/item/get?catid=your_category_id`.
- To get an item by ID, send a GET request to `/api/item/get?itemid=your_item_id`.


### Thankyou 
### Assignment By Divyanshu Verma
