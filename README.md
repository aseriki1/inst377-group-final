# INST377-Group-Website

# Project Title: Student Time Management Application

## Description
The Student Time Management Application is a web-based tool designed to address the unique time management challenges faced by college and high school students. By integrating calendar services with custom features tailored to student needs, the application helps users plan their schedules, reduce stress, and improve their academic performance. The application also benefits parents, advisors, and professors by enabling better communication and tracking of student progress.

## Target Browsers
- **Desktop Browsers**: Google Chrome, Firefox, Safari, and Microsoft Edge
- **Mobile Platforms**: iOS (Safari) and Android (Chrome)


# Developer Manual

## Setting Up the Application

### Prerequisites
1. Install [Node.js](https://nodejs.org/) (LTS version recommended).
2. Install [MongoDB](https://www.mongodb.com/try/download/community) or set up a cloud database using MongoDB Atlas.
3. Install [Git](https://git-scm.com/) for version control.
4. Clone the repository from GitHub.

### Installation Steps
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```
2. Install dependencies:
   ```bash
   npm install
   ```

### Running the Application
1. Start the backend server:
   ```bash
   npm start
   ```
2. Launch the front-end development server:
   ```bash
   cd client
   npm start
   ```
3. Open the application in your browser at `http://localhost:3000`.

### Running Tests
To execute any tests written for the application:
```bash
npm test
```

---

## API Endpoints

### **GET** `/api/events`
- **Description**: Retrieve all events for the logged-in user.
- **Parameters**: None
- **Response**: JSON array of event objects.

### **POST** `/api/events`
- **Description**: Add a new event to the user’s calendar.
- **Parameters**: JSON body with event details (e.g., `title`, `startTime`, `endTime`, `description`).
- **Response**: Confirmation of event creation.

### **PATCH** `/api/events/:id`
- **Description**: Update an existing event.
- **Parameters**: Event ID in the URL, JSON body with updated event details.
- **Response**: Confirmation of event update.

### **DELETE** `/api/events/:id`
- **Description**: Delete an event by ID.
- **Parameters**: Event ID in the URL.
- **Response**: Confirmation of event deletion.

---

## Known Bugs
- Occasional delay in syncing events with Google Calendar API.
- Limited support for recurring events (roadmap feature).

## Roadmap for Future Development
- Add advanced time analytics for users to understand their time management patterns.
- Introduce support for recurring events.
- Develop a mobile app version for better accessibility.
- Integrate additional APIs (e.g., task management tools).


