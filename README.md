# Netflix Clone

A full-stack web application that mimics the core functionalities of Netflix, allowing users to browse movies and TV shows, create watchlists, and stream content.

## Features

- User authentication (login, signup)
- Browse and search for movies and TV shows
- View detailed information about each title
- Create and manage a personal watchlist
- Streaming functionality for selected content
- Responsive design for mobile and desktop devices

## Tech Stack

- **Frontend**: React.js, CSS, Bootstrap or Material-UI
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication**: JWT (JSON Web Tokens)
- **Movie API**: The Movie Database (TMDb) API or similar

## Project Structure

```
netflix-clone/
│
├── client/                # Frontend React app
│   ├── public/            # Public assets
│   ├── src/
│   │   ├── components/    # React components
│   │   ├── App.js         # Main App component
│   │   ├── index.js       # Entry point for React
│   │   └── styles/        # Stylesheets
│   └── package.json       # Frontend dependencies
│
├── server/                # Backend API
│   ├── models/            # Database models
│   ├── routes/            # API routes
│   ├── server.js          # Express server setup
│   └── package.json       # Backend dependencies
│
├── .env                   # Environment variables
├── README.md              # Project documentation
└── package.json           # Project dependencies
```

## Getting Started

### Prerequisites

Ensure you have the following installed on your system:

- Node.js
- npm or yarn
- MongoDB (for local development)
- An account with The Movie Database (TMDb) for API access

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/BorisagarRushabh/Netflix_Clone.git
   cd Netflix_Clone
   ```

2. Install dependencies for both frontend and backend:

   ```bash
   # Install backend dependencies
   cd server
   npm install

   # Install frontend dependencies
   cd ../client
   npm install
   ```

3. Set up environment variables:

   Create a `.env` file in the `server/` directory with the following information:

   ```
   MONGO_URI=your_mongodb_uri
   JWT_SECRET=your_jwt_secret
   TMDB_API_KEY=your_tmdb_api_key
   ```

4. Start the development servers:

   - Backend (Express.js) server:

     ```bash
     cd server
     npm start
     ```

   - Frontend (React.js) server:

     ```bash
     cd client
     npm start
     ```

5. Open the application in your browser:

   - Frontend: [http://localhost:3000](http://localhost:3000)
   - Backend API: [http://localhost:5000](http://localhost:5000)

## API Endpoints

- **GET** `/api/movies`: Fetch a list of movies.
- **GET** `/api/movies/:id`: Get details of a specific movie.
- **POST** `/api/watchlist`: Add a movie to the user's watchlist.
- **DELETE** `/api/watchlist/:id`: Remove a movie from the user's watchlist.

## Future Improvements

- Implement a recommendation system based on user preferences.
- Add user reviews and ratings for movies.
- Create a mobile app version of the clone.
- Enhance the streaming functionality for better user experience.

## Contributing

Contributions are welcome! Feel free to fork the repository, open issues, or submit pull requests to improve the project.
