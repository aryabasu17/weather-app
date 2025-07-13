# Simple Weather App

A lightweight, responsive weather application built with React that allows users to search for the current weather in any city using live data from a weather API.

## Features

- **Search by City:** Enter any city to retrieve current weather information.
- **Weather Details:** Displays temperature, humidity, wind speed, and general conditions.
- **Responsive Design:** Works seamlessly on desktops, tablets, and mobile devices.
- **Error Handling:** Notifies users if a location isn't found or the API fails.

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

3. **Run the app:**
   ```bash
   npm start
   ```
   Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

## Usage

- Enter a city name in the search box and press the search button or hit Enter.
- The app will display the current weather data for the specified city.

## API Configuration

This app uses OpenWeatherMap API for weather data.  
The API key is already configured in the source code, but you can replace it with your own:

1. Sign up at [OpenWeatherMap](https://openweathermap.org/) and get your API key.
2. Open `src/components/Main.js` and replace the API key in the `APP_KEY` constant:
   ```javascript
   const APP_KEY = "YOUR_API_KEY_HERE";
   ```

## Project Structure

- `public/index.html` – Main HTML file and entry point.
- `src/App.js` – Main React component.
- `src/components/Main.js` – Main weather component handling API calls and user interactions.
- `src/components/WeatherData.js` – Component for displaying weather information.
- `src/index.css` – Styles for layout and responsiveness.

## Available Scripts

In the project directory, you can run:

### `npm start`
Runs the app in development mode at [http://localhost:3000](http://localhost:3000).

### `npm test`
Launches the test runner in interactive watch mode.

### `npm run build`
Builds the app for production to the `build` folder.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

1. Fork the repo
2. Create your feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a pull request

## License

This project is licensed under the MIT License.
