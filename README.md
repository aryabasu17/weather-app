# Simple Weather App

A modern, responsive weather application built with React that provides real-time weather information for cities worldwide. Get current weather conditions, forecasts, and detailed meteorological data with a clean, intuitive interface.

## Features

- **City Search**: Search for weather information by city name with real-time results
- **Current Weather Display**: View current temperature, weather conditions, and descriptive icons
- **Detailed Weather Information**: Access comprehensive data including:
  - Wind speed and direction
  - Minimum and maximum temperatures
  - Humidity levels
  - Atmospheric pressure
  - Sunrise and sunset times
- **Responsive Design**: Optimized for desktop and mobile devices with adaptive layouts
- **Interactive Elements**: Horizontal scrollable weather details on mobile devices
- **Weather Icons**: Dynamic SVG icons representing current weather conditions
- **City Information**: Direct links to Wikipedia for additional city information
- **Real-time Updates**: Fresh weather data from OpenWeatherMap API

## Installation

Follow these steps to run the weather app locally:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/aryabasu17/weather-app.git
   cd weather-app
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Start the development server**:
   ```bash
   npm start
   ```

4. **Open your browser** and navigate to [http://localhost:3000](http://localhost:3000)

The app will automatically reload when you make changes to the code.

## Usage

1. **Search for a City**: Enter a city name in the search box at the top of the application
2. **View Weather Data**: The app will display current weather conditions including temperature, description, and weather icon
3. **Explore Details**: Scroll through additional weather information including wind speed, humidity, pressure, and sunrise/sunset times
4. **Mobile Navigation**: On mobile devices, use the arrow buttons or swipe to navigate through weather details
5. **City Information**: Click the external link icon next to the city name to view more information on Wikipedia

## API Configuration

This application uses the OpenWeatherMap API to fetch weather data. To set up your own API key:

1. **Get an API Key**:
   - Visit [OpenWeatherMap](https://openweathermap.org/api)
   - Sign up for a free account
   - Generate your API key

2. **Configure the API Key**:
   - Open `src/components/Main.js`
   - Locate line 14: `const APP_KEY = "4f34b1df244dd43f543c494d754e0147";`
   - Replace the existing key with your new API key:
     ```javascript
     const APP_KEY = "your-api-key-here";
     ```

3. **Save the file** and restart the development server

**Note**: The current API key is for demonstration purposes. For production use, consider using environment variables to secure your API key.

## Project Structure

```
weather-app/
├── public/
│   ├── assets/               # Weather condition SVG icons
│   ├── index.html           # Main HTML template
│   └── manifest.json        # PWA manifest
├── src/
│   ├── components/
│   │   ├── Main.js          # Main component with search and API logic
│   │   ├── WeatherData.js   # Weather display component
│   │   ├── search.svg       # Search icon
│   │   └── external-link.svg # External link icon
│   ├── App.js               # Root application component
│   ├── index.js             # Application entry point
│   └── index.css            # Global styles and responsive design
├── package.json             # Dependencies and scripts
└── README.md               # Project documentation
```

### Key Files

- **`src/components/Main.js`**: Contains the main application logic, API calls, search functionality, and state management
- **`src/components/WeatherData.js`**: Handles the display of weather information, including current conditions and detailed metrics
- **`src/index.css`**: Comprehensive styling including responsive design, gradient backgrounds, and mobile optimizations
- **`public/assets/`**: Collection of SVG icons representing different weather conditions (sunny, cloudy, rainy, etc.)

## Contributing

We welcome contributions to improve the Simple Weather App! Here's how you can help:

1. **Fork the repository** on GitHub
2. **Create a feature branch**: `git checkout -b feature/your-feature-name`
3. **Make your changes** and ensure they follow the existing code style
4. **Test your changes** thoroughly
5. **Commit your changes**: `git commit -m "Add your descriptive commit message"`
6. **Push to your branch**: `git push origin feature/your-feature-name`
7. **Open a Pull Request** with a clear description of your changes

### Development Guidelines

- Follow React best practices and hooks patterns
- Maintain responsive design principles
- Test on both desktop and mobile devices
- Keep API calls efficient and handle errors gracefully
- Update documentation for any new features

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

**Built with ❤️ by Arya Basu**

For questions or support, please open an issue on GitHub.
