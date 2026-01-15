<div align="center">
  <img src="resources/images/logo.jpeg" alt="Community Heritage Memorial Project Logo" width="400" />

  # Community Heritage Memorial Project

  **Preserving memories, connecting communities through AI-powered storytelling**

  [![React](https://img.shields.io/badge/React-19.2.3-61DAFB?logo=react)](https://reactjs.org/)
  [![TypeScript](https://img.shields.io/badge/TypeScript-5.8.2-3178C6?logo=typescript)](https://www.typescriptlang.org/)
  [![Vite](https://img.shields.io/badge/Vite-6.2.0-646CFF?logo=vite)](https://vitejs.dev/)
  [![Google Gemini](https://img.shields.io/badge/Google_Gemini-AI-4285F4?logo=google)](https://ai.google.dev/)
</div>

---

## 📖 Overview

The **Community Heritage Memorial Project** is an AI-powered platform designed to preserve and celebrate community heritage through advanced storytelling, historical narrative generation, and interactive visualizations. Built with React and powered by Google's Gemini AI, this project creates meaningful connections between past and present, honoring memories while making them accessible to future generations.

### Key Capabilities

- **🎬 Synthetic Story Generation**: Transform static historical images into dynamic video narratives using Gemini's Veo model
- **💬 Talk With the Past**: Interactive AI conversations that bring historical figures and memories to life
- **🔍 AI-Powered Image Analysis**: Automatically generate descriptions and context for historical photographs
- **🌐 Knowledge Graph Visualization**: Interactive D3.js network graphs showing relationships between people, places, and events
- **🏛️ Institutional & Geographic Connections**: Track heritage across countries and institutions
- **📱 Augmented Reality Features**: Experience history in immersive new ways

---

## 🚀 Quick Start

### Prerequisites

- **Node.js** (v18 or higher)
- **Google Gemini API Key** ([Get one here](https://makersuite.google.com/app/apikey))

### Installation

1. **Clone and install dependencies:**
   ```bash
   npm install
   ```

2. **Configure your API key:**
   Create a `.env` file in the project root:
   ```bash
   VITE_GEMINI_API_KEY=your_api_key_here
   ```

3. **Run the development server:**
   ```bash
   npm run dev
   ```

   Open [http://localhost:5173](http://localhost:5173) in your browser.

### Build for Production

```bash
npm run build
npm run preview  # Preview the production build
```

### Package for Distribution

```bash
npm run package        # Full package with compression
npm run package:quick  # Quick package without optimization
```

---

## 🎨 Features

### 1. Cinematic Video Background
A stunning 4×3 grid video collage with subtle parallax scrolling (5% scroll speed) that creates an immersive, emotional atmosphere. Videos automatically loop and include hover effects for enhanced interactivity.

### 2. AI-Powered Storytelling
- **Image to Narrative**: Upload historical photos and let Gemini AI generate respectful, contextual narratives
- **Video Generation**: Transform static images into 2-3 second video clips with camera movements
- **Historical Context**: AI provides detailed analysis of clothing, architecture, time periods, and cultural significance

### 3. Interactive Knowledge Graph
Live D3.js force-directed graph visualization that displays:
- Community connections and relationships
- Geographic distribution across countries
- Institutional affiliations
- Temporal connections across generations

### 4. Talk With the Past
Conversational AI interface allowing visitors to:
- Ask questions about historical events
- Learn about individuals and their stories
- Explore cultural heritage through dialogue

### 5. Multi-Platform Architecture
- **React Application**: Full-featured interactive experience
- **Marketing Page** ([marketing.html](marketing.html)): Standalone demo requiring no API keys
  - Works completely offline
  - Interactive feature demonstrations
  - Self-contained HTML with embedded styles

---

## 📁 Project Structure

```
community-heritage-memorial-project/
├── components/
│   ├── Hero.tsx                  # Landing section with video background
│   ├── VideoBackground.tsx       # Reusable video collage component
│   ├── SyntheticStory.tsx        # AI video generation interface
│   ├── TalkWithPast.tsx          # Conversational AI interface
│   ├── KnowledgeGraphViz.tsx     # D3.js network visualization
│   ├── AugmentedReality.tsx      # AR features
│   ├── Countries.tsx             # Geographic connections
│   └── Institutions.tsx          # Institutional affiliations
├── resources/
│   ├── original/                 # Place source images here for AI processing
│   ├── videos/stories/           # Video clips for background collage (9 videos)
│   └── images/
│       └── logo.jpeg             # Project logo
├── App.tsx                       # Main application component
├── marketing.html                # Standalone marketing page
├── package.json
└── README.md
```

---

## 🛠️ Technology Stack

### Frontend
- **React 19.2.3** - Modern UI library with concurrent features
- **TypeScript 5.8.2** - Type-safe development
- **Tailwind CSS 4.1.18** - Utility-first styling
- **Vite 6.2.0** - Lightning-fast build tool

### AI & Data Visualization
- **@google/genai** - Google Gemini AI integration
- **D3.js 7.9.0** - Interactive data visualizations

### Development Tools
- **PostCSS** with Autoprefixer
- **Vite Plugin React** for Fast Refresh

---

## 🎥 Video Background Setup

The video collage background requires **9 video files** placed in:
```
resources/videos/stories/
```

**Specifications:**
- Grid: 4×3 on desktop, 3×3 on mobile
- Format: MP4, WebM (recommended for web)
- Performance: 60fps smooth scrolling via `requestAnimationFrame`
- Effects: Grayscale with brightness hover effect

---

## 🔒 Environment Variables

Create a `.env` file with:

```bash
# Required: Google Gemini API Key
VITE_GEMINI_API_KEY=your_key_here
```

> **Important:** Never commit your `.env` file. It's already in `.gitignore`.

---

## 📦 Deployment

### Option 1: Static Hosting (Recommended)
```bash
npm run build
```
Deploy the `dist/` folder to:
- [Vercel](https://vercel.com)
- [Netlify](https://netlify.com)
- [GitHub Pages](https://pages.github.com)
- Any static hosting service

### Option 2: Package for Self-Hosting
```bash
npm run package
```
Generates `memorial-heritage-project.tar.gz` containing:
- Optimized production build
- All required resources
- Ready for deployment on any web server

---

## 🤝 Contributing

Contributions are welcome! This project is designed to help communities preserve their heritage. Whether you're adding features, improving documentation, or fixing bugs, your help is appreciated.

---

## 📄 License

This project is part of the Community Heritage Memorial initiative. Please respect the sensitive nature of historical content and handle all materials with appropriate dignity.

---

## 🙏 Acknowledgments

- **Google Gemini AI** for powering intelligent narrative generation
- **D3.js** community for visualization tools
- **React** team for an exceptional development experience
- All contributors working to preserve community heritage

---

<div align="center">

  **Preserving the past, inspiring the future**

  Made with ❤️ for communities worldwide

</div>
