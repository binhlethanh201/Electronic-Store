# React Electronic Store Management

This repository contains a modern React electronic store management application built with React Bootstrap for UI components and JSON Server for backend simulation. The app features a complete e-commerce experience including product browsing, category and brand filtering, product detail viewing, and product management capabilities. It demonstrates React component architecture, state management, RESTful API integration, and responsive design for a modern electronic store management platform.

## Prerequisites

- Node.js and npm installed on your system
- A modern web browser (Chrome, Firefox, Edge, Safari, etc.)
- (Optional) A code editor like VS Code, Sublime Text, or Atom for easier code navigation

## Installation

1. **Clone the repository** (if not already downloaded):
   ```sh
   git clone <repository-url>
   cd Electronic-Store-main
   ```
2. **Install dependencies**:
   ```sh
   npm install
   ```

## How to Run

1. **Start the JSON Server** (backend simulation):
   ```sh
   npx json-server --watch database.json --port 9999
   ```

2. **Start the React development server** (in a new terminal):
   ```sh
   npm start
   ```

This will open the app in your default browser at [http://localhost:3000](http://localhost:3000). The main page displays the products catalog with filtering options, and you can click on any product to view its detailed information. The page will reload automatically when you make changes to the source code.

**Note**: Make sure both the JSON Server (port 9999) and React development server (port 3000) are running simultaneously for the application to work properly.

## Project Structure

```
Electronic-Store-main/
├── database.json
├── public/
│   ├── images/
│   │   ├── iphone9.webp
│   │   ├── iphonex.jpeg
│   │   ├── samsunguniverse9.jpeg
│   │   ├── oppf19.png
│   │   ├── huaweip30.png
│   │   ├── macbook.jpeg
│   │   ├── samsungbook.jpeg
│   │   ├── sureface.jpeg
│   │   └── ...
│   ├── index.html
│   ├── manifest.json
│   └── robots.txt
├── src/
│   ├── components/
│   │   ├── index.jsx
│   │   └── detail.jsx
│   ├── App.js
│   └── index.js
├── package.json
├── package-lock.json
└── README.md
```

- **database.json**: Mock database containing products, categories, and brands for the JSON Server.
- **public/**: Contains static assets and the HTML template.
  - `images/`: Product images for the electronic store catalog.
  - `index.html`: The main HTML file loaded by React.
  - `manifest.json`, `robots.txt`: Standard web app metadata and configuration.
- **src/**: Contains the React source code.
  - `components/`: Reusable React components for different sections of the app.
    - `index.jsx`: Main product catalog component with browsing, filtering by category and brand, and product card display.
    - `detail.jsx`: Product detail component displaying comprehensive product information with delete functionality.
  - `App.js`: Main application component that sets up routing and renders the electronic store interface.
  - `index.js`: Entry point that renders the React app.
- **package.json**: Project metadata and dependencies including React, React Bootstrap, React Router, and JSON Server.
- **README.md**: Project documentation (this file).

## Features

- **Product Catalog**: Display electronic products in a clean card format with comprehensive details including title, price, discount, rating, and stock information
- **Category Filtering**: Filter products by specific categories (smartphones, laptops, etc.) using radio button selection
- **Brand Filtering**: Filter products by specific brands (Apple, Samsung, Huawei, etc.) using radio button selection
- **Product Details**: View detailed product information including description, pricing with discount calculations, ratings, and stock levels
- **Product Management**: Delete products from the catalog with confirmation dialogs
- **Responsive Design**: Modern, responsive interface built with Bootstrap for optimal viewing on all devices
- **Real-time Updates**: Dynamic data updates with JSON Server backend simulation
- **Interactive UI**: Clean card-based layout with hover effects and action buttons
- **Navigation**: Easy navigation between product catalog and individual product details
- **Image Display**: High-quality product images with proper styling and responsive design

## Data Structure

The application manages the following data entities:

- **Products**: Product items with id, title, description, price, discountPercentage, rating, stock, brand, category, and image
- **Categories**: Product categories with id and name for filtering
- **Brands**: Product brands with id and name for filtering

## Technologies Used

- **React 18.2.0**: Modern React with hooks and functional components
- **React Bootstrap 2.10.2**: Bootstrap components built for React
- **Bootstrap 5.3.3**: CSS framework for responsive design and UI components
- **React Router DOM 6.13.0**: Client-side routing for navigation
- **JSON Server 0.17.3**: Mock REST API backend for development
- **React Scripts 5.0.1**: Development and build tools
- **Axios 1.6.7**: HTTP client for API requests

## API Endpoints

The application uses the following API endpoints:

### Local JSON Server
- `GET /product` - Retrieve all products
- `GET /product/:id` - Retrieve specific product by ID
- `DELETE /product/:id` - Delete specific product by ID
- `GET /category` - Retrieve all categories
- `GET /brand` - Retrieve all brands

## Features in Detail

### Product Catalog Management (`index.jsx`)
- Displays products in responsive card layout with comprehensive product information
- Category-based filtering with radio button selection
- Brand-based filtering with radio button selection
- Product cards with hover effects and smooth transitions
- Product images with proper styling and responsive design
- Real-time data updates with JSON Server integration
- Responsive design with Bootstrap styling
- Clean and intuitive user interface

### Product Detail Management (`detail.jsx`)
- Displays comprehensive product information in a detailed view
- Product images with large display format
- Complete product details including description, pricing, and specifications
- Discount calculation and display of original vs. discounted prices
- Product deletion functionality with confirmation dialogs
- Navigation back to product catalog
- Responsive layout with proper spacing and typography

### Product Information Displayed

Each product includes comprehensive information:
- **Basic Details**: ID, title, description, and image
- **Pricing Information**: Original price, discount percentage, and calculated new price
- **Product Metrics**: Rating and stock availability
- **Categorization**: Brand and category classification for filtering

### Filtering and Navigation Features

The application provides intuitive filtering and navigation:
- **Category Filtering**: Radio button selection to filter products by category
- **Brand Filtering**: Radio button selection to filter products by brand
- **Combined Filtering**: Apply both category and brand filters simultaneously
- **Product Navigation**: Click on product cards to view detailed information
- **Responsive Layout**: Card-based design that adapts to different screen sizes
- **Back Navigation**: Easy return to product catalog from detail view

### Product Management Features

The application provides product management capabilities:
- **Product Deletion**: Remove products from the catalog with confirmation
- **Data Persistence**: All changes are reflected in the JSON Server database
- **Error Handling**: Proper error handling for failed operations
- **User Confirmation**: Confirmation dialogs for destructive actions

## User Experience Flow

1. **Product Browsing**: Users view all available electronic products in a clean card format
2. **Category Filtering**: Users can filter products by specific categories using radio buttons
3. **Brand Filtering**: Users can filter products by specific brands using radio buttons
4. **Product Details**: Users can click on product cards to view detailed product information
5. **Product Management**: Users can delete products with confirmation dialogs
6. **Navigation**: Users can easily navigate between product catalog and detail views
7. **Data Persistence**: All changes are saved to the JSON Server database

## Development Notes

- The application uses JSON Server for local data management and API simulation
- React hooks (useState, useEffect) manage component state and side effects
- React Router handles navigation between different views
- Bootstrap provides responsive design and card/table styling
- Fetch API handles all HTTP requests to the local JSON Server
- Component-based architecture ensures maintainable and scalable code
- Form validation ensures data integrity before operations
- Hover effects and transitions enhance user experience

## Learn More

- [React Documentation](https://reactjs.org/)
- [React Bootstrap Documentation](https://react-bootstrap.github.io/)
- [Bootstrap Documentation](https://getbootstrap.com/)
- [React Router Documentation](https://reactrouter.com/)
- [JSON Server Documentation](https://github.com/typicode/json-server)
- [React Hooks Documentation](https://reactjs.org/docs/hooks-intro.html)

For questions or contributions, please open an issue or pull request.
