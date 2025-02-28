
<img src="https://github.com/user-attachments/assets/46b01e2d-0afb-4470-95c8-7eca4436bea4" alt="Image" height="300" width="100%"/>

# Twit Master Project
  This project is a clone of Twitter, built as a full-stack web application. The backend is developed using Spring Boot (Java), and the frontend is implemented with React. The application supports core features like user authentication, posting tweets, liking tweets, and real-time updates. This project was developed as part of an online course where I worked under the guidance of an instructor. The course provided hands-on experience in building a full-stack application from scratch, covering both backend and frontend development.


---
## Key Features

### Frontend
- **Modern UI/UX**: Developed with React, following responsive design principles for optimal user experience.
- **Dynamic Routing**: Utilized React Router for seamless page navigation.
- **State Management**: Managed application state with Redux Toolkit.
- **Real-Time Updates**: Integrated WebSockets to update the UI dynamically without refreshing.
- **API Integration**: Fetches data from the Spring Boot REST API.

### Backend
- **Spring Boot REST API**: Provides secure and efficient endpoints for CRUD operations.
- **User Authentication**: Implements JWT-based authentication for secure login and session management.
- **Database Management**: Uses MySQL for data storage, with JPA/Hibernate for ORM.
- **Scalability**: Backend architecture designed for easy scalability.

---

## Application Modules

### Frontend (React)
- **Login/Signup**: User authentication with form validation.
- **Dashboard**: Displays a timeline of tweets.
- **Tweet Interaction**: Users can post, like, and delete tweets.
- **Profile Management**: Edit user profile details and view past tweets.

### Backend (Spring Boot)
- **Controllers**: Handles HTTP requests and responses.
  - `AuthController`: Manages user authentication and registration.
  - `TwitController`: Handles tweet-related operations.
  - `UserController`: Manages user profiles.
  - `LikeController`: Processes tweet likes.
- **Services**: Implements the business logic of the application.
- **Repositories**: Provides data access via JPA.
- **DTOs & Mappers**: Transfers data between layers, ensuring clean code and separation of concerns.

---

## Technologies Used

### Frontend
- React
- Redux Toolkit
- React Router
- Axios
- Tailwind CSS
- WebSockets

### Backend
- Java (Spring Boot)
- MySQL
- JPA/Hibernate
- JWT for Authentication
- Maven

---

## Installation Guide

### Prerequisites
Ensure you have the following installed:
- **Node.js** (v14 or higher)
- **Java** (v11 or higher)
- **MySQL**
- **Maven**

### Steps to Set Up Locally

#### Backend Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/twitter-clone-backend.git
   cd twitter-clone-backend

2. Update the `application.properties` File

-  Open the `application.properties` file located in the `src/main/resources/` directory of each backend module.
- Update the following configurations with your MySQL and JWT details

3. Build and run the application

#### Frontend Setup 
1. Navigate to the frontend folder:
   ```bash
   cd twitter-clone-frontend

2. Install dependencies:
   ```bash
   npm install

3. Start the development server:
   ```bash
   npm start

---

## API Endpoints

### User Management
| HTTP Method | Endpoint                  | Description                                  |
|-------------|---------------------------|----------------------------------------------|
| GET         | `/api/users/profile`      | Fetch the profile details of the logged-in user |
| GET         | `/api/users/{userId}`     | Fetch details of a user by their ID         |
| GET         | `/api/users/search`       | Search users by query string                |
| PUT         | `/api/users/update`       | Update the logged-in user's profile         |
| PUT         | `/api/users/{userId}/follow` | Follow or unfollow a user                   |

### Tweet Management
| HTTP Method | Endpoint                    | Description                                  |
|-------------|-----------------------------|----------------------------------------------|
| POST        | `/api/twits/create`         | Create a new tweet                          |
| POST        | `/api/twits/reply`          | Reply to an existing tweet                  |
| PUT         | `/api/twits/{twitId}/retwit`| Retweet an existing tweet                   |
| GET         | `/api/twits/{twitId}`       | Fetch a tweet by its ID                     |
| DELETE      | `/api/twits/{twitId}`       | Delete a tweet                              |
| GET         | `/api/twits/`               | Fetch all tweets                            |
| GET         | `/api/twits/user/{userId}`  | Fetch all tweets by a user                  |
| GET         | `/api/twits/user/{userId}/likes` | Fetch tweets liked by a specific user      |

### Like Management
| HTTP Method | Endpoint                       | Description                                  |
|-------------|--------------------------------|----------------------------------------------|
| POST        | `/api/twits/{twitId}/like`     | Like a specific tweet                       |
| DELETE      | `/api/twits/{twitId}/unlike`   | Unlike a specific tweet                     |
| GET         | `/api/twits/twit/{twitId}`     | Get all likes for a specific tweet          |

---
# Contact
For any queries, please contact [sjawale@usc.edu].


