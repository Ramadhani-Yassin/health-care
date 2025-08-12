# HealthCare Drugstore System

## Overview
HealthCare Drugstore is a comprehensive digital pharmacy management system for customers and administrators. It streamlines the process of ordering, managing, and delivering pharmaceutical products, and provides a platform for managing prescriptions, bills, and announcements. The system consists of three main components:

- **Back End**: PHP REST API with MySQL database
- **Front End**: HTML/CSS/JavaScript web application (Admin & Customer portals)
- **Mobile App**: Android app for customers (order products, manage prescriptions, view bills)

---

## Project Structure

```
drugstore/
  ├── admin/           # PHP Admin Panel
  ├── api/             # PHP REST API
  ├── assets/          # Frontend Assets (CSS, JS, Images)
  ├── clinic-app/      # Android Mobile App
  └── index.html       # Main Customer Portal
```

### Back End (PHP)
- **Admin Panel**: Complete admin interface for managing products, orders, users, and system settings
- **API**: RESTful API endpoints for mobile app and web integration
- **Database**: MySQL database with comprehensive schema for pharmacy management
- **Services**: Business logic for order processing, prescription management, and notifications

### Front End (HTML/CSS/JavaScript)
- **Customer Portal**: Main website for product browsing and ordering
- **Admin Dashboard**: Comprehensive admin interface with analytics and management tools
- **Responsive Design**: Mobile-friendly interface with modern UI/UX
- **Features**: Product catalog, shopping cart, order tracking, prescription upload

### Mobile App (Android)
- **Customer App**: Native Android experience for customers
  - **Product Browsing**: Browse categories and products with search functionality
  - **Shopping Cart**: Add/remove items and manage quantities
  - **Prescription Upload**: Upload prescription images for prescription-based orders
  - **Order Management**: Track orders and view order history
  - **Bill Payments**: Upload and manage utility bills
  - **Profile Management**: Update personal information and preferences
- **Modern UI/UX**: Material Design with smooth animations and intuitive navigation

---

## Setup Instructions

### Back End (PHP/MySQL)
1. Ensure you have XAMPP/LAMPP installed
2. Import the `drugstore.sql` file into MySQL
3. Configure database connection in `admin/includes/config.php`
4. Start Apache and MySQL services
5. Access admin panel at `http://localhost/drugstore/admin/`

### Front End
1. Place the project in your web server directory (e.g., `/opt/lampp/htdocs/drugstore/`)
2. Access the main site at `http://localhost/drugstore/`
3. Admin login credentials:
   - **Username**: `admin`
   - **Password**: `admin`

### Mobile App (Android)
1. Navigate to the `clinic-app` directory
2. Ensure you have Android Studio and Flutter installed
3. Install dependencies:
   ```
   flutter pub get
   ```
4. Run the app on an emulator or device:
   ```
   flutter run
   ```

---

## API Endpoints (Sample)
- **POST /api/v1/user/login**: User authentication
- **GET /api/v1/products**: Get all products
- **POST /api/v1/orders**: Create new order
- **GET /api/v1/orders/{user_id}**: Get user orders
- **POST /api/v1/prescriptions**: Upload prescription
- **GET /api/v1/categories**: Get product categories

---

## Features

### For Administrators
- **Product Management**: Add, edit, and manage products with categories
- **Order Management**: Process and track customer orders
- **User Management**: Manage customer accounts and profiles
- **Prescription Management**: Review and approve prescription-based orders
- **Analytics Dashboard**: View sales reports and system statistics
- **Banner Management**: Manage promotional banners and offers
- **Inventory Control**: Track stock levels and manage inventory

### For Customers (Web & Mobile)
- **Product Browsing**: Browse products by categories with search functionality
- **Shopping Cart**: Add products to cart and manage quantities
- **Order Placement**: Place orders with delivery address and payment options
- **Prescription Upload**: Upload prescription images for prescription-based products
- **Order Tracking**: Track order status and delivery progress
- **Bill Payments**: Upload and manage utility bills
- **Profile Management**: Update personal information and preferences
- **Order History**: View all past orders and their statuses

### Mobile App Features
- **Native Experience**: All customer features available natively on Android
- **Offline Capability**: Basic functionality works offline
- **Push Notifications**: Real-time order updates and promotions
- **Camera Integration**: Direct prescription and bill image capture
- **Modern UI**: Material Design with smooth animations and intuitive navigation

---

## Database Schema
The system uses a comprehensive MySQL database with tables for:
- Users and authentication
- Products and categories
- Orders and order items
- Prescriptions and bills
- Banners and promotions
- Admin management

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.

---

## 🏆 Developed by

**Ramadhani Yassin**  
[Personal Website](http://ramadhani-yassin.vercel.app/)  
[LinkedIn](https://www.linkedin.com/in/ramadhani-yassin-ramadhani/)

<div align="center">
  <a href="https://github.com/Ramadhani-Yassin" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">
  </a>
  <a href="https://www.linkedin.com/in/ramadhani-yassin-ramadhani/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
  <a href="mailto:yasynramah@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email">
  </a>
  <a href="http://ramadhani-yassin.vercel.app/" target="_blank">
    <img src="https://img.shields.io/badge/Website-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Website">
  </a>
</div>

---

## 🚀 Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/Ramadhani-Yassin/health-care.git
   cd health-care
   ```

2. **Setup Database**
   - Import `drugstore.sql` into MySQL
   - Configure database settings in `admin/includes/config.php`

3. **Start the Application**
   - Start XAMPP/LAMPP
   - Access web application at `http://localhost/drugstore/`
   - Access admin panel at `http://localhost/drugstore/admin/`

4. **Mobile App**
   - Open `clinic-app` in Android Studio
   - Run on device or emulator

---

## 📱 Screenshots

Check the `clinic-app/screen/` directory for mobile app screenshots and the main directory for web application previews.

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
