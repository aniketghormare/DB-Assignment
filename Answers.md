## Answers to Database Schema Assignment

**Question 1: Relationship between Product and Product_Category**

The relationship between "Product" and "Product_Category" entities is **one-to-many**. A product can belong to **one** category, but a category can have **many** products. This is enforced by the presence of a foreign key called "category_id" in the "Product" table.

Ex.  Think of it like clothes in a store. A single shirt (product) belongs to one clothing type (category) like t-shirts, jackets, etc. But, a clothing type (category) can have many shirts (products) within it. This connection is established through the "category_id" in the product table, which acts like a label linking each shirt to its category. 

**Question 2: Ensuring Valid Category Assignment**

There are two ways to ensure each product has a valid category:

1. **NOT NULL constraint on category_id:** This prevents product insertion without a valid category.

ex. No shirt gets added without a proper clothing type label. Just like this, we can prevent products from being added without a valid category assigned.

2. **Default value for category_id:** Set a default value like an "Uncategorized" category ID. This ensures all products have a category, even if not the most specific.

ex. Shirts get a default label like "Uncategorized" if they don't have a specific type yet. Similarly, products can have a default category assigned (like "Uncategorized") if no specific category is chosen initially.
