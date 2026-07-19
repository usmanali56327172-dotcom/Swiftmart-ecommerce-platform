SwiftMart — Full-Stack E-Commerce Platform
============================================

SwiftMart is a production-grade, full-stack e-commerce platform built to demonstrate
enterprise-level engineering practices across the entire stack: a Next.js 14 (App Router)
frontend, a Node.js/Express REST API, and a PostgreSQL database managed through Prisma ORM.
It was built as a complete Amazon-style shopping experience rather than a basic CRUD demo,
covering everything a real online store needs to operate.

On the customer side, SwiftMart offers a searchable and filterable product catalog with
categories and brands, detailed product pages with image galleries and customer reviews,
a wishlist, a side-by-side product comparison tool, and a persistent shopping cart with
server-computed totals and coupon support. Checkout supports four payment methods tailored
for the Pakistani market: credit/debit cards through Stripe, JazzCash mobile wallet payments
with a properly signed and verified transaction flow, manual bank transfer with an admin
verification workflow, and Cash on Delivery. Every order includes a real-time tracking
timeline from placement through delivery.

On the business side, an admin dashboard provides revenue and order analytics with charts,
low-stock inventory alerts, full product and category management with direct image uploads,
order status management, and coupon administration.

The platform is built with authentication and authorization using JWT access and refresh
tokens with rotation, bcrypt password hashing, and role-based route protection. The API is
fully documented with an OpenAPI/Swagger specification, validated end-to-end with Zod
schemas, and protected with rate limiting, Helmet, and centralized error handling. The
frontend is fully responsive across mobile, tablet, and desktop, supports dark mode, and
uses React Query for data fetching and Zustand for client state.

The project follows a clean, modular architecture with a clear separation between routes,
controllers, services, and validators on the backend, and reusable, typed components on the
frontend. It includes a Docker Compose setup for local development, a deployment guide for
Vercel and Railway, and complete setup documentation, making it a realistic reference for
how a modern e-commerce system is actually structured and shipped.
