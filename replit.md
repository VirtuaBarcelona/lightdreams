# Overview

Nana App is a marketing landing page for a baby sleep guide mobile application. The project is a full-stack web application built to promote and provide information about a mobile app that helps parents track their baby's sleep patterns, access expert guidance, and establish healthy sleep routines. The landing page includes multiple sections showcasing app features, benefits, testimonials, and calls-to-action to drive app downloads.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **Framework**: React 18 with TypeScript, using Vite as the build tool
- **Routing**: Wouter for client-side routing with support for multiple pages (landing, privacy policy, terms of service, contact)
- **Styling**: Tailwind CSS with custom design system based on purple/blue color palette
- **Component Library**: Radix UI primitives with shadcn/ui component system for consistent, accessible UI components
- **State Management**: TanStack Query for server state management and caching
- **Form Handling**: React Hook Form with Zod validation schemas

## Backend Architecture
- **Runtime**: Node.js with Express.js framework
- **Language**: TypeScript with ES modules
- **Development Server**: Custom Vite integration for SSR and hot module replacement
- **Storage Interface**: Abstract storage layer with in-memory implementation (easily replaceable with database)
- **API Structure**: RESTful API design with `/api` prefix routing

## Data Storage
- **ORM**: Drizzle ORM configured for PostgreSQL with Neon Database integration
- **Schema**: User management system with username/password authentication
- **Migrations**: Drizzle Kit for database schema management
- **Session Storage**: PostgreSQL-based session storage using connect-pg-simple

## Design System
- **Component System**: Comprehensive UI library with consistent spacing, colors, and typography
- **Responsive Design**: Mobile-first approach with Tailwind breakpoints
- **Color Palette**: Purple/violet primary colors (270° 85% 25%) with cream backgrounds and supporting colors
- **Typography**: Inter font family with clear hierarchy and generous spacing
- **Interactive Elements**: Hover states, smooth transitions, and elevation effects for user engagement

## Development Tools
- **Build System**: Vite with React plugin and TypeScript support
- **Code Quality**: TypeScript strict mode with comprehensive type checking
- **Asset Management**: Vite asset handling with custom aliases for components and shared code
- **Hot Reload**: Development server with HMR and runtime error overlay

# External Dependencies

## Database Services
- **Neon Database**: Serverless PostgreSQL database hosting
- **Connection**: `@neondatabase/serverless` driver for database connectivity

## UI Component Libraries
- **Radix UI**: Headless component primitives for accessibility and functionality
- **Lucide React**: Icon library for consistent iconography
- **Tailwind CSS**: Utility-first CSS framework for styling
- **class-variance-authority**: For component variant management

## Development & Build Tools
- **Vite**: Fast build tool and development server
- **TypeScript**: Type safety and enhanced developer experience
- **ESBuild**: Fast JavaScript bundler for production builds
- **PostCSS**: CSS processing with Tailwind CSS integration

## Form & Data Management
- **React Hook Form**: Form state management and validation
- **Zod**: Schema validation for type-safe data handling
- **TanStack Query**: Server state synchronization and caching
- **date-fns**: Date manipulation and formatting utilities

## Development Experience
- **Replit Integration**: Custom Vite plugins for Replit development environment
- **Runtime Error Handling**: Development error overlay for debugging
- **Hot Module Replacement**: Fast development iteration with Vite HMR