# ShopFinder

A web application for finding and discovering local shops and businesses.

## Features

- User authentication (login/register)
- Search for nearby shops
- Filter by category and distance
- Sort by rating or distance
- Interactive map view
- Premium shop highlights
- Advanced features page

## Prerequisites

- Node.js (v14 or higher)
- Python (v3.7 or higher)
- FastAPI
- SQLite

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd shopfinder
```

2. Install frontend dependencies:
```bash
npm install
```

3. Install backend dependencies:
```bash
pip install fastapi uvicorn passlib sqlite3
```

4. Set up the database:
```bash
python setup_db.py
```

5. Add your Google Maps API key:
   - Open `src/pages/main.html`
   - Replace `YOUR_API_KEY` with your actual Google Maps API key

## Running the Application

1. Start the backend server:
```bash
python app.py
```
The backend will run on http://localhost:8000

2. Start the frontend development server:
```bash
npm run dev
```
The frontend will run on http://localhost:5173

## Project Structure

```
shopfinder/
├── src/
│   ├── pages/          # HTML pages
│   ├── scripts/        # JavaScript files
│   └── styles/         # CSS files
├── app.py             # Backend FastAPI application
├── setup_db.py        # Database setup script
└── README.md          # Documentation
```

## Usage

1. Open the application in your browser
2. Register a new account or login
3. Use the search bar and filters to find shops
4. Click "View on Map" to see shop locations
5. Access advanced features through the navigation menu

## API Endpoints

- POST /register - Register new user
- POST /login - User authentication
- GET /shops/nearby - Find nearby shops with filters

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License.