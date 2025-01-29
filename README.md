# Vue E-Commerce Application

This project is a **full-stack e-commerce application** designed as a clone of **Alibaba**, one of the world’s largest online marketplaces. It allows users to browse products, add them to their cart, and securely complete purchases. Built with modern web technologies like **Vue.js**, **Nuxt.js**, **Pinia**, and **Supabase**, the app provides a responsive, user-friendly shopping experience. The integration of **Stripe** enables secure and reliable payment processing.

## Live Demo

You can try out the deployed version of the application here:  
[**Live Project Demo**](https://vue-ecommerce-app-arman-wain.vercel.app)

You can use the following test card for payments:
<br/>
**4242 4242 4242 4242**

For the rest of the payment form, you can enter any information you like.

## Tech Stack

- **Vue.js**: Progressive JavaScript framework for building the user interface
- **Nuxt.js**: Vue.js framework for server-side rendering and static site generation
- **Pinia**: State management for Vue.js
- **Stripe**: Payment processing system
- **Supabase**: Backend-as-a-Service (BaaS) for authentication, database, and storage
- **Tailwind CSS**: Utility-first CSS framework for responsive design

## Prerequisites

Make sure you have the following installed on your machine:

- [Git](https://git-scm.com/)
- [Node.js](https://nodejs.org/en)
- [npm](https://www.npmjs.com/)

## Installation Steps

Follow these instructions to set up and run the project locally.

1. **Clone the repository**:

   Start by cloning the repository to your local machine:

   ```
   git clone https://github.com/ArmanWain/vue-ecommerce-app.git
   cd vue-ecommerce-app
   ```

2. **Configure environment variables**:

   Create a new file named `.env` in the root of your project and add the following content:

   ```
   STRIPE_PK_KEY=your_stripe_public_key
   STRIPE_SK_KEY=your_stripe_secret_key

   SUPABASE_URL=your_supabase_url
   SUPABASE_KEY=your_supabase_key

   DATABASE_URL=your_database_url
   ```

   Make sure to replace the placeholders with your actual credentials.

3. **Set Up Google OAuth**:
   To enable Google OAuth for authentication, follow the instructions here:
   [Set up Google OAuth with Supabase](https://supabase.com/docs/guides/auth/social-login/auth-google).

4. **Install dependencies**:

   Next, install the necessary dependencies:

   ```
   npm i
   ```

5. **Seed the Database**:

   Run the following commands to add products to the database:

   ```
   npx prisma generate
   npx prisma migrate dev --name init
   ```

6. **Run the project**:

   Finally, start the development server to run the project locally:

   ```
   npm run dev
   ```

   You can now go to http://localhost:3000/ to view the app.
