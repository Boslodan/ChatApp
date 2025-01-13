# ChatApp

**ChatApp** is a real-time communication application developed using **Laravel** for the backend and **ReactJS** for the frontend. 
The application was built between February 2024 and August 2024 as a project for the Internet Technologies course at 
the Faculty of Organizational Sciences, University of Belgrade.

## 🛠️ Technologies
- **Backend:** Laravel
- **Frontend:** ReactJS
- **CSS:** For styling the user interface
- **Axios:** For communication between the frontend and backend

## 🚀 Features
- **Authentication:** User registration, login, and logout.
- **Real-time communication:** Sending text messages and sharing links.
- **User roles:**
  - **Administrator:** View all users and delete accounts.
  - **Moderator:** Access to all chats and messages.
  - **User:** Create and participate in conversations.
- **Chat export:** Export chat history to a PDF file.
- **Admin Dashboard:** Overview of all registered users.
- **Contact page:** Users can submit inquiries with their name, email, and message.

## ⚙️ Installation and Setup

To run the **ChatApp**, follow these steps:

**Backend setup**
1. Clone the repository:
   ```bash
   git clone https://github.com/elab-development/internet-tehnologije-projekat-chatapp_2020_0348.git
2. Navigate to the backend directory:
   cd chatapp
   
4. Install the required dependencies:
   composer install

5. Copy the .env example file to .env and configure the database connection:
   cp .env.example .env

6. Generate the appliaction key:
   php artisan key:generate

7. Run the database migrations and seed the data:
   php artisan migrate --seed

8. Start the backend development server:
   php artisan serve
   
**Frontend Setup**
1. Navigate to the frontend directory:
   cd chat-app
   
3. Install the required dependencies:
   npm install
   
5. Start the frontend development server:
   npm start

The application will be available at:
Backend: http://localhost:8000
Frontend: http://localhost:3000

**User Experience**
Home Page: Access login and sign-up forms.
Chat Page: Create and manage conversations.
Admin Dashboard: Available only to administrators to review users.

**Data Models**
Message: Stores messages and links them to users and chats.
Chat: Represents conversations between users.
UserChat: Links users to their conversations.
User: Stores user information.
Role: Manages user permissions.
