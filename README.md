# Sri Murugen Nursery Garden — E-Commerce Website

## 🌿 Overview

A complete, production-ready single-file e-commerce website for **Sri Murugen Nursery Garden**, built with React. No server or database required — runs entirely in the browser using `localStorage` for persistence.

---

## ✅ Features Included

| Feature | Status |
|---|---|
| Public product catalog (browse without login) | ✅ |
| User signup & login | ✅ |
| Add to cart (login required) | ✅ |
| Cart drawer with quantity control | ✅ |
| Checkout with order placement | ✅ |
| My Orders page | ✅ |
| Admin dashboard (separate login) | ✅ |
| Admin: Add / Edit / Delete products | ✅ |
| Admin: Upload product photos | ✅ |
| Admin: Show/hide products | ✅ |
| Admin: View all orders | ✅ |
| Admin: Confirm orders | ✅ |
| Admin: View registered customers | ✅ |
| Contact page with WhatsApp / Email / Map | ✅ |
| Contact form | ✅ |
| Google Maps embed | ✅ |
| Mobile responsive design | ✅ |
| 12 pre-loaded sample plants | ✅ |
| Toast notifications | ✅ |
| Product detail modal | ✅ |
| Search & category filter | ✅ |

---

## 🚀 Deployment Options

### Option 1: Open Directly (Zero Setup)
Just double-click `index.html` in your file manager. The website works instantly in any modern browser.

### Option 2: Deploy to Netlify (Recommended for public access)
1. Go to [netlify.com](https://netlify.com) and create a free account
2. Drag and drop the `index.html` file onto the Netlify dashboard
3. Your website goes live instantly with a free URL like `https://sri-murugen.netlify.app`

### Option 3: Deploy to GitHub Pages
1. Create a GitHub repository
2. Upload `index.html`
3. Go to Settings → Pages → Source: `main` branch
4. Website is live at `https://yourusername.github.io/repo-name`

### Option 4: WhatsApp Hosting / Simple Web Host
Upload `index.html` to any web host (Hostinger, Bluehost, etc.) in the `public_html` folder.

---

## 🔐 Admin Access

| Field | Value |
|---|---|
| Email | `admin@srimurugen.com` |
| Password | `Admin@2024!` |

> **To change admin credentials:** Open `index.html` in a text editor and find the line:
> ```js
> const ADMIN_CREDENTIALS = { email: 'admin@srimurugen.com', password: 'Admin@2024!' };
> ```
> Replace with your preferred email and password.

---

## 👤 User Registration

Customers register directly on the website. Their details (name, email, phone, password) are stored in `localStorage` in the browser.

> ⚠️ **Note on passwords:** For this single-file deployment, passwords are stored in plain text in localStorage. This is acceptable for a small local business site. For a production app with a backend server, upgrade to a hashed password system (bcrypt, etc.).

---

## 📦 Data Storage

All data is stored in the visitor's browser `localStorage`:

| Key | Contents |
|---|---|
| `smn_products` | All plant products |
| `smn_users` | Registered customers |
| `smn_orders` | All placed orders |
| `smn_cart` | Current cart |
| `smn_user` | Logged-in user |
| `smn_admin` | Admin session flag |

> **Data persists** between page refreshes and browser restarts. Data is per-browser — different devices have separate data.

---

## 🌿 Adding Products (Admin)

1. Login with admin credentials
2. Go to **Admin → Products**
3. Click **+ Add Plant**
4. Fill in: name, category, price, description, care details, emoji icon
5. Upload a plant photo (optional)
6. Click **Save Plant**

---

## 📞 Contact Details Configured

| Contact | Value |
|---|---|
| WhatsApp | +91 9566617816 |
| Email | nanthacpm99@gmail.com |
| Maps Link | https://maps.app.goo.gl/BDS1a8edxPZ1AgiB7 |

To update these, search for the phone number or email in `index.html` and replace all occurrences.

---

## 📱 WhatsApp Order Flow

When a customer places an order:
1. Order is saved to admin dashboard
2. Customer is shown a success screen with a **WhatsApp link** to contact the nursery
3. Admin can confirm orders from the Orders panel

---

## 🎨 Customisation Guide

| What to change | Where in index.html |
|---|---|
| Business name | Search `Sri Murugen` |
| Admin credentials | `ADMIN_CREDENTIALS` constant |
| Sample plants | `SAMPLE_PLANTS` array |
| WhatsApp number | Search `9566617816` |
| Email | Search `nanthacpm99` |
| Maps link | Search `maps.app.goo.gl` |
| Colors | `:root` CSS variables |

---

## 🛠 Tech Stack

- **React 18** (loaded via CDN — no npm required)
- **Babel Standalone** (JSX transpilation in browser)
- **Google Fonts** (Playfair Display + DM Sans)
- **localStorage** (all data persistence)
- No backend server required
- No database required
- No build step required

---

## 📋 Order Management

Orders flow:
1. Customer adds plants to cart → places order
2. Order appears in Admin → Orders with status **Pending**
3. Admin clicks **✅ Confirm** to mark as confirmed
4. Customer is encouraged to follow up via WhatsApp

---

*Built for Sri Murugen Nursery Garden, Nagapattinam.*
