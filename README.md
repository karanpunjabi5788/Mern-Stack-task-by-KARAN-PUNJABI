# MERN Stack Backend Task

This project is the backend part of a MERN stack challenge using Node.js, Express, and MongoDB.

## Features

- Fetch and store transaction data from a third-party API
- List transactions with search and pagination
- Generate statistics for a selected month
- Create bar chart and pie chart data
- Combined endpoint for all stats

## Setup Instructions

1. Clone the repo or unzip this folder.
2. Make sure MongoDB is running locally or set your MongoDB URI in `.env`.
3. Install dependencies:
   ```
   npm install
   ```
4. Run the server:
   ```
   npm start
   ```
5. Hit `/api/initialize` once to load data into your database.

## Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/initialize` | Seed database with sample data |
| GET | `/api/transactions?month=March&search=&page=1` | List transactions |
| GET | `/api/statistics?month=March` | Show summary statistics |
| GET | `/api/barchart?month=March` | Bar chart data |
| GET | `/api/piechart?month=March` | Pie chart data |
| GET | `/api/combined?month=March` | Combined API response |

## Note

- The month filter works regardless of the year.
- You can update the MongoDB connection string in the `.env` file.

---

Built with ❤️ by Karan Punjabi
