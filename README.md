# 🌌 Curated Boutique — Premium Full-Stack E-Commerce Experience

[![Vite](https://img.shields.io/badge/Vite-6.x-646CFF?logo=vite&logoColor=white)](https://vite.dev/)
[![React](https://img.shields.io/badge/React-19.0-61DAFB?logo=react&logoColor=black)](https://react.dev/)
[![Express](https://img.shields.io/badge/Express-4.x-000000?logo=express&logoColor=white)](https://expressjs.com/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4.x-38B2AC?logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![Gemini AI](https://img.shields.io/badge/Gemini_AI-2.5_/_3.5-blue?logo=google-gemini&logoColor=white)](https://ai.google.dev/)

Welcome to **Curated Boutique**, an ultra-premium, full-stack digital shopfront designed for tech-forward professionals, minimalist desk architects, and design connoisseurs. Engineered with an absolute obsession for fluid transitions, high-contrast typography, and intuitive administrative control.

---

## 🎨 Immersive Virtual Shopfront

<div align="center">
  <img src="https://images.unsplash.com/photo-1513151233558-d860c5398176?auto=format&fit=crop&w=1200&q=80" alt="Curated Boutique Workspace Concept" width="100%" style="border-radius: 12px; margin-bottom: 20px; box-shadow: 0 10px 30px rgba(0,0,0,0.15);" />
  
  *Designing the ultimate digital workspace with hand-picked physical artifacts.*
</div>

---

## ✨ Features & Architecture

### 🛍️ Client & Customer Experience
- **Fluid Grid Interface**: Built on a modular Swiss layout using Tailwind CSS, featuring subtle hover expansions and micro-interactions powered by `motion` (Framer Motion).
- **Gemini AI Smart Picks**: Fully integrated with the Google GenAI SDK. If a model encounters a high-demand limit, our API automatically heals, cycling through redundant high-performing candidates (`gemini-2.5-flash`, `gemini-1.5-flash`, `gemini-3.5-flash`, `gemini-flash-latest`) to secure smart product recommendations.
- **Dynamic Context Search & Filters**: Search, browse, and filter items by price ranges, high ratings, categories, and inventory instantly.
- **Smart Shopping Bag**: Seamless checkout pipeline with live total computation, visual item counters, and flexible cart actions.
- **Flexible Checkout Flow**: Supports standard secure integration. If your `STRIPE_SECRET_KEY` is not present, the app gracefully deploys a gorgeous, fully responsive checkout simulator.

### ⚙️ Admin Control Center (Power Dashboard)
- **JWT Secured Login**: Restricts entry using high-entropy passwords secured through industrial-grade salt-and-hash algorithms (`bcryptjs`) and secure `jsonwebtoken` cookies.
- **Real-Time Catalog Management**: Full CRUD capabilities to instantly create new products, adjust inventory counts, update descriptions, and replace Unsplash high-resolution URLs.
- **Dynamic Database Healing**: Our backend system automatically backfills missing catalog records on startup so that your workspace remains fully healthy and updated.
- **Interactive Analytics**: Monitor sales, overall reviews, average ratings, low-stock warnings, and hot-selling categories directly from a high-contrast panel.

---

## 🛠️ Technology Stack

| Layer | Technology | Purpose |
| :--- | :--- | :--- |
| **Frontend UI** | React 19, Motion, Lucide Icons | Responsive SPA layout, tactile buttons, fluid transitions |
| **Backend Server** | Express v4, TSX Runtime | High-speed REST APIs, secure API proxies, static file delivery |
| **AI Integration** | `@google/genai` (SDK v2) | Contextual product recommendations based on shopping history |
| **Authentication** | BcryptJS, JWT | Salt-and-hash credentials, signed cookie session handshakes |
| **Styling Engine** | Tailwind CSS v4, Inter, JetBrains Mono | Global theme definitions, high-contrast typography pairings |
| **Build Compiler** | Vite, ESBuild | Blazing-fast bundler, clean ES module path resolution |

---

## 🚀 Getting Started Locally

### Prerequisites
Make sure you have **Node.js** (v18 or higher) installed.

### 1. Clone & Install Dependencies
Navigate to your project root folder and execute:
```bash
npm install
```

### 2. Configure Environment Variables
Create a `.env` (or `.env.local` for development) in your root directory. Copy the values from `.env.example`:
```ini
# Required for AI personalized recommendations
GEMINI_API_KEY="your_api_key_here"

# Required for signing JWT session tokens
JWT_SECRET="your_high_entropy_secret_passphrase"

# Optional: Stripe Payment Gateway configuration
STRIPE_SECRET_KEY="sk_test_..."
```

### 3. Run the Development Server
Fire up the local dual-layer Express + Vite compiler:
```bash
npm run dev
```
Open your browser to [http://localhost:3000](http://localhost:3000) to view the workspace!

### 4. Build for Production
To bundle assets and compile the server-side architecture into a unified target format:
```bash
npm run build
npm start
```

---

## 🔑 Administrative Access

To experience the Admin Dashboard and customize your store catalog:
- **Default Username**: `admin`
- **Default Password**: `admin123`

---

## 💡 Aesthetic Style Notes
- **Inter** is mapped as the primary UI font, ensuring supreme readability and structure.
- **JetBrains Mono** is embedded for analytical metrics, currency tickers, and technical details.
- Standard borders and grids feature clean, modern neutral lines (`border-neutral-100`) to create a calm, eye-safe environment.

Enjoy configuring your ultra-premium **Curated Boutique**! 🌌
