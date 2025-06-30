# 📸 CameraLearn - Interactive Photography Learning Platform

[![React](https://img.shields.io/badge/React-18-blue.svg)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0-blue.svg)](https://www.typescriptlang.org/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-15-blue.svg)](https://www.postgresql.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-3.0-blue.svg)](https://tailwindcss.com/)

An immersive, interactive web application designed to teach photography fundamentals through real-time camera controls, intelligent hints, and gamified learning experiences.

## ✨ Features

### 🎯 Interactive Learning System
- **Real-time Camera Controls** - Adjust ISO, aperture, shutter speed, white balance, and focus with instant visual feedback
- **Smart Hint System** - Context-aware suggestions that analyze your settings and provide professional photography advice
- **Enhanced Tooltips** - Comprehensive explanations with usage ranges, effects, and practical tips for each camera setting
- **Interactive Tutorial** - Step-by-step guided learning through photography fundamentals

### 🏆 Gamified Experience
- **Learning Path** - Structured modules with XP points and skill development tracking
- **Achievement System** - Bronze, silver, gold, and platinum achievements that unlock as you practice
- **Progress Tracking** - Monitor your photography journey with detailed statistics and completion rates
- **Practice Challenges** - Real-world scenarios with target settings and difficulty levels

### 🎨 Visual & Technical
- **Canvas-based Image Effects** - Real-time simulation of ISO noise, aperture blur, white balance, and exposure changes
- **Professional UI** - Clean, modern interface inspired by Adobe Lightroom with photography-focused design
- **Responsive Design** - Works seamlessly on desktop, tablet, and mobile devices
- **Database Integration** - PostgreSQL with persistent progress tracking and user data

### 📚 Educational Content
- **Photography Quiz** - Interactive questions with detailed explanations and scoring
- **Professional Tips** - Expert advice on camera shake, diffraction, exposure triangle, and creative techniques
- **Practical Scenarios** - Learn through realistic photography situations and challenges

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ 
- PostgreSQL database
- Git

### Installation
```bash
# Clone the repository
git clone https://github.com/your-username/camera-learn.git
cd camera-learn

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
# Edit .env with your database credentials

# Initialize database
npm run db:push

# Start development server
npm run dev
```

Visit `http://localhost:5000` to start learning photography!

## 🛠️ Technology Stack

### Frontend
- **React 18** with TypeScript for component architecture
- **Vite** for fast development and optimized builds
- **Tailwind CSS** for utility-first styling
- **Radix UI** for accessible component primitives
- **Canvas API** for real-time image effects
- **TanStack Query** for efficient data fetching

### Backend
- **Express.js** with TypeScript for API routes
- **Drizzle ORM** for type-safe database operations
- **PostgreSQL** for reliable data persistence
- **Zod** for runtime type validation

### Development Tools
- **TypeScript** for enhanced developer experience
- **ESLint & Prettier** for code quality
- **Vite** for fast hot module replacement

## 📖 How It Works

1. **Interactive Controls** - Use sliders to adjust camera settings and see real-time effects on the preview image
2. **Smart Feedback** - Receive intelligent hints about your current settings, from warnings about camera shake to congratulations on good technique
3. **Learn by Doing** - Follow the interactive tutorial or explore the learning path with structured modules
4. **Track Progress** - Earn XP points and unlock achievements as you master different photography concepts
5. **Test Knowledge** - Take quizzes to reinforce learning and track your understanding

## 🎓 What You'll Learn

- **ISO Sensitivity** - Master light sensitivity and noise management
- **Aperture Control** - Create depth of field effects and control sharpness
- **Shutter Speed** - Freeze motion or create artistic blur effects  
- **White Balance** - Achieve accurate colors in different lighting conditions
- **Exposure Triangle** - Balance all three settings for perfect exposure
- **Professional Techniques** - Learn about diffraction, camera shake, and creative applications

## 🏗️ Project Structure

```
camera-learn/
├── client/src/
│   ├── components/          # React components
│   │   ├── camera-controls.tsx
│   │   ├── smart-hints.tsx
│   │   ├── learning-progress.tsx
│   │   └── achievement-system.tsx
│   ├── pages/              # Page components
│   ├── hooks/              # Custom React hooks
│   └── lib/                # Utilities and configurations
├── server/                 # Express.js backend
│   ├── index.ts           # Server entry point
│   ├── routes.ts          # API routes
│   └── db.ts              # Database connection
├── shared/                # Shared types and schemas
└── docs/                  # Documentation
```

## 🚀 Deployment

### Quick Deploy Options
- **Vercel** (Recommended): Connect your GitHub repository for automatic deployments
- **Railway**: Full-stack deployment with automatic PostgreSQL provisioning
- **Render**: Deploy both frontend and backend with custom domains
- **Netlify**: Frontend-only deployment (requires separate backend hosting)

See [DEPLOYMENT.md](./DEPLOYMENT.md) for detailed deployment instructions.

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guide](./CONTRIBUTING.md) for details.

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Commit changes: `git commit -m 'Add amazing feature'`
4. Push to branch: `git push origin feature/amazing-feature`
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.

## 🙏 Acknowledgments

- Built with modern web technologies for optimal learning experience
- Inspired by professional photography education and gamified learning principles
- Uses authentic photography concepts and real-world scenarios

---

**Ready to master photography?** [Start Learning →](https://your-app-url.com)

Built with ❤️ for photography education and interactive learning.