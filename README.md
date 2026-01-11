# Lucky - Service Marketplace Platform

A commission-based service marketplace connecting customers with service providers.

## Features

### Customer Panel
- Search services by category, location, price, and rating
- Online booking with date/time selection
- Track booking status
- View service provider profiles
- Rate and review services
- User authentication (OTP/Email)

### Service Provider Panel
- Registration and profile creation
- Service management (categories, pricing, availability)
- Booking management dashboard
- Earnings tracking
- KYC verification
- Ratings visibility

### Admin Panel
- Full dashboard with SQL integration
- Service category management
- Provider approval/blocking
- User, booking & transaction management
- Dynamic commission settings (10%-30%)
- Revenue analytics
- Role-based access control

### Payment System
- Commission auto-calculation
- Provider wallet system
- Multiple payment options (Razorpay/Stripe/PayPal)
- Cash booking option
- Invoice generation
- Transaction history

## Tech Stack

- **Backend**: Laravel 10.x (PHP 8.1+)
- **Database**: MySQL 8.0+
- **Frontend**: Blade Templates + Tailwind CSS + Alpine.js
- **Authentication**: Laravel Breeze/Sanctum
- **Payment**: Razorpay/Stripe Integration
- **API**: RESTful API for future mobile app

## Installation

### Prerequisites
- PHP 8.1 or higher
- Composer
- MySQL 8.0 or higher
- Node.js & NPM

### Setup Steps

1. Clone the repository
```bash
git clone https://github.com/tejindersingh8877-blip/lucky.git
cd lucky
```

2. Install dependencies
```bash
composer install
npm install
```

3. Configure environment
```bash
cp .env.example .env
php artisan key:generate
```

4. Configure database in `.env`
```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=lucky_db
DB_USERNAME=your_username
DB_PASSWORD=your_password
```

5. Run migrations and seeders
```bash
php artisan migrate --seed
```

6. Build assets
```bash
npm run build
```

7. Start the server
```bash
php artisan serve
```

Visit: http://localhost:8000

## Default Admin Credentials
- Email: admin@lucky.com
- Password: admin123

## Project Structure

```
lucky/
├── app/
│   ├── Http/Controllers/
│   │   ├── Admin/
│   │   ├── Customer/
│   │   └── Provider/
│   ├── Models/
│   └── Services/
├── database/
│   ├── migrations/
│   └── seeders/
├── resources/
│   ├── views/
│   │   ├── admin/
│   │   ├── customer/
│   │   └── provider/
│   └── js/
├── routes/
│   ├── web.php
│   └── api.php
└── public/
```

## Security Features
- CSRF Protection
- SQL Injection Prevention
- XSS Protection
- Password Hashing (bcrypt)
- Rate Limiting
- Secure Authentication

## API Documentation
API endpoints available at `/api/documentation` after setup.

## License
Proprietary - All rights reserved

## Support
For support, email: support@lucky.com