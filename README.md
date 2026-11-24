# 🎉 Event Finder – Discover, Create & Manage Events

<p align="center">
  <b>A Full-Stack Event Management Web Application</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&amp;logo=nodedotjs&amp;logoColor=white">
  <img src="https://img.shields.io/badge/Express.js-000000?style=for-the-badge&amp;logo=express&amp;logoColor=white">
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&amp;logo=mongodb&amp;logoColor=white">
  <img src="https://img.shields.io/badge/EJS-B4CA65?style=for-the-badge&amp;logo=ejs&amp;logoColor=black">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&amp;logo=javascript&amp;logoColor=black">
</p>


## 📌 Overview

**Event Finder** is a full-stack web application designed to help users discover, create, and manage events through a simple and user-friendly interface.

The application allows users to explore available events, view event details, and manage their own events. It provides complete CRUD (Create, Read, Update, Delete) functionality with MongoDB as the database.

The platform also includes user authentication, password hashing, session management, and dynamically rendered pages using EJS.

## ✨ Key Features

### 🔍 Event Management
- Browse and explore available events.
- View detailed event information.
- Create and publish new events.
- Update existing event details.
- Delete events when they are no longer required.
- Store event information in MongoDB.

### 🔐 User Authentication
- User registration and login functionality.
- Secure password hashing using bcrypt.
- Password verification during login.
- Session-based user authentication.
- Logout functionality.
- Protected event creation route.

### 📱 User Interface
- Dynamic content rendering using EJS.
- Responsive web interface.
- Organized event information.
- Easy navigation between pages.

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| HTML5 | Webpage structure |
| CSS3 | Styling and layout |
| JavaScript | Client-side functionality |
| Node.js | Backend runtime environment |
| Express.js | Server and routing |
| MongoDB | Database |
| Mongoose | Database modeling |
| EJS | Dynamic webpage rendering |
| bcrypt | Password hashing |
| Express Session | User session management |
| JWT | Token generation |
| Cookie Parser | Cookie handling |
| dotenv | Environment variable management |

## 🏗️ System Architecture

The application follows a client-server architecture.

```text
             USER
               |
               v
       Frontend (EJS, CSS)
               |
               v
       Express.js Server
               |
       +-------+-------+
       |               |
       v               v
 Authentication    Event Routes
       |               |
       v               v
   bcrypt         CRUD Operations
       |               |
       +-------+-------+
               |
               v
          Mongoose
               |
               v
           MongoDB
```

## 📂 Project Structure

```text
Eventfinder-Web-Application/
│
├── models/
│   ├── eventmodel.js
│   └── usermodel.js
│
├── public/
│   ├── css/
│   ├── js/
│   └── images/
│
├── views/
│   ├── index.ejs
│   ├── read.ejs
│   ├── add.ejs
│   ├── edit.ejs
│   ├── login.ejs
│   ├── signup.ejs
│   ├── about.ejs
│   └── contact.ejs
│
├── .env
├── .gitignore
├── index.js
├── package.json
├── package-lock.json
└── README.md
```

## ⚙️ Installation & Setup

Follow these steps to run the project locally.

### 1. Clone the Repository

```bash
git clone https://github.com/Pawanthakr/Eventfinder-Web-Application.git
```

### 2. Navigate to Project Directory

```bash
cd Eventfinder-Web-Application
```

### 3. Install Dependencies

```bash
npm install
```

### 4. Configure Environment Variables

Create a `.env` file in the root directory.

```env
MONGODB_URI=your_mongodb_connection_string
PORT=3000
```

Replace the MongoDB connection string with your own MongoDB connection URI.

### 5. Start the Application

```bash
npm start
```

### 6. Open in Browser

```text
http://localhost:3000
```

Your Event Finder application should now be running locally.

## 🗄️ Database Structure

The application uses MongoDB with Mongoose for database operations.

### User Collection

Stores registered user information.

| Field | Description |
|---|---|
| fullname | User's full name |
| email | User's email address |
| password | Hashed password |

### Event Collection

Stores event-related information.

| Field | Description |
|---|---|
| eventtitle | Name of the event |
| location | Event location |
| image | Event image URL |
| date | Event date |
| time | Event timing |
| category | Event category |
| contact | Contact information |
| description | Event description |
| creator | Name of the event creator |

## 🔗 Application Routes

| Method | Route | Description |
|---|---|---|
| GET | `/` | Home page |
| GET | `/read` | Display all events |
| GET | `/add` | Open event creation page |
| POST | `/create` | Create a new event |
| GET | `/edit/:eventid` | Open event editing page |
| POST | `/update/:eventid` | Update event details |
| GET | `/delete/:id` | Delete an event |
| GET | `/signup` | Registration page |
| POST | `/signup` | Register a new user |
| GET | `/login` | Login page |
| POST | `/login` | Authenticate user |
| GET | `/logout` | Logout user |
| GET | `/about` | About page |
| GET | `/contact` | Contact page |

## 🔄 CRUD Operations

The application implements all four fundamental database operations.

| Operation | Functionality |
|---|---|
| Create | Add new events |
| Read | Display available events |
| Update | Modify existing event details |
| Delete | Remove events from the database |

These operations are implemented using Express.js routes and Mongoose database methods.

## 🔐 Security Implementation

The application includes basic security-related functionality:

- Password hashing using bcrypt.
- Password verification using bcrypt.compare().
- Session-based authentication.
- Protected event creation route.
- Environment variables for database configuration.

**Note:** For production deployment, session secrets and JWT secrets should be stored in environment variables, and event modification/deletion routes should enforce ownership and authorization checks.

## 🚀 Live Demo

**Live Website:** https://eventfinder-web-application.onrender.com

**GitHub Repository:** https://github.com/Pawanthakr/Eventfinder-Web-Application

## 🔮 Future Enhancements

The following improvements can make the application more powerful:

- Advanced event search and filtering.
- Location-based event discovery.
- Event registration and online booking.
- Email notifications and reminders.
- Event categories and sorting.
- Admin dashboard for event management.
- User profile management.
- Event ratings and reviews.
- Improved authorization and security.

## 📚 Learning Outcomes

Through this project, I gained practical experience in:

- Full-stack web application development.
- Backend development using Node.js and Express.js.
- MongoDB database integration.
- Implementing CRUD operations.
- User authentication and password hashing.
- Session management.
- Dynamic rendering using EJS.
- Organizing a real-world web application.
- Deploying a Node.js application.

## 👨‍💻 Author

**Pawan Thakre**

GitHub: [@Pawanthakr](https://github.com/Pawanthakr)

---

<p align="center">
  ⭐ If you find this project useful, consider giving it a star!
</p>

<p align="center">
  Built with ❤️ using Node.js, Express.js and MongoDB.
</p>
