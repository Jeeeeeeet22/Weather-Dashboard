# Weather Dashboard

A modern weather dashboard application built with React, TypeScript, and Tailwind CSS.

## Features

- Real-time weather data for any city
- Clean, responsive UI with dark mode support
- Recent search history
- Loading states and error handling
- Beautiful animations with Framer Motion

## Tech Stack

- React + TypeScript
- Vite
- Tailwind CSS
- Framer Motion
- Axios
- React Hot Toast

## Setup Instructions

1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file in the root directory:
   ```
   VITE_OPENWEATHER_API_KEY=your_api_key_here
   VITE_API_BASE_URL=https://api.openweathermap.org/data/2.5
   ```
4. Start the development server:
   ```bash
   npm run dev
   ```

## Deployment

### Vercel Deployment

1. Sign up for a [Vercel](https://vercel.com) account
2. Install Vercel CLI:
   ```bash
   npm install -g vercel
   ```
3. Login to Vercel:
   ```bash
   vercel login
   ```
4. Deploy:
   ```bash
   vercel
   ```

### Environment Variables in Vercel

1. Go to your project settings in Vercel
2. Navigate to the "Environment Variables" section
3. Add the following variables:
   - `VITE_OPENWEATHER_API_KEY`: Your OpenWeather API key
   - `VITE_API_BASE_URL`: https://api.openweathermap.org/data/2.5

### GitHub Pages Deployment

1. Install gh-pages:
   ```bash
   npm install --save-dev gh-pages
   ```
2. Add the following to your package.json:
   ```json
   "homepage": "https://yourusername.github.io/weather-dashboard",
   "scripts": {
     "predeploy": "npm run build",
     "deploy": "gh-pages -d dist"
   }
   ```
3. Deploy:
   ```bash
   npm run deploy
   ```

## API Integration

This project uses the OpenWeatherMap API:
- Base URL: https://api.openweathermap.org/data/2.5
- Rate Limit: 60 calls/minute for free tier
- API Key: Required (get one from [OpenWeatherMap](https://openweathermap.org/api))

## License

MIT
