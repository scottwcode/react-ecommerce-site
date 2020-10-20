TheStore eCommerce Platform
eCommerce webSite built with React, MongoDB, Express, NodeJS, Mongoose, Redux and several other technogies.

Features
Shopping cart
Product reviews & ratings
Top rated products carousel
Product pagination
Product search 
User profile maintenance and order list
Admin product management
Admin user management
Admin Order details page
Mark orders as delivered
Checkout process (shipping address, payment method, etc)
PayPal / credit card integration
Database seeder (products & users)

Usage
ES Modules in Node
We use ECMAScript Modules in the backend in this project. Be sure to have at least Node v14.6+ or you will need to add the "--experimental-modules" flag.

Also, when importing a file (not a package) to the backend section, be sure to add .js at the end or you will get a "module not found" error

Since this project uses MongoDB as the database and paypal sandbox as a test payment authenticator, you should have accounts set up with these tools in order to have the uri and ids/keys needed to use these products.

Env Variables
Create a .env file in then root and add the following

NODE_ENV = development
PORT = 5000
MONGO_URI = your mongodb uri
JWT_SECRET = 'abc123'
PAYPAL_CLIENT_ID = your paypal client id
Install Dependencies (frontend & backend)
npm install
cd frontend
npm install
Run
# Run frontend (:3000) & backend (:5000)
npm run dev

# Run backend only
npm run server
Build & Deploy
# Create frontend prod build
cd frontend
npm run build
There is a Heroku postbuild script, so if you push to Heroku, no need to build manually for deployment to Heroku

Seed Database
You can use the following commands to seed the MongoDB database with some sample users and products as well as destroy all data

# Import data
npm run data:import

# Destroy data
npm run data:destroy
Sample User Logins

admin@example.com (Admin)
123456

john@example.com (Customer)
123456

jane@example.com (Customer)
123456
License
The MIT License

Copyright (c) 2020 ScottwCode

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.