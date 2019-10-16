# How to add products to DB
Run the console command 'rails c' and write:
$ rail c
Product.create!([{ name: 'apple', price: 5.55, description: '1 kg' },
                          { name: 'water', price: 2.15, description: '1.5 l' },
                          { name: 'bread', price: 1.79, description: '0.5 kg' },
                          { name: 'beef', price: 10, description: '0.6 kg' },
                          { name: 'potato', price: 9.99, description: '5 kg' }])

To check products in the DB, run the console command 'rails s' and write:
$ curl -H "Accept: application/json" "http://localhost:3000/api/products"
It shows the list of the products.

To check specific product in the DB, run the console command 'rails s' and write:
$ curl -H "Accept: application/json" "http://localhost:3000/api/products/1"
It shows the information about the product with id = 1.
