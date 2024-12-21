# Bus-Ticketing-API

Bus-Ticketing-API is a backend service that provides RESTful APIs for managing bus ticket reservations. It handles operations such as user authentication, bus scheduling, seat selection, and booking management, serving as the core engine for the Bus-Ticketing system.

## Features

- **User Authentication**: Secure user registration and login functionalities.
- **Bus Management**: CRUD operations for bus schedules and routes.
- **Seat Reservation**: Real-time seat availability and booking.
- **Booking Management**: View, update, and cancel bookings.
- **Payment Processing**: Integration with payment gateways for ticket purchases.

## Technologies Used

- **Node.js**: JavaScript runtime for building the server.
- **Express.js**: Web framework for Node.js.
- **MongoDB**: NoSQL database for data storage.
- **Mongoose**: Object Data Modeling (ODM) library for MongoDB and Node.js.
- **JSON Web Tokens (JWT)**: For secure user authentication.

## Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/JayaKarthikkumar/Bus-Ticketing-API.git
   ```

2. **Navigate to the project directory**:

   ```bash
   cd Bus-Ticketing-API
   ```

3. **Install dependencies**:

   ```bash
   npm install
   ```

4. **Set up environment variables**:

   Create a `.env` file in the root directory and add the following variables:

   ```env
   PORT=3000
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret_key
   ```

5. **Start the server**:

   ```bash
   npm start
   ```

   The API server will run at `http://localhost:3000`.

## API Endpoints

- **Authentication**:
  - `POST /api/register`: Register a new user.
  - `POST /api/login`: Authenticate a user and retrieve a token.

- **Buses**:
  - `GET /api/buses`: Retrieve all bus schedules.
  - `POST /api/buses`: Create a new bus schedule.
  - `PUT /api/buses/:id`: Update a bus schedule.
  - `DELETE /api/buses/:id`: Delete a bus schedule.

- **Bookings**:
  - `GET /api/bookings`: Retrieve all bookings for the authenticated user.
  - `POST /api/bookings`: Create a new booking.
  - `PUT /api/bookings/:id`: Update a booking.
  - `DELETE /api/bookings/:id`: Cancel a booking.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your enhancements or bug fixes.

## Acknowledgements

- [Node.js](https://nodejs.org/)
- [Express.js](https://expressjs.com/)
- [MongoDB](https://www.mongodb.com/)
- [Mongoose](https://mongoosejs.com/)
- [JSON Web Tokens](https://jwt.io/)
