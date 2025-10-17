<div align="center">

# 🛒 Quick Cart — E‑commerce Platform 🌐

**Quick Cart** is a modern, production-ready e‑commerce application built with Next.js and a server backend using Node/Express and MongoDB. It includes secure authentication, product and seller dashboards, checkout with Stripe, media management via Cloudinary, and a fast, responsive UI built with Tailwind CSS — ideal as a portfolio project or a lightweight production storefront.

[Live Demo](https://quick-cart-e-commerce-beryl.vercel.app/) • [Portfolio](https://harshkushwaha7x.github.io/Portfolio) • [GitHub](https://github.com/harshkushwaha7x/QuickCart-E-Commerce)

</div>

---

<p align="center">
  <a href="https://github.com/harshkushwaha7x/QuickCart-E-Commerce"><img src="https://img.shields.io/github/last-commit/harshkushwaha7x/QuickCart-E-Commerce?style=flat-square" alt="last commit"></a>
  <a href="https://github.com/harshkushwaha7x/QuickCart-E-Commerce"><img src="https://img.shields.io/github/languages/top/harshkushwaha7x/QuickCart-E-Commerce?style=flat-square" alt="languages"></a>
  <img src="https://img.shields.io/badge/license-MIT-blue?style=flat-square" alt="license" />
  <img src="https://img.shields.io/badge/version-1.0.0-success?style=flat-square" alt="version" />
</p>

---

## ✨ Highlights

- Secure authentication using Clerk (or replaceable auth provider).
- Seller & Buyer dashboards, product CRUD, and image uploads (Cloudinary).
- Cart, checkout flow, and Stripe payment integration (webhooks supported).
- Server-side APIs, server-rendered pages (Next.js app router), and efficient data modeling with Mongoose.
- CI/CD friendly: Vercel for frontend, Render/Railway for backend, MongoDB Atlas for the database.

---

## 📦 Features

- 🔐 Authentication (Clerk) & role‑based pages
- 📦 Product management (add, edit, delete, images)
- 🛒 Shopping cart & checkout (Stripe integration)
- 🧾 Order history & seller dashboard
- 📱 Fully responsive UI with Tailwind CSS
- 📸 Image uploads via Cloudinary
- ⚡ Fast builds with Next.js and Turbopack (where applicable)
- ✅ Basic input validation, error handling, and auth guards

---

## 🧩 Tech Stack

**Frontend:** Next.js, React, Tailwind CSS, Vite (dev tooling)  
**Backend:** Node.js, Express (or Next API), Inngest (background jobs), Mongoose (MongoDB)  
**Database:** MongoDB (Atlas recommended)  
**Media:** Cloudinary (image storage & CDN)  
**Payments:** Stripe (payment processing & webhooks)  
**Auth:** Clerk (replaceable with NextAuth/Auth0)  
**DevOps:** Vercel, Render/Railway, Docker (optional)

---

## 📁 Project Structure

```
/app (Next.js app router)
/components       # Reusable UI components
/config           # Config and helper utilities
/lib              # Utility functions
/models           # Mongoose models
/pages/api        # Serverless / API routes (if used)
/public/screenshots
/server           # Optional: express server, jobs, webhooks
/.env.example
```

---

## 🚀 Quick Start (Local)

> This assumes the repository name `QuickCart-E-Commerce` and the project uses a separate `client` (Next.js) and `server` or unified Next app. Adjust commands to your repo layout.

1. **Clone & install**
```bash
git clone https://github.com/harshkushwaha7x/QuickCart-E-Commerce.git
cd QuickCart-E-Commerce
npm install
```

2. **Create `.env`** — copy `.env.example` and provide real values:
```env
MONGO_URI=your_mongodb_connection_string
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
CLERK_PUBLISHABLE_KEY=pk_clerk_...
CLERK_SECRET_KEY=sk_clerk_...
STRIPE_PUBLISHABLE_KEY=pk_test_...
STRIPE_SECRET_KEY=sk_test_...
JWT_SECRET=your_jwt_secret
NEXT_PUBLIC_API_BASE_URL=http://localhost:3000
```

3. **Run locally**
```bash
npm run dev
# or, if client/server are separate:
# cd client && npm run dev
# cd server && npm run dev
```

4. **Open the app**
Visit `http://localhost:3000` (or the port specified by your Next.js app).

---

## 🔌 API Endpoints (examples)

> Replace `/api` with your configured API root if different.

**Auth & Users**
- `POST /api/auth/register` — register user (handled by Clerk)
- `GET /api/profile` — get user profile

**Products**
- `GET /api/products` — list products
- `GET /api/products/:id` — product details
- `POST /api/products` — create product (seller)
- `PUT /api/products/:id` — update product (seller)
- `DELETE /api/products/:id` — delete product (seller)

**Cart & Orders**
- `POST /api/cart` — add item to cart
- `POST /api/checkout` — create Stripe session / place order
- `GET /api/orders` — list user orders
- `POST /api/webhook/stripe` — Stripe webhook for payment events

---

## ☁️ Deployment

**Frontend (Vercel)**:
- Connect the GitHub repository to Vercel, set environment variables, and deploy.

**Backend (Render / Railway / Render)**:
- Deploy the backend service and set environment variables for DB, Stripe, and Cloudinary.

**Database**:
- Use MongoDB Atlas for production-grade managed database.

**Stripe Webhooks**:
- Configure webhook endpoint in your Stripe dashboard and secure it using the webhook secret in your server.

---

## 🖼️ Screenshots

Include screenshots in `/public/screenshots/` and reference them like:
```md
![Home UI](https://raw.githubusercontent.com/harshkushwaha7x/QuickCart-E-Commerce/main/public/screenshots/quick-cart-ecommerce.png)
![Seller Dashboard](https://raw.githubusercontent.com/harshkushwaha7x/QuickCart-E-Commerce/main/public/screenshots/seller-dashboard.png)
```

---

## ✅ Testing & Quality

- Use ESLint + Prettier (config recommended)
- Add unit tests for critical APIs and components (Jest/React Testing Library)
- Monitor errors with Sentry or an equivalent service (optional)

---

## 🤝 Contributing

Contributions are welcome — please follow this flow:

1. Fork the repository
2. Create a feature branch: `git checkout -b feat/awesome`
3. Commit changes: `git commit -m "Add awesome feature"`
4. Push and open a Pull Request

Please keep PRs small and include descriptive commit messages and screenshots for UI changes.

---

## 📄 License

This project is licensed under the **MIT License** — see [LICENSE](https://github.com/harshkushwaha7x/QuickCart-E-Commerce/blob/main/LICENSE) for details.

---

## 📬 Contact

**Harsh Kushwaha** — Developer & Maintainer  
- Portfolio: https://harshkushwaha7x.github.io/Portfolio  
- GitHub: https://github.com/harshkushwaha7x  
- LinkedIn: https://www.linkedin.com/in/harshkushwaha7x/  
- Email: harshkushwaha4151@gmail.com

---

<div align="center">
Made by **Harsh Kushwaha**
</div>
