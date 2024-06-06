
# Project E-commerce

## Introduction
Project E-commerce is an online marketplace platform designed to facilitate the buying and selling of products. The app allows users to browse a wide range of products, add them to their shopping cart and place orders safely and efficiently. The goal is to provide a seamless and accessible user experience for buyers, with robust management features.
 
## Models

### User
Represents registered users on the platform, who can be buyers or sellers.

- **Attributes:**
 - `id`: Unique identifier of the user.
 - `name`: Name of the user.
 - `email`: User's email address.
 - `password`: User's encrypted password.
 - `address`: User's shipping address.
 - `type`: Type of user (buyer or seller).

### Product
Represents the products available for sale on the platform.

- **Attributes:**
 - `id`: Unique identifier of the product.
 - `name`: Name of the product.
 - `description`: Detailed description of the product.
 - `price`: Price of the product.
 - `stock`: Available quantity of the product.
 - `category`: Category to which the product belongs.
 - `vendedorId`: Identifier of the seller who offers the product.

### Order
Represents the orders placed by users on the platform.

- **Attributes:**
 - `id`: Unique identifier of the order.
 - `userId`: Identifier of the user who placed the order.
 - `date`: Date on which the order was placed.
 - `total`: Total amount of the order.
 - `status`: Status of the order (pending, shipped, delivered, cancelled).

###OrderDetail
Represents the details of each product in a specific order.

- **Attributes:**
 - `id`: Unique identifier of the order detail.
 - `orderId`: Identifier of the order to which this detail belongs.
 - `productId`: Product identifier.
 - `quantity`: Quantity of products in this detail.
 - `price`: Price of the product at the time of placing the order.

### Category
Represents product categories to facilitate navigation and search.

- **Attributes:**
 - `id`: Unique identifier of the category.
 - `name`: Name of the category.
 - `description`: Description of the category.

### Review
Represents the reviews and ratings that users can leave about products.

- **Attributes:**
 - `id`: Unique identifier of the review.
 - `productId`: Identifier of the reviewed product.
 - `userId`: Identifier of the user who made the review.
 - `rating`: Product rating (1-5 stars).
 - `comment`: User comment about the product.
 - `date`: Date on which the review was made.

### Prerequisites
- Node.js (v16 recommended)
- npm

### Steps
```bash
git clone https://github.com/yourusername/project_ecommerce.git
cd project_ecommerce
npm install
npm start

# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
