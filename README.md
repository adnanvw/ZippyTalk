# ZippyTalk: Real-Time Chat Website with MERN Stack, Socket.io, Redux Toolkit, and Tailwind CSS

ZippyTalk is a real-time chat website that allows users to connect with each other and chat in real-time. It was built using the MERN stack (MongoDB, Express.js, React.js, and Node.js), Socket.io, Redux Toolkit, and Tailwind CSS.

- If you liked it, please give this repository a Star⭐

## Technologies Used

- MERN stack (MongoDB, Express.js, React.js, and Node.js)
- Socket.io
- Redux Toolkit
- Tailwind CSS

## Features

- Real-time chat: Users can send and receive messages in real-time.
- User authentication: Users can sign up, log in, and log out using JWT and Google Auth.
- Group creation: Users can create chat rooms and invite others to join.
- Notifications: Users receive notifications on new messages.
- Emojis: Users can send and receive emojis in messages.
- Profile page: Users can update their avatar and display name.
- Users can create a room to chat with others.
- Search functionality.
- Responsive design: The website is optimized for different screen sizes and devices.

## Configuration and Setup

To run this project locally, simply fork and clone the repository or download it as a zip file and unzip it on your machine.

### Setting up the Client

1. Open the project in your preferred code editor.
2. Go to the terminal and open a new terminal window (If you are using VS Code).
3. Split your terminal into two parts (one for the client and the other for the server).

In the first terminal:


$ cd client
$ touch .env


Edit the `.env` file in your client directory and add the following credentials:


REACT_APP_GOOGLE_CLIENT_ID=
REACT_APP_SERVER_URL='http://localhost:8000'


To obtain your Google Client ID for authentication, follow these steps:

- Go to the [Google Cloud Console](https://console.cloud.google.com/apis/credentials).
- Create a new project if you don't have one.
- Click "Create credentials" > "OAuth client ID."
- Select the "Web application" type.
- Name your OAuth client and click "Create."
- Provide your domain and redirect URLs. In development, these will be `http://localhost:3000` and `http://localhost:3000/login`.
- Copy the Client ID and assign it to the `REACT_APP_GOOGLE_CLIENT_ID` variable in your .env file.

Now, start the client:


$ npm install  # Install client-side dependencies
$ npm start    # Start the client


### Setting up the Server

In the second terminal:


$ cd server
$ touch .env


Edit the `.env` file in your server directory and add the following credentials:


PORT=8000
URL= MONGODB URL
SECRET=
CLIENT_ID=
BASE_URL="http://localhost:3000"


Now, start the server:


$ npm install  # Install server-side dependencies
$ npm start    # Start the server

