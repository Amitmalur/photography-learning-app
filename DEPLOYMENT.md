# CameraLearn - Deployment Guide

## Overview
CameraLearn is an interactive photography learning application built with React, TypeScript, and Express.js. This guide covers deployment to various platforms including Git repositories, Vercel, Netlify, and other hosting services.

## Quick Deploy to Git Repository

### 1. Initialize Repository (if not already done)
```bash
git init
git add .
git commit -m "Initial commit: Interactive photography learning app"
```

### 2. Add Remote Repository
```bash
# For GitHub
git remote add origin https://github.com/your-username/camera-learn.git

# For GitLab
git remote add origin https://gitlab.com/your-username/camera-learn.git

# For Bitbucket
git remote add origin https://bitbucket.org/your-username/camera-learn.git
```

### 3. Push to Repository
```bash
git branch -M main
git push -u origin main
```

## Project Structure for Deployment

```
camera-learn/
├── client/                 # Frontend React application
│   ├── src/
│   │   ├── components/     # React components
│   │   ├── pages/         # Page components
│   │   ├── hooks/         # Custom React hooks
│   │   └── lib/           # Utility libraries
├── server/                # Backend Express.js API
│   ├── index.ts          # Server entry point
│   ├── routes.ts         # API routes
│   └── db.ts             # Database connection
├── shared/               # Shared types and schemas
├── docs/                # Documentation
├── package.json         # Dependencies and scripts
├── vite.config.ts      # Vite configuration
├── tailwind.config.ts  # Tailwind CSS config
└── README.md           # Project documentation
```

## Environment Variables Required

Create a `.env` file with these variables:

```env
# Database
DATABASE_URL=your_postgresql_connection_string
PGHOST=your_database_host
PGPORT=5432
PGUSER=your_database_user
PGPASSWORD=your_database_password
PGDATABASE=your_database_name

# Application
NODE_ENV=production
PORT=5000
```

## Deployment Platforms

### 1. Vercel (Recommended for Full-Stack)
```bash
npm install -g vercel
vercel
```

### 2. Netlify (Frontend Only)
```bash
npm run build
# Upload dist/ folder to Netlify
```

### 3. Railway
```bash
# Connect your GitHub repository to Railway
# Set environment variables in Railway dashboard
```

### 4. Render
```bash
# Connect GitHub repository
# Set build command: npm run build
# Set start command: npm start
```

### 5. Heroku
```bash
heroku create camera-learn-app
git push heroku main
```

## Build Commands

### Development
```bash
npm run dev          # Start development server
```

### Production Build
```bash
npm run build        # Build for production
npm start           # Start production server
```

### Database Setup
```bash
npm run db:push     # Push schema to database
```

## Features Included

### Core Photography Learning
- ✅ Interactive camera controls (ISO, aperture, shutter speed, white balance, focus)
- ✅ Real-time image preview with canvas-based effects
- ✅ Professional photography tutorials and guidance
- ✅ Smart hint system with context-aware suggestions

### Educational Features
- ✅ Step-by-step interactive tutorial system
- ✅ Gamified learning path with unlockable modules
- ✅ Achievement system with bronze/silver/gold/platinum tiers
- ✅ Practice challenges with different difficulty levels
- ✅ Interactive quiz system with progress tracking

### Technical Features
- ✅ PostgreSQL database with Drizzle ORM
- ✅ Full-stack TypeScript architecture
- ✅ Responsive design with Tailwind CSS
- ✅ Professional UI with Radix components
- ✅ Real-time visual feedback and effects

## Browser Support
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## Performance Features
- Optimized Canvas rendering for real-time effects
- Lazy loading of components
- Efficient state management
- Fast build times with Vite

## Security Features
- Input validation with Zod schemas
- SQL injection protection with Drizzle ORM
- Environment variable protection
- Secure session management

## Support and Documentation
- Full API documentation in `/docs/api.md`
- User guide in `/docs/user-guide.md`
- Architecture overview in `/docs/architecture.md`
- Setup instructions in `/README.md`

## License
MIT License - See LICENSE file for details

---

Built with ❤️ for photography education and interactive learning.