# 🧠 AI Mind Map Generator

A stunning AI-powered mind map generator that transforms ideas into interactive visual knowledge maps using advanced AI technology and vibrant 3D graphics.

![AI Mind Map Generator](https://img.shields.io/badge/AI-Powered-purple?style=for-the-badge)
![React](https://img.shields.io/badge/React-18-blue?style=for-the-badge&logo=react)
![TypeScript](https://img.shields.io/badge/TypeScript-strict-blue?style=for-the-badge&logo=typescript)
![Tailwind](https://img.shields.io/badge/Tailwind-CSS-cyan?style=for-the-badge&logo=tailwindcss)

## ✨ Features

- **🤖 AI-Powered Generation**: Uses OpenRouter API to create comprehensive mind maps from any topic
- **🎨 Vibrant 3D Design**: Animated gradients, glass-morphism effects, and floating animations
- **⚡ Interactive Visualization**: Built with Mind-Elixir for dynamic mind map exploration
- **🚀 Modern Tech Stack**: React 18, TypeScript, Express.js, and Tailwind CSS
- **📱 Responsive Design**: Beautiful experience across all devices
- **🎭 Animated UI**: Neon glows, bounce effects, and smooth transitions

## 🎬 Demo

Enter any topic like "Photosynthesis", "Machine Learning", or "Ancient Rome" and watch as AI generates a stunning visual mind map with interconnected concepts and subtopics.

## 🛠️ Tech Stack

### Frontend
- **React 18** with TypeScript
- **Vite** for fast development and building
- **Wouter** for lightweight routing
- **TanStack Query** for server state management
- **shadcn/ui** component library
- **Tailwind CSS** with custom animations
- **Mind-Elixir** for mind map visualization

### Backend
- **Express.js** with TypeScript
- **OpenRouter API** integration
- **Zod** for data validation
- **RESTful API** design

## 🚀 Quick Start

### Prerequisites
- Node.js 20+ installed
- OpenRouter API key ([Get one here](https://openrouter.ai/))

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/ai-mindmap-generator.git
   cd ai-mindmap-generator
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   ```bash
   # Create a .env file in the root directory
   echo "OPENROUTER_API_KEY=your_api_key_here" > .env
   ```

4. **Start the development server**
   ```bash
   npm run dev
   ```

5. **Open your browser**
   Navigate to `http://localhost:5000` and start creating amazing mind maps!

## 🎨 Visual Design

The application features a stunning visual design with:

- **Animated Gradient Backgrounds**: Dynamic color shifting between purple, pink, blue, cyan, yellow, and orange
- **Glass-Morphism Effects**: Translucent cards with backdrop blur for a modern look
- **3D Hover Transformations**: Interactive elements that respond to user interaction
- **Floating Animations**: Background elements that gently float across the screen
- **Neon Glows**: Vibrant lighting effects on key components
- **Gradient Text**: Beautiful color transitions in typography

## 🔧 Configuration

### OpenRouter API Setup
1. Visit [OpenRouter.ai](https://openrouter.ai/)
2. Create a free account
3. Generate an API key from your dashboard
4. Add it to your environment variables as `OPENROUTER_API_KEY`

### Customization
- Modify colors in `client/src/index.css` CSS variables
- Adjust animations and effects in the same file
- Update AI prompts in `server/routes.ts`

## 📁 Project Structure

```
├── client/                 # Frontend React application
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── hooks/          # Custom React hooks
│   │   ├── lib/            # Utility libraries
│   │   ├── pages/          # Application pages
│   │   └── App.tsx         # Main app component
├── server/                 # Backend Express server
│   ├── index.ts           # Server entry point
│   ├── routes.ts          # API routes
│   └── storage.ts         # Data storage interface
├── shared/                 # Shared types and schemas
│   └── schema.ts          # Zod validation schemas
└── README.md              # This file
```

## 🎯 Usage

1. **Enter a Topic**: Type any subject you want to explore (e.g., "Climate Change", "Quantum Physics")
2. **Generate**: Click the "Generate Mind Map" button or try an example
3. **Explore**: Interact with the generated mind map - zoom, pan, and explore connections
4. **Export**: Use the toolbar to export your mind map (feature in development)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [OpenRouter](https://openrouter.ai/) for AI API access
- [Mind-Elixir](https://github.com/ssshooter/mind-elixir-core) for mind map visualization
- [shadcn/ui](https://ui.shadcn.com/) for beautiful components
- [Tailwind CSS](https://tailwindcss.com/) for styling utilities

## 🐛 Issues & Support

If you encounter any issues or have questions:
1. Check the [Issues](https://github.com/yourusername/ai-mindmap-generator/issues) page
2. Create a new issue with detailed information
3. Include screenshots if relevant

---

**Made with ❤️ and AI magic**