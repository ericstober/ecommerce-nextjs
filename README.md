# Ecommerce Next.js

A modern, full stack ecommerce web application built with Next.js, Prisma, Tailwind Css, and Stripe. This project serves as a foundational template for developing scalable and performant online stores.

## Features

- **Next.js** with the App Router architecture
- **Prisma ORM** for type-safe database interactions
- **Tailwind CSS** for rapid UI devlopment
- **Stripe** integration for secure payment processing
- **TypeScript** for enhanced code reliability
- Responsive and accessible design
- Optimized for SEO and performance

## Tech Stack

- **Framework:**: Next.js
- **Database**: Prisma
- **Styling**: Tailwind CSS
- **Payments**: Stripe
- **Language**: TypeScript

## Getting Started

### Prerequisites

- Node.js
- Package manager
- Stripe account for payment integration

### Installation

1. Clone the repository

```bash
git clone https://github.com/ericstober/ecommerce-nextjs.git
cd ecommerce-nextjs
```

2. Install dependencies

```bash
npm install
```

3. Set up environment variables
   Create a `.env` in the root directory and add the following:

```env
DATABASE_URL=your_database_url
STRIPE_SECRET_KEY=your_stripe_secret_key
STRIPE_PUBLIC_KEY=your_stripe_public_key
```

4. Set up the database

```bash
npx prisma migrate dev --name init
```

5. Run the development server

```bash
npm run dev
```

Open http://localhost:3000 with your web browser to see the application.

## Project Structure

```
├── prisma/             # Prisma schema and migrations
├── src/
│   ├── app/            # Next.js App Router pages
│   ├── components/     # Reusable UI components
│   ├── lib/            # Utility functions and libraries
│   └── styles/         # Tailwind CSS configurations
├── .env                # Environment variables
├── next.config.mjs     # Next.js configuration
├── tailwind.config.ts  # Tailwind CSS configuration
└── tsconfig.json       # TypeScript configuration
```

## Stripe Integration

This project integrates Stripe for handling payments. Ensure you have a Stripe account and have set the `STRIPE_SECRET_KEY` and `STRIPE_PUBLIC_KEY` in your `.env` file.

For testing purposes, you can use Stripe's test card numbers. Refer to Stripe's testing documentation for more information.

## License

This project is licensed under the MIT License.
