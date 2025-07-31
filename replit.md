# Mind Map Generator Application

## Overview

This is a React-based mind map generator application that uses AI to create interactive mind maps from user-provided topics. The application integrates with OpenRouter API for AI-powered content generation and uses Mind-Elixir for visualization. Built with a modern tech stack including React, TypeScript, Express.js, and styled with Tailwind CSS and shadcn/ui components.

## User Preferences

Preferred communication style: Simple, everyday language.
Design preferences: Vibrant, animated 3D graphics with attractive colors that engage users.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript
- **Build Tool**: Vite for fast development and building
- **Routing**: Wouter for lightweight client-side routing
- **State Management**: React Query (TanStack Query) for server state management
- **UI Components**: shadcn/ui component library with Radix UI primitives
- **Styling**: Tailwind CSS with custom CSS variables for theming
- **Form Handling**: React Hook Form with Zod validation

### Backend Architecture
- **Framework**: Express.js with TypeScript
- **API Style**: RESTful API design
- **Middleware**: JSON parsing, URL encoding, and custom logging middleware
- **Error Handling**: Centralized error handling with proper HTTP status codes
- **Development**: Hot reload with Vite integration in development mode

### Build System
- **Frontend**: Vite with React plugin and runtime error overlay
- **Backend**: esbuild for production bundling
- **TypeScript**: Strict mode enabled with path mapping for clean imports
- **Development**: Concurrent frontend and backend development with file watching

## Key Components

### Mind Map Generation Flow
1. **Input Component** (`MindMapGenerator`): Text input with validation for topic submission
2. **API Integration**: OpenRouter API calls for AI-generated mind map content
3. **Canvas Component** (`MindMapCanvas`): Mind-Elixir integration for interactive visualization
4. **Data Flow**: React Query for async state management and caching

### UI System
- **Design System**: shadcn/ui with vibrant 3D animated theming via CSS variables
- **Visual Style**: Gradient backgrounds, glass-morphism effects, neon glows, and floating animations
- **Responsive Design**: Mobile-first approach with Tailwind CSS and 3D hover effects
- **Component Architecture**: Modular, reusable components with proper TypeScript typing
- **Animations**: Floating elements, bounce-in effects, gradient shifts, and pulse glows
- **Toast Notifications**: User feedback for success/error states

### External Libraries
- **Mind-Elixir**: Dynamically loaded for mind map visualization
- **Radix UI**: Accessible, unstyled component primitives
- **Lucide React**: Icon system for consistent iconography

## Data Flow

### Mind Map Generation Process
1. User enters topic in input field
2. Form validation using Zod schemas
3. API request to `/api/mindmap/generate` endpoint
4. OpenRouter API processes request and returns structured JSON
5. Response validation against predefined schemas
6. Mind map data conversion to Mind-Elixir format
7. Dynamic rendering of interactive mind map

### API Response Structure
```typescript
{
  topic: string,
  branches: [
    {
      title: string,
      children: string[]
    }
  ]
}
```

### Error Handling
- Client-side validation before API calls
- Server-side error responses with proper HTTP status codes
- Toast notifications for user feedback
- Graceful fallbacks for failed API requests

## External Dependencies

### Primary Dependencies
- **OpenRouter API**: AI content generation service requiring API key configuration
- **Mind-Elixir CDN**: Dynamically loaded for mind map visualization (no build dependency)
- **Neon Database**: PostgreSQL database (configured but not actively used for mind map generation)

### Development Dependencies
- **Replit Integration**: Development banner and cartographer plugin for Replit environment
- **Drizzle ORM**: Database toolkit configured for PostgreSQL with migration support

### Environment Configuration
- `OPENROUTER_API_KEY`: Required for AI mind map generation
- `DATABASE_URL`: PostgreSQL connection string (future use)
- `NODE_ENV`: Environment detection for development features

## Deployment Strategy

### Production Build
- **Frontend**: Vite build outputs to `dist/public` directory
- **Backend**: esbuild bundles server code to `dist/index.js`
- **Static Assets**: Served directly from Express in production

### Development Workflow
- **Hot Reload**: Vite dev server with HMR for frontend changes
- **Backend Watching**: tsx with file watching for server-side changes
- **Environment**: Automatic detection and configuration based on NODE_ENV

### Database Management
- **Schema**: Defined in `shared/schema.ts` using Drizzle ORM
- **Migrations**: Generated in `migrations/` directory
- **Commands**: `db:push` for schema synchronization

