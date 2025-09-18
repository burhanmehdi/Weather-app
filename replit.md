# Weather App

## Overview

This is a modern full-stack weather application built with React, Express, and TypeScript. The app provides current weather conditions, hourly forecasts, and multi-day forecasts for any location worldwide. Users can search for cities or use geolocation to get weather data for their current location. The application features a clean, responsive design with temperature unit conversion and caching for improved performance.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript
- **Styling**: Tailwind CSS with shadcn/ui component library for consistent design
- **State Management**: TanStack Query (React Query) for server state management and caching
- **Routing**: Wouter for lightweight client-side routing
- **Build Tool**: Vite for fast development and optimized production builds
- **UI Components**: Comprehensive set of accessible components using Radix UI primitives

### Backend Architecture
- **Runtime**: Node.js with Express.js framework
- **Language**: TypeScript for type safety across the entire stack
- **API Design**: RESTful API with structured error handling and request logging
- **Development Setup**: Hot module replacement with Vite integration for seamless development experience

### Data Storage Solutions
- **Primary Storage**: PostgreSQL database configured with Drizzle ORM
- **Caching Layer**: In-memory caching system for weather data with 10-minute expiration
- **Session Management**: PostgreSQL-backed session storage using connect-pg-simple
- **Database Migrations**: Managed through Drizzle Kit with schema versioning

### External Dependencies
- **Weather Service**: OpenWeatherMap API for current conditions, forecasts, and location search
- **Database Hosting**: Configured for Neon serverless PostgreSQL
- **Icon Library**: Font Awesome for weather condition icons
- **Component Library**: Extensive shadcn/ui component collection including forms, dialogs, charts, and navigation

### Key Features
- **Location Services**: City search with autocomplete and GPS-based location detection
- **Weather Data**: Current conditions, 7-day forecast, and 24-hour hourly predictions
- **User Experience**: Temperature unit conversion (Celsius/Fahrenheit), responsive design, and loading states
- **Performance**: API response caching, optimistic updates, and efficient re-fetching strategies
- **Accessibility**: ARIA-compliant components and keyboard navigation support

### Development Tools
- **Type Safety**: Shared TypeScript schemas between frontend and backend using Zod validation
- **Code Quality**: ESLint and TypeScript compiler checks
- **Build Process**: Separate client and server builds with optimized bundling
- **Development Experience**: Hot reloading, error overlays, and integrated debugging tools