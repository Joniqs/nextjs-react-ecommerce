# Next.js React eCommerce

This is a sample eCommerce project built with Next.js and React. It provides a starting point for creating your own eCommerce website or online store.

## Features

- Content created with sanity.io
- Product catalog with search and filtering
- Shopping cart functionality
- Checkout process with payment integration
- Order management for administrators
- Responsive design for mobile and desktop devices

## Installation

1. Clone the repository:

   ```shell
   git clone https://github.com/Joniqs/nextjs-react-ecommerce.git
   ```

2. Navigate to the project directory:
   ```shell
   cd nextjs-react-ecommerce
   ```
3. Install the dependencies:
   ```shell
   npm install
   ```
4. Set up environment variables:  
    Create a .env.local file in the root directory and add the following variables:

   ```shell
   NEXT_PUBLIC_SANITY_TOKEN = 'your-sanity-token'
   NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY = 'your-stripe-publishable-key'
   NEXT_PUBLIC_STRIPE_SECRET_KEY = 'your-stripe-secret-key'
   ```

   These two are optional if you don't want to use them, delete them from here and pages/api/stripe.js

   ```shell
   NEXT_PUBLIC_SHIPPING_RATE_FREE = 'your-shipping-rate-free'
   NEXT_PUBLIC_SHIPPING_RATE_FAST = 'your-shipping-rate-fast'
   ```

5. Start the development server:

   ```shell
   npm run dev
   ```

   The application will be running at http://localhost:3000.

## Sanity CMS Setup:

The sanity folder contains the Sanity CMS setup for managing your eCommerce data. Follow these steps to set it up:

- Navigate to the sanity folder:

  ```shell
  cd sanity
  ```

- Install the Sanity CLI globally:

  ```shell
  npm install -g @sanity/cli
  ```

- Log in to Sanity:

  ```shell
  sanity login
  ```

If you don't have a Sanity account, you'll need to create one.

- Initialize the Sanity project:

  ```shell
  sanity init
  ```

  This will guide you through the setup process and create a new Sanity project.

- Start Sanity Studio

  ```shell
  sanity start
  ```

  You can now use Sanity Studio to manage your eCommerce data.

## Deployment

To deploy the application to a production environment, follow the Next.js deployment guide: https://nextjs.org/docs/deployment

Remember to put

    npm install --legacy-peers-dep

on install when deploying!

## Contributing

Contributions are welcome! If you find any issues or want to enhance the project, feel free to open a pull request.

## License

This project is licensed under the MIT License.
