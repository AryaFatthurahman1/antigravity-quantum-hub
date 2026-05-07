# AntiGravity Quantum Hub

[![PHP](https://img.shields.io/badge/PHP-8.0+-777BB4?style=flat&logo=php)](https://php.net/)
[![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?style=flat&logo=mysql)](https://mysql.com/)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=flat&logo=javascript)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

Unified control hub for the AntiGravity development ecosystem. A PHP-based platform that serves as the central management system for all web, AI, mobile, and quantum computing projects.

## Overview

AntiGravity Quantum Hub is a comprehensive PHP platform featuring:
- User authentication and registration system
- Service ordering platform for development services
- Dashboard with order history and analytics
- Quantum particle visualization background
- Glassmorphism design with dark theme
- Multi-page architecture with routing

## Features

### User Management
- Registration with email validation
- Secure login with password hashing
- Role-based access control (user/admin)
- Session management

### Services
- AI & Quantum Computing Services
- Web Development (Next.js, React, Vue, Svelte, Laravel)
- Mobile App Development (Flutter, React Native)
- Machine Learning API Integration
- Database Design & Management
- DevOps & Docker Solutions
- E-Commerce Platforms
- Hotel & Booking Systems

### Dashboard
- Order history with status tracking
- Account status monitoring
- Security level indicators
- Responsive data tables

### Design
- Particle canvas animation background
- Glassmorphism UI components
- Neon gradient accents
- Responsive navigation with mega menu
- Mobile-friendly hamburger menu

## Tech Stack

| Component | Technology |
|-----------|------------|
| Backend | PHP 8+ (Vanilla) |
| Database | MySQL with PDO |
| Frontend | HTML5, CSS3, JavaScript |
| Styling | Custom CSS with CSS Variables |
| Icons | Font Awesome 6.5 |
| Fonts | Outfit, JetBrains Mono, Space Grotesk |
| Animation | HTML5 Canvas API |

## Database Schema

### Tables
- **users** - User accounts with role management
- **orders** - Service orders with status tracking

## Installation

### Requirements
- PHP 8.0 or higher
- MySQL 5.7 or higher
- Apache/Nginx web server
- Laragon (recommended for Windows)

### Setup
1. Clone the repository to your web server directory
2. Create MySQL database `antigravity_hub`
3. The application auto-creates tables on first run
4. Access via `http://localhost/antigravity-quantum-hub/`

## Project Structure

```
antigravity-quantum-hub/
├── assets/
│   └── app.css              # Main stylesheet with glassmorphism
├── includes/
│   ├── auth.php             # Authentication functions
│   ├── db.php               # Database connection & auto-setup
│   ├── css_router.php       # CSS serving utility
│   ├── header.php           # Navigation & head section
│   └── footer.php           # Footer with scripts
├── pages/
│   ├── home.php             # Landing page with hero
│   ├── services.php         # Services listing
│   ├── projects.php         # Project portfolio
│   ├── quantum.php          # Quantum systems info
│   ├── order.php            # Service ordering form
│   ├── login.php            # Login page
│   ├── register.php         # Registration page
│   └── dashboard.php        # User dashboard
├── index.php                # Router & entry point
└── README.md
```

## Pages

| Page | Description |
|------|-------------|
| Home | Landing page with statistics and features |
| Services | 11 service categories with pricing |
| Projects | Portfolio of all live projects |
| Quantum | Quantum computing infrastructure details |
| Order | Service ordering form (requires login) |
| Login/Register | Authentication pages |
| Dashboard | User control panel with order history |

## Development

### Adding a New Page
1. Create a new `.php` file in the `pages/` directory
2. Add the page name to the `$allowedPages` array in `index.php`
3. Add a title case in the `$pageTitle` match expression

### Styling
The project uses CSS custom properties for theming:
```css
:root {
  --quantum-cyan: #00f5ff;
  --quantum-purple: #a855f7;
  --bg-dark: #050505;
  --glass-panel: rgba(15, 15, 20, 0.6);
}
```

## Author

**Arya Fatthurahman**
- GitHub: [@AryaFatthurahman1](https://github.com/AryaFatthurahman1)

## License

MIT License
