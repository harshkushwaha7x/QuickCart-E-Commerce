<div align="center">

# 🛒 Quick Cart — E‑commerce Platform 🌐

**Quick Cart** is a modern, production-ready e‑commerce application built with Next.js and a server backend using Node/Express and MongoDB. It includes secure authentication, product and seller dashboards, checkout with Stripe, media management via Cloudinary, and a fast, responsive UI built with Tailwind CSS — ideal as a portfolio project or a lightweight production storefront.

[Live Demo](https://quick-cart-e-commerce-beryl.vercel.app/) • [Portfolio](https://harshkushwaha7x.github.io/Portfolio) • [GitHub](https://github.com/harshkushwaha7x/QuickCart-E-Commerce)

</div>

---

<p align="center">
  <a href="https://github.com/harshkushwaha7x/QuickCart-E-Commerce"><img src="https://img.shields.io/github/last-commit/harshkushwaha7x/QuickCart-E-Commerce?style=flat-square" alt="last commit"></a>
  <a href="https://github.com/harshkushwaha7x/QuickCart-E-Commerce"><img src="https://img.shields.io/github/languages/top/harshkushwaha7x/QuickCart-E-Commerce?style=flat-square" alt="languages"></a>
  <a href="https://github.com/harshkushwaha7x/QuickCart-E-Commerce/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue?style=flat-square" alt="license" /></a>
  <img src="https://img.shields.io/badge/version-1.0.0-success?style=flat-square" alt="version" />
</p>

---

## ✨ Summary

Quick Cart provides a complete starter e‑commerce platform: user authentication, seller & buyer dashboards, product CRUD, cart & checkout with Stripe, image uploads via Cloudinary, and deploy-ready configuration for Vercel/Render. It’s perfect as a portfolio project to demonstrate full-stack, cloud, and payment integration skills.

---

## 📦 Highlights & Use Cases

- Developer portfolio demo or starter store for small businesses.  
- Demonstrates end‑to‑end flow: authentication → product management → checkout → order history.  
- CI/CD friendly and easy to deploy on modern platforms (Vercel + Render).

---

## 🚀 Features

- 🔐 Authentication (Clerk) & role‑based pages (buyer/seller)  
- 📦 Product management (create, read, update, delete, images)  
- 🛒 Shopping cart & checkout using Stripe (session + webhook handling)  
- 🧾 Order history & seller dashboard with sales overview  
- 📱 Mobile‑first responsive UI with Tailwind CSS  
- 📸 Image uploads via Cloudinary + CDN delivery  
- ⚡ Fast builds with Next.js and modern tooling  
- ✅ Input validation, auth guards, and basic error handling

---

## 🧩 Tech Stack

**Frontend:** Next.js, React, Tailwind CSS  
**Backend:** Node.js, Express / Next API routes, Inngest (background jobs)  
**Database:** MongoDB (Atlas recommended)  
**Media:** Cloudinary  
**Payments:** Stripe (webhooks)  
**Auth:** Clerk (can swap with NextAuth/Auth0)  
**DevOps:** Vercel (frontend), Render/Railway (backend), Docker (optional)

---

## 📁 Project Structure (high-level)

```
/app                     # Next.js app router (UI & pages)
/components              # Reusable UI components
/config                  # Config & helpers (db, cloudinary, stripe)
/lib                     # Utility functions
/models                  # Mongoose models
/pages/api               # API routes / server functions
/public/screenshots      # Demo screenshots referenced in README
/server                  # Optional express server / background jobs
/.env.example            # Example env variables
```

---

## 🛠️ Quick Start (Local)

1. **Clone & install**
```bash
git clone https://github.com/harshkushwaha7x/QuickCart-E-Commerce.git
cd QuickCart-E-Commerce
npm install
```

2. **Environment** — copy `.env.example` to `.env` and add your keys:
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

3. **Run**
```bash
npm run dev
# or if split into client/server:
# cd client && npm run dev
# cd server && npm run dev
```

4. **Open**: http://localhost:3000

---

## 🔌 API Endpoints (examples)

**Auth & Users**
- `GET /api/profile` — user profile (auth required)

**Products**
- `GET /api/products`  
- `GET /api/products/:id`  
- `POST /api/products` (seller)  
- `PUT /api/products/:id` (seller)  
- `DELETE /api/products/:id` (seller)  

**Cart & Orders**
- `POST /api/cart` — add item to cart
- `POST /api/checkout` — create Stripe session / place order
- `GET /api/orders` — list user orders
- `POST /api/webhook/stripe` — Stripe webhook for payment events

---

## 🖼️ Screenshots

<div align="center">

### 🏠 Home UI  
<img src="https://raw.githubusercontent.com/harshkushwaha7x/QuickCart-E-Commerce/main/public/screenshots/quick-cart-ecommerce.png" alt="Quick Cart - Home" width="700" />

### 📊 Seller Dashboard  
<img src="https://raw.githubusercontent.com/harshkushwaha7x/QuickCart-E-Commerce/main/public/screenshots/seller-dashboard.png" alt="Quick Cart - Seller Dashboard" width="700" />

</div>

---

## ✅ Testing & Quality

- Use ESLint + Prettier for consistent formatting.  
- Add unit and integration tests (Jest, React Testing Library).  
- Consider runtime monitoring with Sentry for production.

---

## 🤝 Contributing

Contributions are welcome — please follow this flow:

1. Fork repository.
2. Create a feature branch: `git checkout -b feat/awesome`.
3. Commit & push: `git commit -m "feat: add ..." && git push`.
4. Open a Pull Request with a clear description and screenshots for UI changes.

Include small, focused PRs and keep the README updated for any new features.

---

## 📄 License

This project is licensed under the **MIT License** — see [LICENSE](https://github.com/harshkushwaha7x/QuickCart-E-Commerce/blob/main/LICENSE).

---

## 📬 Contact

**Harsh Kushwaha** — Developer & Maintainer  
- Portfolio: https://harshkushwaha7x.github.io/Portfolio  
- GitHub: https://github.com/harshkushwaha7x/QuickCart-E-Commerce  
- LinkedIn: https://www.linkedin.com/in/harshkushwaha7x/  
- Email: harshkushwaha4151@gmail.com

---

<div align="center">
Made by <b>Harsh Kushwaha</b>
</div>
