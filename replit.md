# Overview

DataBoard is a business intelligence dashboard application that provides comprehensive analytics and reporting for organizational units. Built as a full-stack web application, it displays key performance metrics including sales data, performance scores, and financial information across different business units. The system features an interactive dashboard with detailed drill-down capabilities and responsive data visualization.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **Framework**: React with TypeScript for type safety and component-based development
- **Routing**: Wouter for lightweight client-side routing
- **State Management**: TanStack Query (React Query) for server state management and caching
- **UI Framework**: Radix UI components with shadcn/ui for consistent, accessible design system
- **Styling**: Tailwind CSS for utility-first styling with CSS custom properties for theming
- **Build Tool**: Vite for fast development and optimized production builds

## Backend Architecture
- **Runtime**: Node.js with Express.js for REST API server
- **Language**: TypeScript with ES modules for modern JavaScript features
- **API Design**: RESTful endpoints organized by business domains (units, sales, performance, financial data)
- **Error Handling**: Centralized middleware for consistent error responses
- **Development**: Hot reloading with Vite integration in development mode

## Data Layer
- **ORM**: Drizzle ORM for type-safe database operations and migrations
- **Database**: PostgreSQL as primary data store (configured for Neon serverless)
- **Schema**: Relational design with units as central entity, linked to sales, performance, and financial data tables
- **Validation**: Zod schemas for runtime type validation integrated with Drizzle
- **Session Storage**: PostgreSQL-based session storage using connect-pg-simple

## Component Architecture
- **Layout System**: Main layout with sidebar navigation and detail sidebar for drill-down views
- **Data Tables**: Reusable DataTable component with sorting, filtering, and click-to-detail functionality
- **UI Components**: Comprehensive component library including cards, charts, forms, dialogs, and data visualization elements
- **Responsive Design**: Mobile-first approach with adaptive layouts and touch-friendly interactions

## External Dependencies

- **Database**: Neon PostgreSQL for serverless database hosting
- **UI Components**: Radix UI primitives for accessible, headless components
- **Charts**: Recharts for data visualization and charting capabilities
- **Date Handling**: date-fns for date manipulation and formatting
- **Development Tools**: ESBuild for fast bundling, TSX for TypeScript execution
- **Styling**: Tailwind CSS with PostCSS for processing and optimization
- **Session Management**: Express sessions with PostgreSQL store
- **Form Handling**: React Hook Form with Hookform resolvers for validation
- **Icons**: Lucide React for consistent iconography throughout the application