### Replit Optimization
- **Banner Integration**: Development mode banner for external access
- **Cartographer**: Code mapping for better debugging experience
- **File System**: Configured security restrictions for production safety

## Recent Changes

### January 31, 2025 - Visual Tree Diagram Generation
- **ASCII Tree Diagrams**: Added tree diagram format with visual ASCII art representation
- **SVG Vector Graphics**: Scalable vector graphics export for high-quality visual diagrams
- **Enhanced Export Options**: Five total formats - HTML, Markdown, Plain Text, ASCII Diagram, SVG
- **Visual Tree Structure**: Downloadable diagrams showing ROOT → Branch → Leaf hierarchy
- **Cross-Platform Compatibility**: Diagrams work on all devices and can be printed or shared

### January 31, 2025 - Enhanced Download Functionality Fix
- **Cross-Platform Downloads**: Rewritten download system with multiple fallback methods for reliable file saving
- **Mobile Download Improvements**: Enhanced iOS Safari support with dedicated download pages and clear instructions
- **File Share API Integration**: Native mobile sharing capabilities with automatic fallbacks
- **Better Error Handling**: Multiple download triggers and comprehensive mobile device detection
- **Enhanced Preview Function**: Improved report preview with better formatting and download hints

### January 31, 2025 - GitHub Repository Preparation
- **Project Documentation**: Created comprehensive README with setup instructions and feature descriptions
- **License and Environment**: Added MIT license and example environment configuration
- **GitHub Setup Guide**: Step-by-step instructions for repository creation and upload
- **Repository Structure**: Well-organized codebase ready for version control and collaboration

### January 31, 2025 - Complete Frontend Layout Redesign
- **Fixed Tree Spacing Issues**: Completely redesigned tree layout with proper node alignment and spacing
- **Mobile-First Design**: Responsive grid layout that works perfectly on all screen sizes
- **Enhanced Node Display**: Clean, properly sized nodes with contained text and no overflow
- **Improved Mobile Downloads**: iOS Safari support with download instructions and file save functionality
- **Better Visual Hierarchy**: Clear ROOT → Branch → Leaf structure with proper connecting lines
- **Professional Card Layout**: Well-spaced cards with proper padding and responsive design

### January 31, 2025 - Printable Tree Report Generator Implementation
- **Print-Optimized HTML**: CSS styling specifically designed for clean printing
- **Download & Preview Options**: Direct download, browser preview, and print functionality
- **Report Statistics**: Automatic calculation and display of node counts and structure metrics

### January 31, 2025 - Tree Hierarchy View Implementation
- **Hierarchical Tree Structure**: Replaced visual mind map with organized tree hierarchy display
- **Root-Branch-Leaf Organization**: Clear visual hierarchy with ROOT → Branches → Leaf nodes
- **Color-Coded Levels**: Purple for root, blue for branches, green for leaf nodes with connecting lines
- **Tree Statistics**: Added node counts showing root, branch, and leaf node statistics
- **Enhanced Readability**: Structured layout with proper indentation and visual connections

### January 31, 2025 - Clean Professional Redesign
- **Improved Typography**: Proper font sizes (4xl headers, xl descriptions) with consistent spacing and clean line heights
- **Better Layout Structure**: Organized sections with appropriate padding (p-8, py-6) and margins (mb-12, gap-8)
- **Simplified Color Palette**: Clean gradient backgrounds without overwhelming effects, reduced complexity
- **Professional Spacing**: Consistent space-x-4, space-y-6 throughout interface, no overlapping elements
- **Clean Text Layout**: Removed excessive highlighting, improved readability with proper text spacing
- **Organized Components**: Well-structured cards, buttons, and input fields with proper visual hierarchy
- **Responsive Grid**: Proper md:grid-cols-3 layout for features section with consistent gap spacing

### January 30, 2025 - Enhanced Visual Design
- **Vibrant Color Scheme**: Implemented animated gradient backgrounds with purple, pink, blue, cyan, yellow, and orange color palette
- **3D Effects**: Added glass-morphism styling, neon glows, card hover transformations, and floating animations
- **Interactive Elements**: Enhanced buttons with gradient backgrounds, scaling effects, and improved visual feedback
- **Animated Components**: Floating background elements, bounce-in animations, and gradient text effects
- **Enhanced Mind Map Canvas**: Updated both interactive and fallback views with vibrant 3D styling and improved user experience