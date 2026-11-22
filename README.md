# Snapzo Frontend part 

<img width="500" height="212" alt="image" src="https://github.com/user-attachments/assets/3f362136-e614-491e-b55c-66c6f15f0916" />


Snapzo is a React-based food ordering frontend built with Vite. Users can browse meals, add items to a cart, sign in, place orders with cash on delivery or Stripe, and view their previous orders.

## Features

- Browse food categories and available meals
- Add and remove items from the shopping cart
- User sign-in and token-based authentication
- Delivery information and order checkout
- Cash on delivery and Stripe payment options
- Order history and order verification
- Responsive layout with toast notifications

## Tech Stack

- React 19
- React Router
- Vite
- Axios
- React Toastify
- CSS

## Getting Started

### Prerequisites

- Node.js 18 or newer
- The Snapzo backend API running on `http://localhost:4000`

### Installation

```bash
git clone https://github.com/CoderNasim2023/Snapzo-frontend.git
cd Snapzo-frontend/frontend
npm install
```

### Run the development server

```bash
npm run dev
```

Open the local URL shown by Vite, usually `http://localhost:5173`.

## Available Scripts

| Command | Description |
| --- | --- |
| `npm run dev` | Start the development server |
| `npm run build` | Create a production build |
| `npm run preview` | Preview the production build |
| `npm run lint` | Run ESLint |

## Application Routes

| Route | Page |
| --- | --- |
| `/` | Home and food menu |
| `/cart` | Shopping cart |
| `/order` | Checkout and payment |
| `/myorders` | Order history |
| `/verify` | Order/payment verification |

## Backend Integration

The frontend uses `http://localhost:4000` as the backend base URL. Start the backend before using authentication, cart synchronization, food-list loading, or order placement.

```text
/api/food/list
/api/user/*
/api/cart/*
/api/order/*
```

## Project Structure

```text
frontend/
├── public/                 # Public assets
├── src/
│   ├── assets/             # Images and shared asset references
│   ├── components/         # Navbar, footer, pages, and UI components
│   ├── Context/            # Global cart, menu, and authentication state
│   ├── App.jsx             # Application routes and global UI
│   └── main.jsx            # React entry point
├── package.json
└── vite.config.js
```

## Production Build

```bash
npm run build
```

The optimized files are generated in `frontend/dist/`.
