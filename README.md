# UCAB – Cab Booking Application

UCAB is a **MERN Stack (MongoDB, Express.js, React.js, Node.js)** based cab booking web application that allows users to easily book rides, track drivers in real time, and make secure payments.  
The platform is designed to provide a **simple, fast, and reliable ride booking experience**.

---

#  Features

- User Registration & Login
- Book Cab with Pickup & Drop Location
- View Nearby Available Cabs
- Estimated Fare & Arrival Time
- Real-Time Ride Tracking
- Secure Online Payment
- Ride History
- Discount & Promo Codes
- Donation Option
- Refreshment Ordering During Ride

---

#  Technical Architecture

UCAB follows a **3-Tier Architecture**:

Frontend (Client Layer)
- React.js
- HTML
- CSS
- JavaScript

Backend (Server Layer)
- Node.js
- Express.js
- REST APIs

Database (Data Layer)
- MongoDB

Additional Tools
- JWT Authentication
- Google Maps API
- Socket.io for real-time updates

---

#  MVC Pattern

The backend follows the **Model–View–Controller (MVC)** architecture.

Model
- MongoDB Schemas
- User, Driver, Cab, Ride, Payment

View
- React.js frontend interface

Controller
- Handles application logic
- Ride booking
- Authentication
- Payment processing

---

# Roles and Responsibilities

### User
- Register and login
- Book rides
- Track rides in real time
- Make payments
- View ride history
- Apply discounts or donate

### Driver
- Accept ride requests
- Pick up passengers
- Complete rides
- View ride history and earnings

### Admin
- Manage users and drivers
- Monitor ride bookings
- Manage cab details
- Handle payments and offers

---

# User Flow

1. User logs in or registers
2. User enters pickup and drop location
3. System shows nearby available cabs
4. User selects cab type
5. Driver receives ride request
6. Driver accepts the ride
7. User tracks ride in real time
8. Ride is completed
9. Payment is processed
10. Ride is saved in booking history

---

##  Steps for Execution

Follow the steps below to run the **UCAB Cab Booking Application** locally.

---

###  Setup Frontend (React Application)

Open a terminal and navigate to the **frontend** folder:

```bash
cd frontend
```

Install all required dependencies:

```bash
npm install
```

Start the React development server:

```bash
npm run dev
```

The frontend application will start running at:

```
http://localhost:5173
```

---

###  Setup Backend (Express Server)

Open a new terminal window and navigate to the **backend** folder:

```bash
cd backend
```

Install backend dependencies:

```bash
npm install
```

---

###  Configure Environment Variables

Inside the **backend** folder create a file named:

```
.env
```

Add the following environment variables inside the `.env` file:

```
MONGO_URI=mongodb://localhost:27017/ucab_database
PORT=8000
```

---

###  Start Backend Server

Run the backend server using:

```bash
nodemon server.js
```

or

```bash
npm start
```

The backend server will run at:

```
http://localhost:8000
```

---

### Run the Application

Once both frontend and backend servers are running:

1. Open your browser  
2. Navigate to:

```
http://localhost:5173
```

3. Register or login  
4. Enter pickup and drop location  
5. Book a cab and track your ride
