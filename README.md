# Product

Given two files `app.js` and a database file `product.db` consisting a table `product`.

Write APIs to perform operations on the table `product` containing the following columns,

| Columns        | Type    |
| -------------- | ------- |
| product_id     | INTEGER |
| product_name   | TEXT    |
| Item_number    | INTEGER |

### API 1

#### Path: `/products/`

#### Method: `GET`

#### Description:

Returns a list of all products in the product table

#### Response

```
[
  {
    productId: 1,
    productName: "XXX",
    itemNumber: 5,
   
  },

  ...
]
```

### API 2

#### Path: `/products/`

#### Method: `POST`

#### Description:

Creates a new product in the table (database). `product_id` is auto-incremented

#### Request

```
{
  "productName": "YYY",
  "itemNumber": 17,
  
}
```

#### Response

```
Product Added to Table
```

### API 3

#### Path: `/product/:productId/`

#### Method: `GET`

#### Description:

Returns a product based on a product ID

#### Response

```
{
  productId: 1,
  productName: "ZZZ",
  itemNumber: 5,
  
}
```

### API 4

#### Path: `/products/:productId/`

#### Method: `PUT`

#### Description:

Updates the details of a product in the team (database) based on the product ID

#### Request

```
{
  "productName": "EEE",
  "itemNumber": 54,
  
}
```

#### Response

```
Product Details Updated

```

### API 5

#### Path: `/products/:productId/`

#### Method: `DELETE`

#### Description:

Deletes a product from the table (database) based on the product ID

#### Response

```
Product Removed
```

<br/>

Use `npm install` to install the packages.

**Export the express instance using the default export syntax.**

**Use Common JS module syntax.**
