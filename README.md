# Simple Weather App

A modern, responsive weather application built with React that provides real-time weather information for any city worldwide. The app features a clean, user-friendly interface with gradient backgrounds and intuitive weather data visualization.

## Features

- **City Search**: Search for weather information by city name with real-time results
- **Current Weather Display**: Shows temperature, weather description, and weather icons
- **Detailed Weather Information**: Displays humidity, wind speed, pressure, and feels-like temperature
- **Sunrise/Sunset Times**: View sunrise and sunset times for the selected city
- **Responsive Design**: Fully responsive layout that works seamlessly on desktop and mobile devices
- **Interactive Interface**: Click-to-search functionality with Enter key support
- **Weather Icons**: Beautiful weather icons that represent current conditions
- **Error Handling**: Graceful error handling for invalid city names
- **Horizontal Scrolling**: Mobile-friendly horizontal scrolling for weather details

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/aryabasu17/weather-app.git
   cd weather-app
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Set up the API key** (see API Configuration section below)

4. **Start the development server:**
   ```bash
   npm start
   ```

5. **Open your browser** and navigate to `http://localhost:3000`

## Usage

1. **Search for a city**: Type the name of any city in the search bar
2. **View weather data**: The app will display current temperature, weather conditions, and detailed information
3. **Explore details**: Scroll horizontally (on mobile) or view the detailed weather panel to see additional information like humidity, wind speed, and sunrise/sunset times
4. **Try different cities**: Search for multiple cities to compare weather conditions

## API Configuration

This app uses the OpenWeatherMap API to fetch weather data. You need to set up your own API key:

1. **Get an API key:**
   - Visit [OpenWeatherMap](https://openweathermap.org/api)
   - Sign up for a free account
   - Generate your API key from the dashboard

2. **Configure the API key:**
   - Open `src/components/Main.js`
   - Find the line: `const APP_KEY = "4f34b1df244dd43f543c494d754e0147";`
   - Replace the existing key with your own API key:
     ```javascript
     const APP_KEY = "YOUR_API_KEY_HERE";
     ```

3. **Save and restart** the development server for changes to take effect

## Project Structure

```
weather-app/
├── public/
│   ├── assets/           # Weather icons and images
│   ├── index.html        # Main HTML template
│   └── manifest.json     # PWA manifest
├── src/
│   ├── components/
│   │   ├── Main.js       # Main component with search and API logic
│   │   └── WeatherData.js # Weather data display component
│   ├── App.js            # Root React component
│   ├── index.js          # React DOM entry point
│   └── index.css         # Global styles and responsive design
├── package.json          # Dependencies and scripts
└── README.md            # Project documentation
```

### Key Files

- **`src/components/Main.js`**: Contains the main application logic, including city search functionality, API calls to OpenWeatherMap, and state management
- **`src/components/WeatherData.js`**: Handles the display of weather information, including temperature, weather conditions, and additional details
- **`src/index.css`**: Contains all styling for the application, including responsive design and gradient backgrounds
- **`public/assets/`**: Stores weather icons used throughout the application

## Contributing

We welcome contributions to improve the Simple Weather App! Here's how you can help:

1. **Fork the repository** on GitHub
2. **Create a feature branch**: `git checkout -b feature/your-feature-name`
3. **Make your changes** following the existing code style
4. **Test your changes** thoroughly
5. **Commit your changes**: `git commit -m "Add your feature description"`
6. **Push to your branch**: `git push origin feature/your-feature-name`
7. **Open a Pull Request** with a clear description of your changes

### Development Guidelines

- Follow React best practices and hooks patterns
- Maintain responsive design compatibility
- Test on both desktop and mobile devices
- Keep API keys secure and configurable
- Write clear, descriptive commit messages

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

**Built with ❤️ by Arya Basu**
