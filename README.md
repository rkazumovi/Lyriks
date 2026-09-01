# 🎵 Lyriks

A modern, Spotify-inspired music streaming web app that lets users discover trending songs, explore top artists and charts, search for music, and listen through a built-in audio player — all wrapped in a clean, responsive interface.

🌐 **Live Demo:** [lyriks-music-app-site.netlify.app](https://lyriks-music-app-site.netlify.app/)
📂 **Repository:** [github.com/rkazumovi/Lyriks](https://github.com/rkazumovi/Lyriks)

![React](https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=black)
![Redux Toolkit](https://img.shields.io/badge/Redux%20Toolkit-1.8-764ABC?logo=redux&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-2-646CFF?logo=vite&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3-38B2AC?logo=tailwindcss&logoColor=white)

---

## Overview

Lyriks provides a modern music discovery experience inspired by platforms like Spotify. Users can browse curated music sections, discover trending tracks, explore artists and regional charts, search for songs, and play tracks directly in the app through a persistent audio player with full playback controls.

All music data is sourced live from the **Shazam Core API**, with API calls managed through RTK Query for efficient caching and data fetching.

## ✨ Features

- 🎵 Discover trending songs and curated recommendations
- 🌍 "Around You" — explore tracks trending by country/location
- 📈 Top Charts — browse chart-topping hits worldwide
- 🎤 Top Artists — explore popular artists and their discographies
- 🔍 Search for songs and artists in real time
- ▶️ Built-in music player with play/pause, seek bar, volume control, and track info
- 🔁 Related songs suggestions on each track's detail page
- 📱 Fully responsive design across desktop, tablet, and mobile
- ⚡ Fast, dynamic content loading with loading and error states

## 🏗️ Core Sections

| Section | Description |
|---|---|
| **Discover** | Browse popular songs and new music recommendations |
| **Around You** | Explore music trending in different regions/countries |
| **Top Charts** | View trending songs and chart-topping hits |
| **Top Artists** | Discover popular artists and explore their music |
| **Search** | Search for songs, artists, and music content |
| **Song / Artist Details** | Dedicated detail pages with related songs and artist info |

## 🛠️ Built With

**Languages**
- JavaScript (JSX) — application logic and components
- CSS — styling via Tailwind CSS
- HTML — base document markup

**Frameworks / Libraries**
- [React](https://react.dev/) 18 — UI library
- [React Router](https://reactrouter.com/) 6 — client-side routing
- [Redux Toolkit](https://redux-toolkit.js.org/) — global state management
- [RTK Query](https://redux-toolkit.js.org/rtk-query/overview) — API data fetching and caching
- [React Redux](https://react-redux.js.org/) — React bindings for Redux
- [Axios](https://axios-http.com/) — HTTP client
- [Swiper](https://swiperjs.com/) — touch-enabled carousels/sliders
- [React Icons](https://react-icons.github.io/react-icons/) — icon library
- [Tailwind CSS](https://tailwindcss.com/) — utility-first styling

**External API**
- [Shazam Core API](https://rapidapi.com/) (via RapidAPI) — music charts, search, artist, and track data

**Build Tools & Tooling**
- [Vite](https://vitejs.dev/) — build tool and dev server
- [PostCSS](https://postcss.org/) + [Autoprefixer](https://github.com/postcss/autoprefixer) — CSS processing
- [ESLint](https://eslint.org/) (Airbnb config) — linting and code consistency

**Deployment**
- [Netlify](https://www.netlify.com/) — hosting and continuous deployment

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or later recommended)
- npm or yarn
- A [RapidAPI](https://rapidapi.com/) account with access to the Shazam Core API and a Geo API key

### Installation

1. Clone the repository
   ```bash
   git clone https://github.com/rkazumovi/Lyriks.git
   cd Lyriks
   ```

2. Install dependencies
   ```bash
   npm install
   ```

3. Configure environment variables

   Create a `.env` file in the project root based on `.env.example`:
   ```
   VITE_SHAZAM_CORE_RAPID_API_KEY=your_rapidapi_key
   VITE_GEO_API_KEY=your_geo_api_key
   ```

4. Start the development server
   ```bash
   npm run dev
   ```

5. Open your browser and navigate to `http://localhost:3000` (or the port shown in your terminal)

### Build for Production

```bash
npm run build
```

### Preview the Production Build

```bash
npm run preview
```

## 📁 Project Structure

```
Lyriks/
├── public/
├── src/
│   ├── assets/               # Static assets, constants, icons
│   ├── components/           # Reusable UI components
│   │   └── MusicPlayer/      # Player, controls, seek bar, volume bar
│   ├── pages/                # Route-level pages (Discover, Search, TopCharts, etc.)
│   ├── redux/
│   │   ├── features/         # Redux slices (e.g. player state)
│   │   ├── services/         # RTK Query API service (Shazam Core)
│   │   └── store.js          # Redux store configuration
│   ├── App.jsx
│   └── index.jsx
├── .env.example
├── tailwind.config.js
├── postcss.config.js
├── vite.config.js
└── package.json
```

## 📱 Responsive Design

The application is fully responsive and optimized for desktop, tablet, and mobile screen sizes.

## 📦 Deployment

This project is deployed with **Netlify** and is live at:
👉 [lyriks-music-app-site.netlify.app](https://lyriks-music-app-site.netlify.app/)

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

1. Fork the repository
2. Create your feature branch
   ```bash
   git checkout -b feature/new-feature
   ```
3. Commit your changes
   ```bash
   git commit -m "Add new feature"
   ```
4. Push to the branch
   ```bash
   git push origin feature/new-feature
   ```
5. Open a Pull Request

## 📄 License

This project is intended for educational and portfolio purposes. Music data is provided via the Shazam Core API through RapidAPI and is subject to that service's terms of use.

---

<p align="center">⭐ If you found this project interesting, consider giving it a star on GitHub!</p>
