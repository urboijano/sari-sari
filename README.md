# 🌱 Sari-Sari Sustento: Philippine SDG-Aligned POS & Analytics System

A dynamic web-based **Point of Sale (POS) system** designed for small-to-medium enterprises in the Philippines, integrating **sales tracking** with **automated reporting** on contributions to the **United Nations Sustainable Development Goals (SDGs).**

---

## 🌟 Features
- **Dynamic Web Application**: Single-page application (SPA) built with React for fluid user experience  
- **Complete CRUD Operations**: Full Create, Read, Update, Delete functionality across all modules  
- **SDG Integration**: Automatic tracking of sales contributions to Sustainable Development Goals  
- **Real-time Dashboard**: Interactive analytics and reporting dashboard  
- **Inventory Management**: Comprehensive product and stock management system  
- **Multi-user Support**: Role-based access control for shop owners and staff  

---

## 🛠️ Tech Stack
- **Frontend**: React.js with Material-UI / Ant Design  
- **Backend**: Django & Django REST Framework (DRF)  
- **Database**: PostgreSQL (production) / SQLite (development)  
- **Authentication**: Token-based authentication system  
- **API**: RESTful API architecture  

---

## 📋 System Modules
### 1. User Management & Authentication
- User registration and role management  
- Secure authentication system  
- Profile management  

### 2. Product & Inventory Management
- Complete product catalog with SDG tagging  
- Stock level tracking and alerts  
- Supplier management  

### 3. Point of Sale (POS)
- Sales transaction processing  
- Cart management with discounts  
- Receipt generation  
- Return/refund handling  

### 4. SDG Analytics & Reporting
- Automated SDG impact reporting  
- Interactive data visualization  
- Time-period based reporting  
- Philippine context-specific SDG mapping  

### 5. Supplier Management (Optional)
- Local supplier tracking  
- SDG-aligned supplier tagging  

---

## 🎯 SDG Integration for Philippine Context
The system automatically tags sales with relevant SDGs:  

- **SDG 1 (No Poverty):** Affordable essential goods tracking  
- **SDG 2 (Zero Hunger):** Nutritious food sales monitoring  
- **SDG 3 (Good Health):** Medicine and health product sales  
- **SDG 4 (Quality Education):** School supplies tracking  
- **SDG 5 (Gender Equality):** Products from women-owned suppliers  
- **SDG 8 (Decent Work):** Formal business operation support  
- **SDG 12 (Responsible Consumption):** Eco-friendly products tracking  
- **SDG 13 (Climate Action):** Energy-efficient product sales  

---

## 🚀 Installation & Setup

### Prerequisites
- Python 3.8+  
- Node.js 14+  
- PostgreSQL (optional for production)  

### Backend Setup (Django)
```bash
# Clone the repository
git clone <repository-url>
cd sustento-backend

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Configure database settings in settings.py

# Run migrations
python manage.py migrate

# Create superuser
python manage.py createsuperuser

# Start development server
python manage.py runserver

cd sustento-frontend

# Install dependencies
npm install

# Start development server
npm start

# 📊 Database Schema & API Documentation

This document provides details on the **database schema**, **API endpoints**, and **deployment options** for the Sari-Sari Sustento system.

---

## 📊 Database Schema

Key models include:

- **User** – Extended user model with roles  
- **Product** – Product information with SDG many-to-many relationship  
- **SDG** – Sustainable Development Goal definitions  
- **Sale** – Transaction records  
- **SaleItem** – Individual items within transactions  
- **Supplier** – Vendor information  

---

## 🔧 API Endpoints

| Method | Endpoint              | Description            |
|--------|-----------------------|------------------------|
| POST   | `/api/auth/register/` | User registration      |
| POST   | `/api/auth/login/`    | User login             |
| GET    | `/api/products/`      | List products          |
| POST   | `/api/products/`      | Create product         |
| GET    | `/api/products/{id}/` | Retrieve product       |
| PUT    | `/api/products/{id}/` | Update product         |
| DELETE | `/api/products/{id}/` | Delete product         |
| POST   | `/api/sales/`         | Create sale            |
| GET    | `/api/sdg-report/`    | Generate SDG report    |

---

## 🌐 Deployment

The application can be deployed using:

- **Traditional Deployment**: Nginx + Gunicorn for backend, React build for frontend  
- **Containerization**: Docker & Docker Compose  
- **PaaS**: Heroku, AWS Elastic Beanstalk, DigitalOcean App Platform  

---

## 🤝 Contributing

1. Fork the project  
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)  
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)  
4. Push to the branch (`git push origin feature/AmazingFeature`)  
5. Open a Pull Request  

---

## 📄 License

This project is licensed under the **MIT License** – see the [LICENSE.md](LICENSE.md) file for details.  

---

## 🙏 Acknowledgments

- United Nations Sustainable Development Goals framework  
- Philippine business community for inspiration  
- Django and React open-source communities  

---

## 📞 Contact

For questions or support, please contact: **[Your Email]** or create an issue in the repository.  
