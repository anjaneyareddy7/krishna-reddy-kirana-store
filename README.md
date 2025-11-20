# krishna-reddy-kirana-store
A full-featured e-commerce web application for Krishna Reddy Kirana Store built with React and Base44. Features include product catalog, shopping cart, checkout, order management, and admin dashboard.

## 📋 Overview

Krishna Reddy Kirana Store is a modern e-commerce platform designed for grocery retail operations. Built using React and Base44, this application provides a complete shopping experience with both customer-facing and administrative features.

## ✨ Features

### Customer Features
- 🛍️ **Product Catalog**: Browse through a comprehensive list of grocery products
- 🛒 **Shopping Cart**: Add, remove, and manage items in your cart
- 💳 **Checkout Process**: Secure and streamlined checkout experience
- 📦 **Order Tracking**: View order history and track current orders
- 🔍 **Product Search**: Easily find products with search functionality

### Admin Features
- 📊 **Dashboard**: Overview of store performance and metrics
- 📝 **Product Management**: Add, edit, and remove products from inventory
- 📋 **Order Management**: Process and manage customer orders
- 📈 **Analytics**: Track sales and customer behavior

## 🛠️ Tech Stack

- **Frontend Framework**: React
- **Platform**: Base44
- **UI Components**: Custom components including ProductCard, Card, CardHeader, CardTitle, CardContent
- **State Management**: React hooks (useState, useEffect)
- **API Integration**: Base44 client and entities
- **Routing**: React Query (@tanstack/react-query)
- **Icons**: Lucide React, XCircle, Truck, CheckCircle
- **Animations**: Framer Motion
- **Form Handling**: date-fns for date formatting
- **Badge Components**: Custom UI components

## 📁 Project Structure

### Pages
- `Home` - Main landing page with product listings
- `Cart` - Shopping cart page
- `Checkout` - Order checkout and payment
- `MyOrders` - Customer order history
- `ProductDetail` - Individual product details
- `AdminDashboard` - Admin overview and analytics
- `AdminProducts` - Product inventory management
- `AdminOrders` - Order processing and management

### Components
- `ProductCard` - Reusable product display component
- Custom UI components for enhanced user experience

### Entities
- `Product` - Product data model
- `Order` - Order data model

## 🚀 Getting Started

This application is built on the Base44 platform. To work with this project:

1. **Base44 Account**: You need a Base44 account to access and modify the application
2. **Access the App**: Visit the Base44 editor at the project URL
3. **View Code**: Navigate through pages, components, and entities in the Base44 interface

## 📱 Application Features in Detail

### Authentication
- User authentication integrated with Base44 Auth
- Automatic redirect to login for unauthorized access
- User session management

### Order Management
- Real-time order status tracking
- Order filtering by user email
- Status badges for order states (pending, uploading, uploaded, failed)

### Product Management
- Dynamic product catalog
- Product categorization
- Image management for products
- Inventory tracking

## 🔧 Development

This application uses Base44's visual development environment:
- **No local setup required** - Development happens in the cloud
- **Real-time preview** - See changes instantly
- **Integrated backend** - Base44 provides API and database management

## 📝 Code Structure

Based on the MyOrders page implementation visible in the codebase:

```javascript
// Example: User authentication and data fetching
const [user, setUser] = useState(null);

useEffect(() => {
  loadUser();
}, []);

const loadUser = async () => {
  try {
    const currentUser = await base44.auth.me();
    setUser(currentUser);
  } catch (error) {
    base44.auth.redirectToLogin();
  }
};
```

## 🌐 Deployment

The application is deployed through Base44's hosting platform:
- Automatic deployment on commit
- CDN-backed hosting for fast global access
- SSL/HTTPS enabled by default

## 📄 License

This project is available for educational and commercial use.

## 👥 Contributing

This is a Base44 project. To contribute:
1. Request access to the Base44 project
2. Make changes in the Base44 editor
3. Test changes in preview mode
4. Submit for review

## 📧 Contact

For questions or support regarding this project, please contact the repository owner.

## 🙏 Acknowledgments

- Built with [Base44](https://base44.com) - Modern web application platform
- React and the React community for excellent documentation and tools

---

**Note**: This application is built on the Base44 platform. The source code is managed through Base44's visual development environment. Direct GitHub integration requires a Base44 paid plan.
