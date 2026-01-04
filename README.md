# 🎸 Sound Signal Instruments - AI-Powered E-commerce Platform

[![Next.js](https://img.shields.io/badge/Next.js-App%20Router-000000?logo=nextdotjs)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-Server%20%26%20Client%20Components-61DAFB?logo=react&logoColor=black)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-Strict-3178C6?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Sanity](https://img.shields.io/badge/Sanity-CMS%20%2B%20App%20SDK-F03E2F?logo=sanity)](https://www.sanity.io/)
[![Clerk](https://img.shields.io/badge/Clerk-Auth%20%2B%20AgentKit-6C47FF?logo=clerk)](https://clerk.com/)
[![Stripe](https://img.shields.io/badge/Stripe-Payments-635BFF?logo=stripe&logoColor=white)](https://stripe.com/)
[![Vercel AI](https://img.shields.io/badge/Vercel-AI%20SDK-000000?logo=vercel)](https://vercel.com/ai)
[![Claude](https://img.shields.io/badge/Claude-AI%20Assistant-FFB000)](https://www.anthropic.com/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-v4-38BDF8?logo=tailwindcss)](https://tailwindcss.com/)
[![shadcn/ui](https://img.shields.io/badge/shadcn-ui-000000)](https://ui.shadcn.com/)
[![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey)](https://creativecommons.org/licenses/by-nc/4.0/)

### Next.js • Sanity • Clerk • Stripe • Vercel AI SDK • Claude / GPT

Sound Signal Instruments is an AI-powered, real-time **instrument e-commerce platform** showcasing modern full-stack patterns with authenticated AI agents, live inventory updates, and secure payments. Built as a production-ready reference for developers exploring AI-native commerce experiences.

---

## ✨ Overview

This project is a **modern instrument e-commerce store with a brain** 🧠 — combining real-time CMS updates, AI shopping assistance, and a powerful admin dashboard.

Shoppers can browse instruments, chat with AI, and securely check out.  
Admins get AI-powered insights, inventory alerts, and live content editing — all without page refreshes.

---

## 🖼️ Screenshots

### 🏠 Home & Product Discovery

| Home Page | Product Listing |
|---------|----------------|
| ![Home](public/screenshots/home.png) | ![Products](public/screenshots/products.png) |

### 🎵 Product & AI Assistance

| Product Detail | AI Shopping Assistant |
|---------------|----------------------|
| ![Product](public/screenshots/product.png) | ![AI Assistant](public/screenshots/ai-shopping-assistant.png) |

### 🛒 Cart & Checkout Flow

| Cart | Checkout |
|----|----------|
| ![Cart](public/screenshots/cart.png) | ![Checkout](public/screenshots/checkout.png) |

### ✅ Order Completion

| Order Confirmation | |
|-------------------|--|
| ![Order Confirmation](public/screenshots/order-confirmation.png) | |

---

## 🚀 Tech Stack

- **Next.js + React** — App Router, Server/Client Components, Server Actions  
- **Sanity CMS** — App SDK, GROQ, TypeGen, real-time mutations  
- **Clerk** — Authentication + AgentKit for AI user context  
- **Vercel AI SDK** — AI Gateway (Claude, GPT, Cohere)  
- **Stripe** — Payments, Checkout, Webhooks  
- **shadcn/ui + Tailwind CSS v4** — Accessible, modern UI  
- **Zustand** — Persisted cart state  
- **TypeScript** — End-to-end type safety  

---

## ⚡ Key Differentiators

- 🤖 AI Shopping Assistant with authenticated tools  
- 🔐 User-aware AI via Clerk AgentKit  
- ⚡ Real-time inventory & content (Sanity Live — no polling)  
- 🧠 AI Admin Dashboard powered by Claude  
- 💳 Stripe Checkout + Webhooks for order processing  
- 🛒 Persisted cart with stock validation  
- 🧩 Embedded Sanity Studio at `/studio`  

---

## 🧠 What Is This App?

Think of it as **an instrument store with an AI sales associate**.

### Customers can:
- 🛒 Browse & buy instruments with live stock updates  
- 🤖 Ask AI to find products, compare prices, or track orders  
- 📦 View order history when signed in  

### Store owners get:
- 📊 AI-generated sales insights & recommendations  
- ✏️ Real-time product & order editing  
- ⚠️ Low-stock alerts & fulfillment tracking  

---

## ✨ Features

### 🧍 For Shoppers

| Feature | Description |
|------|-------------|
| 🤖 AI Shopping Assistant | Natural-language product search & recommendations |
| 🛒 Smart Cart | Persisted cart with live inventory checks |
| 💳 Secure Checkout | Stripe-powered payments |
| 📦 Order Tracking | View orders when signed in |
| 🔄 Live Stock | Real-time inventory visibility |

---

### 🛠️ For Admins

| Feature | Description |
|------|-------------|
| 🧠 AI Insights | Claude-powered trends & action items |
| 📝 Product Management | Live editing via Sanity App SDK |
| 📋 Order Management | Paid → Shipped → Delivered |
| ⚠️ Inventory Alerts | Automatic low-stock warnings |
| 📊 Analytics | Revenue & order metrics |

---

## 🔧 Technical Highlights

| Feature | Technology | Why It Matters |
|------|-----------|---------------|
| ⚡ Real-time UI | Sanity Live + App SDK | Instant updates without refresh |
| 🔐 Authenticated AI | Clerk AgentKit | AI only sees signed-in user data |
| 🧠 AI Gateway | Vercel AI Gateway | Swap models easily |
| 🛒 Cart Persistence | Zustand + localStorage | Cart survives reloads |
| 🧩 Type Safety | TypeScript + TypeGen | CMS → frontend safety |

---

## 🚀 Step-by-Step Setup

### 1. Clone the Repository

```bash
git clone https://github.com/johnsonr84/ai-ecommerce-platform.git
cd ai-ecommerce-sanity-clerk
```

### 2. Install Dependencies

```bash
pnpm install
```

### 3. Set Up Environment Variables

```bash
cp .env.example .env.local
```

```env
# Sanity
NEXT_PUBLIC_SANITY_PROJECT_ID=Your_value_goes_here
NEXT_PUBLIC_SANITY_DATASET=Your_value_goes_here
NEXT_PUBLIC_SANITY_ORG_ID=Your_value_goes_here
SANITY_API_WRITE_TOKEN=Your_value_goes_here

# Clerk
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=Your_value_goes_here
CLERK_SECRET_KEY=Your_value_goes_here

# Stripe
STRIPE_SECRET_KEY=Your_value_goes_here
STRIPE_WEBHOOK_SECRET=Your_value_goes_here

# Vercel
AI_GATEWAY_API_KEY=Your_value_goes_here
```

⚠️ **Security Note:** Never commit `.env.local` to git.  
💡 Variables prefixed with `NEXT_PUBLIC_` are exposed to the browser.

---

### 4. Configure Sanity

- Go to https://sanity.io/manage  
- Create or select a project  
- Copy **Project ID** and **Dataset**  
- Create an **Editor API token**  

---

### 5. Configure Clerk

- Go to https://dashboard.clerk.com  
- Create a new application  
- Copy Publishable Key & Secret Key  

---

### 6. Configure Stripe

```bash
stripe listen --forward-to localhost:3000/api/webhooks/stripe
```

---

### 7. Configure AI Gateway

- Go to https://vercel.com → AI Gateway  
- Create an API key  
- Default model: **Claude Sonnet 4 / 4.5**  
- Swap providers in `lib/ai/shopping-agent.ts`

---

### 8. Generate Types & Import Data

```bash
pnpm typegen
npx sanity dataset import sample-data.ndjson
```

---

### 9. Start Development Server

```bash
pnpm dev
```

Open **http://localhost:3000** 🎉

---

## ✅ First Time Setup Checklist

- [ ] `.env.local` configured  
- [ ] Sanity project & dataset created  
- [ ] Clerk application created  
- [ ] Stripe CLI running  
- [ ] Sample data imported  
- [ ] Types generated  

---

## 👨‍💻 Author

**Robert Johnson**  
Full-Stack Software Engineer  
🌐 https://robertjohnsonportfolio.com  

---
