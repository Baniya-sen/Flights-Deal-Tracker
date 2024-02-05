# Flight Deal Tracker

Welcome to the Flight Deal Tracker project! This tool searches for the cheapest flights from a specified origin city to various destinations within a given budget and time frame.

![Notification Example](https://github.com/Baniya-sen/Flights-Deal-Tracker/assets/144620117/b9fe43af-d494-4016-a356-c81ea298365b)

## Project Overview

This project utilizes Google Sheets and Sheety API to gather destination data and search for flight deals. It iterates through each destination specified in the Google Sheet, searching for flights within a specified time range and budget.

## Getting Started

To use this project, follow these steps:

1. **Install Requirements**:
   - First, install the required Python packages by running:
     ```bash
     pip install -r requirements.txt
     ```

2. **Update Environmental Variables**:
   - Update the environmental variables for the Tequila API and Sheety API in the `.env` file:
     - `TEQUILA_API_KEY`: Get your API key from [Tequila API](https://tequila.kiwi.com/)
     - `SHEETY_API_ENDPOINT`: Update the Sheety API endpoint for your Google Sheet [SHEETY API](https://sheety.co/)
     - Ensure you have permissions set up correctly for accessing the Google Sheet.

3. **Customization**:
   - Open `main.py` and update the `ORIGIN_CITY_IATA` constant with your preferred departure city's IATA code.
   - Customize other parameters as needed, such as currency or date range.

4. **Run the Program**:
   - Execute the `main.py` script to search for flight deals:
     ```bash
     python main.py
     ```

5. **Google Sheet Setup**:
   - Create a copy of the [Google Sheet](https://docs.google.com/spreadsheets/d/1Kv0B_DU7E3W5n5VU6kVU05M7fGr8TgGQHlcZHnrIkIU/copy) with your account and use your sheet link with Sheety API to fetch destination data for the project.

## Notes
- The `ORIGIN_CITY_IATA` constant in `main.py` defines the departure city's IATA code. Update it to set flights 'from' your preferred city.
- The project utilizes Google Sheets and Sheety API to fetch destination data and search for flights. Ensure you update the environmental variables with the correct API keys and endpoints.
- The script searches for flights from tomorrow to 6 months after and sends notifications via email and SMS if a flight within the specified budget is found.

## Screenshots

After running output should look like this-
![Results Example](https://github.com/Baniya-sen/Flights-Deal-Tracker/assets/144620117/67153d1a-d588-4e4b-9fd0-2538ad9e970f)
![Results Finding](https://github.com/Baniya-sen/Flights-Deal-Tracker/assets/144620117/92457424-1585-4507-a23b-64c46bdd7d31)
