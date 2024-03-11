1.The relationship between the product and product_category entities is indirect through the product_inventory table.
Each row in the product_inventory table represents a specific product along with its inventory details, including the category_id indicating the product's category.
2.By implementing a database constraint using a foreign key relationship between the "product" and "product_category" tables we can 
ensure that each product in the "product" table has a valid category assigned to it.
In database schema, At first need to define a foreign key constraint on the "category_id" column in the "product" table. This constraint references the "id" column in the "product_category" table.
With the foreign key constraint in place, the database ensure that any value inserted or updated in the "category_id" column of the "product" table must exist in the "id" column of the "product_category" table.
