# SMM Panel - Social Media Marketing Dashboard

A full-featured SMM (Social Media Marketing) panel for buying and selling social media engagement services (followers, likes, views, comments, etc.) across multiple platforms.

## Features

- 🎯 **Multi-Platform Support**: Instagram, Facebook, TikTok, YouTube, Twitter, Telegram, Spotify
- 💰 **Payment Gateway Integration**: Stripe, PayPal, Cryptocurrency support
- 📊 **Admin Dashboard**: Manage services, pricing, users, and analytics
- 👥 **User Dashboard**: Order management, wallet, transaction history
- 🔄 **API Integration**: Reseller API for automation and bulk operations
- 📈 **Real-time Tracking**: Live order status and delivery progress
- 🛡️ **Security**: JWT authentication, rate limiting, fraud detection
- 📱 **Responsive Design**: Mobile-first UI
- 🔌 **Webhook Support**: Real-time order notifications

## Tech Stack

### Backend
- Node.js + Express.js
- PostgreSQL
- Redis (caching & sessions)
- JWT Authentication

### Frontend
- React 18+
- TypeScript
- Tailwind CSS
- Zustand (state management)

### Infrastructure
- Docker & Docker Compose
- GitHub Actions (CI/CD)
- AWS/DigitalOcean ready

## Quick Start

### Prerequisites
- Node.js 18+
- PostgreSQL 14+
- Redis
- Docker & Docker Compose (optional)

### Installation

```bash
# Clone repository
git clone https://github.com/celoza/smm-panel.git
cd smm-panel

# Install dependencies
npm install

# Setup environment variables
cp .env.example .env

# Run migrations
npm run migrate

# Start development server
npm run dev
```

### Docker Setup

```bash
docker-compose up -d
npm run migrate
npm run dev
```

## Project Structure

```
smm-panel/
├── backend/              # Express API
│   ├── src/
│   │   ├── routes/       # API endpoints
│   │   ├── controllers/  # Business logic
│   │   ├── models/       # Database models
│   │   ├── middleware/   # Auth, validation
│   │   ├── services/     # External integrations
│   │   └── utils/        # Helpers
│   ├── tests/
│   └── package.json
├── frontend/             # React dashboard
│   ├── src/
│   │   ├── pages/        # Route pages
│   │   ├── components/   # Reusable UI
│   │   ├── hooks/        # Custom hooks
│   │   ├── store/        # State management
│   │   └── api/          # API client
│   └── package.json
├── docs/                 # Documentation
├── docker-compose.yml
└── README.md
```

## Documentation

- [Installation Guide](docs/INSTALLATION.md)
- [API Documentation](docs/API.md)
- [Deployment Guide](docs/DEPLOYMENT.md)
- [Architecture](docs/ARCHITECTURE.md)

## License

MIT - See LICENSE file

## Disclaimer

This project is provided for educational purposes. Users are responsible for ensuring compliance with applicable laws and social media platform terms of service.
