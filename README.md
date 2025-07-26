# Shopping Cart Application

A modern e-commerce application built with React, TypeScript, and Material-UI. This application demonstrates a complete shopping experience with authentication, product browsing, cart management, and responsive design.

## Features

- 🛍️ **Product Browsing**

  - View products in a responsive grid layout
  - Search products by name
  - Filter by category and price range
  - Pagination support

- 🔐 **Authentication**

  - User registration and login
  - Protected routes
  - Persistent sessions

- 🛒 **Shopping Cart**

  - Add/remove products
  - Update quantities
  - Real-time cart updates
  - Persistent cart data

- 🎨 **UI/UX**

  - Responsive design
  - Dark/Light theme support
  - Modern and clean interface
  - Loading states and error handling
  - Mobile-friendly navigation

- 🔍 **Search & Filters**
  - Real-time search
  - Category filtering
  - Price range filtering
  - Clear filters option

## Technologies Used

- **React 18** - UI library
- **TypeScript** - Type safety
- **Material-UI (MUI)** - UI components
- **React Router DOM** - Client-side routing
- **TanStack React Query** - Data fetching and caching
- **Styled Components** - Component styling
- **Vite** - Build tool and dev server

## Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/shopping-cart.git
   cd shopping-cart
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Start the development server:

   ```bash
   npm run dev
   ```

4. Open [http://localhost:3000](http://localhost:3000) in your browser.

### Build for Production

```bash
npm run build
```

### Preview Production Build

```bash
npm run preview
```

## Project Structure

```
src/
├── components/         # Reusable components
│   ├── ErrorBoundary.tsx
│   ├── Filters.tsx
│   ├── Footer.tsx
│   ├── LoadingSpinner.tsx
│   └── Pagination.tsx
├── pages/             # Page components
│   ├── Landing.tsx
│   ├── Login.tsx
│   └── Signup.tsx
├── Cart/              # Cart components
│   ├── Cart.tsx
│   └── Cart.styles.ts
├── CartItem/          # Cart item components
│   ├── CartItem.tsx
│   └── CartItem.styles.ts
├── Header/            # Header component
│   └── Header.tsx
├── Item/              # Product item components
│   ├── Item.tsx
│   └── Item.styles.ts
├── assets/            # Static assets
├── App.tsx            # Main application component
├── App.styles.ts      # App styles
├── main.tsx           # Application entry point
├── ThemeContext.tsx   # Theme context
└── vite-env.d.ts      # Vite type definitions
```

## API Integration

The application uses the [Fake Store API](https://fakestoreapi.com/) for:

- **Products**: `GET /products` - Fetch all products
- **Authentication**: `POST /auth/login` - User login
- **Users**: `POST /users` - User registration

### Test Credentials

For testing purposes, you can use these credentials:

- Username: `mor_2314`
- Password: `83r5^_`

## Features in Detail

### Authentication Flow

1. Users can register with email, username, and password
2. Login with username and password
3. JWT token is stored in localStorage
4. Protected routes redirect to login if not authenticated

### Shopping Cart

1. Add products to cart from product grid
2. View cart in slide-out drawer
3. Update quantities with +/- buttons
4. Remove items or empty entire cart
5. View total price

### Product Filtering

1. Search by product name (real-time)
2. Filter by category (dropdown)
3. Filter by price range (slider)
4. Clear all filters option

### Responsive Design

- Mobile-first approach
- Collapsible filters on mobile
- Responsive grid layout
- Touch-friendly interface

## Deployment

### GitHub Pages

The project is configured for GitHub Pages deployment:

1. **Configure the repository name** in `vite.config.ts`:

   ```ts
   base: "/YOUR_REPOSITORY_NAME/";
   ```

2. **Deploy to GitHub Pages**:

   ```bash
   npm run deploy
   ```

3. **Enable GitHub Pages** in your repository settings:
   - Go to Settings > Pages
   - Source: Deploy from a branch
   - Branch: gh-pages
   - Folder: / (root)

**Note**: Make sure to replace `YOUR_REPOSITORY_NAME` with your actual repository name.

### Other Platforms

The application can be deployed to any static hosting service:

- Netlify
- Vercel
- AWS S3
- Firebase Hosting

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License.

## Acknowledgments

- [Fake Store API](https://fakestoreapi.com/) for providing the mock data
- [Material-UI](https://mui.com/) for the UI components
- [TanStack React Query](https://tanstack.com/query/latest) for data fetching and caching
- [React Router](https://reactrouter.com/) for client-side routing
