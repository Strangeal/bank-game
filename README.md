# Stock Market Game

## Overview

This project is a small "serious game" developed for a bank to educate users about the basics and risks of stock trading in a playful way. The game simulates a stock market environment where users can experience stock trading, including the potential for market crashes.

## Features

### User Authentication

- **Registration**: Users can create an account to participate in the game.
- **Login**: Users can log in to access their account and continue their trading activities.
- **Logout**: Users can log out, which clears their session and removes their details from local storage.

### Trading Functionality

- **Depot Holdings**: Displays the user's current play money balance, current profit/loss, current depot holdings, and the number of shares owned.
- **Share Price Overview**: Shows the prices of the ten tradable shares.
- **Detailed Share View**: Provides detailed information about a share, including prices from the last ten days.
- **Order Book**: Displays all purchases and sales made by the user.

### Stock Market Crash Simulation

- **Market Volatility Alert**: When the market becomes volatile and poses a risk of crashing, an alert is displayed on the screen.
- **User Decision**: The alert provides buttons for users to either sell their stocks or hold them, allowing them to make strategic decisions during market volatility.

## Tech Stack

- **Frontend**: React, Next.js
- **Backend**: PHP

## Getting Started

### Prerequisites

- Node.js
- npm or yarn

### Installation

1. Clone the repository:
   ```sh
   git clone git@github.com:Strangeal/bank-game.git
   ```
2. Navigate to the project directory:
   ```sh
   cd bank-game
   ```
3. Install dependencies:
   ```sh
   npm install
   ```
   or
   ```sh
   yarn install
   ```

### Running the Application

1. Start the development server:
   ```sh
   npm run dev
   ```
   or
   ```sh
   yarn dev
   ```
2. Open your browser and navigate to `http://localhost:3000`.

## Project Structure

- **components**: Contains reusable UI components such as buttons, navigation menus, and stock-related components.
- **hooks**: Custom hooks for managing authentication and other stateful logic.
- **pages**: Next.js pages for different routes, including the trading page and authentication pages.
- **utils**: Utility functions for various calculations and formatting.
- **types**: TypeScript types for defining the shape of data used in the application.

## Authentication

The application uses basic authentication without sessions or tokens. User details are stored in local storage to persist login state. When a user logs in, their details are saved in local storage, and when they log out, the details are cleared.

## Protecting Routes

The trading route is protected to ensure only authenticated users can access it. If a user is not logged in, they are redirected to the login page.

## Stock Market Simulation

The game simulates stock trading with the following features:

- **Stock Price Updates**: Stock prices are updated at regular intervals, with a small chance of a market crash.
- **Market Crash Alert**: When a market crash is imminent, an alert is displayed, allowing users to decide whether to sell their stocks or hold them.
- **Trading Actions**: Users can buy and sell shares, with their actions reflected in their depot holdings and order book.

## Conclusion

This project provides an educational and interactive way for users to learn about stock trading and the risks involved. By simulating a stock market environment, users can experience the dynamics of trading and make strategic decisions during market volatility.
