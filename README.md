# Trading App

This application provides real-time data for various company stocks, helping users make informed decisions on buying and selling. The app sends buy or sell signals based on user-defined criteria and calculates stock costs when a signal is triggered.

![Screenshot](./output.png)

## Features

- Real-time stock price monitoring
- Buy/sell signal generation based on user criteria
- Stock cost calculation at signal generation
- Profit/loss percentage calculation

## Project Structure

The Trading App consists of several key components:

- `curl_functions`: Handles HTTP requests to fetch stock data from an external API
- `functions`: Contains the core trading logic and data processing functions
- `main.cpp`: The main entry point and user interaction handler
- `config.json`: Stores the API key for accessing external data sources

## Getting Started

1. Clone this repository:
   ```
   git clone https://github.com/iharsh17/cpp-trading-app
   ```

2. Navigate to the project folder.
   ```
   cd cpp-trading-app
   ```

3. Compile the application:
   ```
   g++ -o trading_app main.cpp curl_functions.cpp functions.cpp -lcurl -ljsoncpp
   ```

4. Run the compiled application:
   ```
   ./trading_app
   ```

## Prerequisites

Before running the Trading App, ensure you have:

- curl library installed
- JsonCpp library installed
- An API key from Twelve Data (place it in `config.json`)

## Future Improvements

- Implement additional trading strategies
- Add a user-friendly GUI
- Integrate with multiple data sources for more comprehensive analysis

Feel free to contribute or suggest improvements!
