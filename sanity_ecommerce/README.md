# E-commerce Store – Sanity & Stripe

A modern e-commerce web application built with Next.js, React, Sanity CMS, and Stripe. Users can browse products, view product details, manage their shopping cart, and complete checkout using Stripe's hosted payment page.

## Screenshots
## Screenshots

### Home Page
![Home Page](./screenshots/sanity-ecommerce-main.png)

### Shopping Bag
![Shopping Bag](./screenshots/sanity-ecommerce-bag.png)

### Successful Order
![Successful Order](./screenshots/sanity-ecommerce-success.png)

## Features

- Browse products and view product details
- Product catalog managed with Sanity CMS
- Add and remove products from the shopping cart
- Increase and decrease product quantities
- Automatically calculate cart totals
- Stripe Checkout integration
- Hosted checkout page for secure test payments
- Success and cancellation pages after checkoutgit add
- Responsive user interface

## Technologies

- Next.js
- React
- JavaScript
- Sanity CMS
- Stripe Checkout
- Stripe.js
- Context API
- HTML5
- CSS3

## Payment Integration

The application integrates Stripe Checkout to handle the payment flow.

The checkout process includes:

1. Sending cart items to the backend API.
2. Creating a Stripe Checkout Session.
3. Redirecting the customer to Stripe's hosted checkout page.
4. Processing payments in Stripe Sandbox (Test Mode).
5. Redirecting the customer to the success or cancellation page.

**Note:** Stripe is configured in test mode. No real payments are processed.

## Getting Started

### 1. Clone the repository

```bash
git clone YOUR_REPOSITORY_URL
cd ecommerce-sanity-stripe
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment variables

Create a `.env` file in the project root:

```env
STRIPE_SECRET_KEY=your_stripe_secret_key
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=your_stripe_publishable_key
```

Add your own Stripe test API keys from your Stripe Dashboard.

### 4. Run the development server

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## Project Structure

```text
ecommerce-sanity-stripe/
├── components/
├── context/
├── lib/
├── pages/
│   └── api/
│       └── stripe.js
├── public/
├── sanity_ecommerce/
├── styles/
├── .env
├── .gitignore
├── package.json
└── README.md
```

## Future Improvements

- Implement Stripe webhooks for reliable payment confirmation.
- Add order history and order management.
- Improve checkout error handling.
- Deploy the application for production use.

## Author

**Rahima Baghirova**

[GitHub](https://github.com/Ragima2412) · [LinkedIn](https://www.linkedin.com/in/rahima-baghirova-a68132236/)
