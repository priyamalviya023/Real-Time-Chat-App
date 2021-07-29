# Real-Time-Chat-App

Intro:
- The project Real Time Chat Application uses Web Technology to transfer messages securely in Real Time.
- The front-end of the Application is created using React.js and the back-end is created using Node.js and Express.js.
- The Database used to store the chats is MongoDB . MongoDB Atlas is used to store Database on cloud
- The messages are sent in Real Time using SOCKET.IO.
- The main features of the Application are Register Page, the Login Page , the Home Page and  the Chat Rooms Page


#How does JWT works:
To implement JWT I used npm module “jsonwebtoken”.
When a user registers or log in, a token containing encrypted user_id is sent from backend as a response which is then stored in local storage of browser or as a cookie. Thereafter whenever a request is sent a token is added to the request which is then checked for validation on the server side. The request will proceed further only if the token is verified else an error will be sent back.

#Database schemas:
It has 3 Schemas:
Message: It stores the data of text messages like message timing, sender id, room id etc.
Room: It stores the room id and room name
User: It stores the user info like name, email, password hash and salt, etc.

#How did you sent the data to frontend:
Data is sent in Json format which is then handled using react.js at frontend.
