# CameraLearn Photography App

## Overview

CameraLearn is a full-stack educational web application designed to teach photography fundamentals through interactive camera controls, real-time image previews, and gamified learning experiences. The app combines a React frontend with an Express.js backend, utilizing PostgreSQL for data persistence and modern UI components for an engaging user experience.

## System Architecture

### Full-Stack Architecture
- **Frontend**: React with TypeScript, using Vite as the build tool
- **Backend**: Express.js with TypeScript
- **Database**: PostgreSQL with Drizzle ORM
- **UI Framework**: Radix UI components with shadcn/ui styling
- **Styling**: Tailwind CSS with custom photography-themed design tokens
- **State Management**: TanStack Query for server state, React hooks for local state
- **Routing**: Wouter for client-side routing

### Project Structure
The application follows a monorepo structure with shared code:
- `client/` - Frontend React application
- `server/` - Backend Express.js API
- `shared/` - Shared types, schemas, and utilities
- Database migrations stored in `migrations/`

## Key Components

### Frontend Architecture
- **Component-based UI**: Modular React components with TypeScript
- **Design System**: Custom photography-themed color palette with CSS variables
- **Interactive Controls**: Real-time camera setting sliders (ISO, aperture, shutter speed, white balance)
- **Image Effects**: Canvas-based image processing for simulating camera settings
- **Responsive Design**: Mobile-first approach with Tailwind CSS

### Backend Architecture
- **RESTful API**: Express.js server with middleware for logging and error handling
- **Storage Interface**: Abstracted storage layer supporting both in-memory and database implementations
- **Development Setup**: Hot-reload with tsx, Vite integration for development

### Database Schema
- **Users**: User accounts with levels, experience points, and completed challenges
- **User Progress**: Tracking lesson completion and scores
- **Quiz Results**: Storing quiz performance data
- **Drizzle ORM**: Type-safe database operations with PostgreSQL dialect

## Data Flow

### Learning Flow
1. Users interact with camera controls (sliders for ISO, aperture, etc.)
2. Settings changes trigger real-time image preview updates
3. Canvas-based effects simulate actual camera behavior
4. Progress tracking stores lesson completion and quiz results
5. Gamification elements (levels, experience) motivate continued learning

### State Management
- **Local State**: Camera settings managed by custom hooks
- **Server State**: User progress and quiz data managed by TanStack Query
- **Real-time Updates**: Immediate visual feedback through canvas manipulation

## External Dependencies

### Core Framework Dependencies
- **React 18**: Component framework with hooks
- **Express.js**: Backend web framework
- **Drizzle ORM**: Type-safe database ORM
- **@neondatabase/serverless**: PostgreSQL serverless driver

### UI and Styling
- **Radix UI**: Accessible component primitives
- **Tailwind CSS**: Utility-first CSS framework
- **Lucide React**: Icon library
- **shadcn/ui**: Pre-built component library

### Development Tools
- **Vite**: Fast build tool with HMR
- **TypeScript**: Type safety across the stack
- **tsx**: TypeScript execution for development

## Deployment Strategy

### Build Process
- **Frontend**: Vite builds optimized React bundle to `dist/public`
- **Backend**: esbuild bundles server code to `dist/index.js`
- **Database**: Drizzle migrations managed via `drizzle-kit push`

### Environment Configuration
- **Development**: NODE_ENV=development with hot-reload
- **Production**: NODE_ENV=production with optimized builds
- **Database**: DATABASE_URL environment variable required

### Replit Integration
- Custom Vite plugins for Replit development environment
- Runtime error overlay for development
- Cartographer integration for code mapping

## Recent Changes

### Advanced Interactive Learning System (June 30, 2025)
- ✓ Enhanced tooltips with comprehensive photography guidance, usage ranges, and practical tips
- ✓ Smart hints system providing real-time context-aware suggestions based on camera settings
- ✓ Interactive camera tutorial with step-by-step guidance through all settings
- ✓ Professional photography warnings (camera shake, diffraction, exposure issues)
- ✓ Actionable recommendations with one-click setting adjustments
- ✓ Learning progress tracking with gamified modules and skill development
- ✓ Achievement system with bronze/silver/gold/platinum tiers and points
- ✓ Tabbed interface for tutorial, learning path, practice, and quiz sections

### Database Integration (June 30, 2025)
- ✓ Integrated PostgreSQL database with Drizzle ORM
- ✓ Created comprehensive API endpoints for users, progress, and quiz results
- ✓ Enhanced quiz system to save results to database
- ✓ Implemented user progress tracking for lessons and challenges
- ✓ Added database storage layer replacing in-memory storage

### Enhanced Interactive Features (June 30, 2025)
- ✓ Added focus control slider with real-time visual feedback
- ✓ Implemented EV (Exposure Value) calculation and display
- ✓ Created fully interactive quiz system with 3 photography questions
- ✓ Enhanced practice challenges with detailed scenarios and target settings
- ✓ Added educational tooltips for all camera controls
- ✓ Improved real-time image effects for ISO noise, aperture blur, white balance, and exposure

### Core Photography Learning Features
- ✓ Real-time camera setting adjustments (ISO, aperture, shutter speed, white balance, focus)
- ✓ Canvas-based image effects that simulate actual camera behavior
- ✓ Interactive practice challenges with different difficulty levels
- ✓ Gamified quiz system with progress tracking and scoring
- ✓ Educational content with tips and explanations for each setting

## Changelog

```
Changelog:
- June 30, 2025. Database integration complete - PostgreSQL with full API endpoints and persistent data storage
- June 30, 2025. Enhanced app with focus control, EV display, interactive quiz, and improved challenges
- June 30, 2025. Initial setup with basic camera controls and image preview
```

## User Preferences

```
Preferred communication style: Simple, everyday language.
```