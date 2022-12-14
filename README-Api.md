# Back-End-Assessment

## Create an api server for an e-commerce application.

### About the users:

- Users
  - Types
    - Customers - Basic users who can sign up and login with email and password.
    - Admins - These users are responsible to manage regions, products.
  - Users can be both customers and admins.
  - Note: Generate users via seed.

### About the store:

- Regions - This application should be flexible to allow creation of stores in different regions. E.g. Vietnam, Singapore, etc. each with their own currency setup. Only Admins can manage regions.

  - Fields:
    - title (region name)
    - country
    - currency (VND, USD, SGD, etc)
    - tax (e.g, 10% which can be stored in cents)
  - Note: Generate regions via seed.

- Products - Each region has their own set of products. Products can be anything - tshirt, pants, mugs, watches. Only Admins can manage products.
  
  - Fields:
    - title
    - description
    - image_url
    - price
    - sku
    - stock (quantity)
      - Note: Customers should not be allowed to order items beyond the available stock number.
  - Note: Generate products via seed.


### Orders

- Fields:
  - customer_name
  - shipping_address
  - order_total
  - paid_at
- An order can contain multiple items.
- Note: Create CRUD for orders.

### Payment 

- Once the order is made, a payment should be made. Create a fake payment gateway and create a task that is triggered 1 minute after order creation that updates the state of the order to either paid or unpaid.

## Requirements

- Implement JWT authentication for sign_in steps
- Mongoose schemas to model the application data
- Update this README to include a list of API endpoints
- Please upload your code to a repository and add emails raphael.mahiet@eqolux.com and marine@eqolux.com access to that repo.

## What libraries/frameworks, packages, tools can I use?

The project backend is in nodeJS (you can select between js or include ts), but other than that you are free to use whatever
libraries/frameworks, packages, tools that you want.



