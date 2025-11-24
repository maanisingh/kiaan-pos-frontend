# Kiaan POS Frontend

Frontend for Kiaan POS system deployed on Railway.

## Features

- **Landing Page**: Main marketing page with service overview
- **Login Page**: Secure authentication with JWT tokens
- **Admin Dashboard**: Full-featured admin interface
- **Mobile App Demo**: Mobile app preview
- **POS Terminal**: POS terminal demo

## Structure

```
frontend/
├── server.js           # Express server
├── package.json        # Dependencies
├── public/            # Static files
│   ├── index.html     # Landing page
│   ├── login.html     # Login page
│   ├── dashboard.html # Admin dashboard
│   ├── mobile.html    # Mobile demo
│   └── pos.html       # POS demo
└── README.md          # This file
```

## Routes

- `/` - Landing page
- `/admin` - Login page
- `/admin/dashboard` - Admin dashboard (requires auth)
- `/dashboard` - Dashboard (alternative route)
- `/mobile` - Mobile app demo
- `/pos` - POS terminal demo

## API Configuration

The frontend connects to the Railway backend:
```javascript
const API_URL = 'https://kiaan-pos-wallet-system-production.up.railway.app/api';
```

## Local Development

```bash
npm install
npm start
```

Server runs on port 3000 by default (or PORT env variable).

## Railway Deployment

1. Push to GitHub
2. Connect GitHub repo to Railway
3. Railway auto-deploys
4. Frontend accessible via Railway URL

## Backend

Backend API: https://kiaan-pos-wallet-system-production.up.railway.app

## Demo Credentials

**Email**: `admin@kiaan.com`
**Password**: `admin123`
