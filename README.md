# Cryptocurrency Trend Monitor

The Cryptocurrency Trend Monitor is a web-based script that fetches OHLCV (Open, High, Low, Close, Volume) data from the Binance API and analyzes the trend of a specified cryptocurrency pair. It calculates moving averages, detects the trend as upward, downward, or in a range, and provides real-time updates on the latest price and trend. Optional sound alerts are available for different trend types. Additionally, the script calculates Fibonacci levels based on the high and low prices.

## Features

- Fetches OHLCV data for a specified cryptocurrency pair from the Binance API.
- Calculates moving averages for different periods to analyze the trend.
- Detects whether the trend is upward, downward, or in a range.
- Calculates Fibonacci levels based on the high and low prices.
- Displays the latest price and time of the cryptocurrency pair.
- Provides optional sound alerts for different trend types: upward trend, downward trend, and range.

## Usage

1. Clone the repository or download the script file.

2. Ensure that you have the necessary audio files in the same directory as the HTML file:
   - `buy.mp3` for the upward trend alert
   - `sell.mp3` for the downward trend alert
   - `range.mp3` for the range alert

3. Open the HTML file (`index.html`) in a web browser.

4. The script will start monitoring the cryptocurrency trend automatically and display the latest price, time, and detected trend in the specified HTML element with the ID `result`.

5. Sound alerts will be triggered based on the detected trend:
   - Upward trend: Plays the `buy.mp3` sound file.
   - Downward trend: Plays the `sell.mp3` sound file.
   - Range: Plays the `range.mp3` sound file.

6. The script will continue monitoring the trend every minute (adjustable via the `setInterval` function in the script) and update the information accordingly.

7. Fibonacci levels are calculated based on the high and low prices of the fetched data. These levels are not displayed in the provided HTML element but can be accessed through the `calculateFibonacciLevels` function in the script.

## Requirements

- Web browser with JavaScript support.
- Internet connection to fetch data from the Binance API.

## Notes

- The script uses the Binance API to fetch OHLCV data. If you encounter any issues with the API, please ensure that you have a stable internet connection and check the API documentation for any updates or changes.

- Sound playback may be subject to browser restrictions or user settings. If the sound alerts are not playing, check your browser settings related to audio autoplay and ensure that the audio files are in a compatible format (e.g., MP3).

## License

This script is released under the [MIT License](LICENSE).
