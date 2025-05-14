# Coding challenge

Build a small analytics program that helps determine the best hour(s) of the day to consume electricity based on spot prices and ambient temperature.

Use gi

### Data folder

In the `/data` folder:

- `spot_prices.json` – Hourly electricity prices
- `temperature.csv` – Temperature data for Oulu (3-minute intervals)

### Api resources

- **Spot prices**: [https://sahkotin.fi/api](https://sahkotin.fi/prices?fix&vat&start=2024-12-31T22:00:00.000Z)
- **Weather data**: [OpenWeather One Call API](https://openweathermap.org/api/one-call-3) (free tier available)
  - Use free access /pricing -> scroll down to Free access https://home.openweathermap.org/users/sign_up
  - It might take a couple of hours for the api key to get activated

## Tech

Use any technology you prefer to complete the challenge (e.g. Python, .NET, React, Material UI, shadcn, etc.).

## Choose One of Two Options

## Option 1 - Fullstack

- Create an API endpoint that:
  - Reads the data provided in data folder
    - Create one api endpoint where you can search for data for a specific date.
    - Aggregate the 3-minute temperature readings into hourly average temperatures.
- Create another endpoint that:
  - Returns data for a specific date
- UI should:
  - Display a list of all hours with: **Date**, **Hour**, **Spot Price**, and **Average Temperature**

## Option 2 - Frontend

- Use the provided public APIs
- Use your **current location** to fetch weather data
- Build a UI that:
  - Visualizes spot price vs. temperature (e.g. charts, graphs)
  - Displays the **highest and lowest spot prices** for a selected date in cards
  - Displays temperature for that date
  - Allows the user to select a date

### Optional

- Implement authentication (e.g. JWT, session-based, OAuth)
- Add filtering by date, time range, or price range
- Allow exporting results as CSV or JSON
- Highlight the cheapest/best hours using a custom scoring model
- Implement a test

## Time tracking

- Track your time and how much time you have been spending on it.

## Side note

This is a coding challenge, and we don’t expect you to spend excessive unpaid time on it. Please don’t aim for perfection or try to complete every optional feature. We’re more interested in how you approach the problem, structure your code, and communicate your thinking than in pixel-perfect results.

## Version Control

Please:

- Use **Git** to version control your project
- Push your solution to a repo on your own github account
- Follow **[Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)** for commit messages (e.g., `feat: add chart to visualize spot prices`)
