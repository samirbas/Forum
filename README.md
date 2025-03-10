On this project you will have to focus on a few points:
•	Registration and Login
•	Creation of posts
o	Commenting posts
•	Private Messages
As you already did the first forum you can use part of the code, but not all of it. Your new forum will have five different parts:
•	SQLite, in which you will store data, just like in the previous forum
•	Golang, in which you will handle data and Websockets (Backend)
•	Javascript, in which you will handle all the Frontend events and clients Websockets
•	HTML, in which you will organize the elements of the page
•	CSS, in which you will stylize the elements of the page
You will have only one HTML file, so every change of page you want to do, should be handled in the Javascript. This can be called having a single page application.
Registration and Login
To be able to use the new and upgraded forum users will have to register and login, otherwise they will only see the registration or login page. This is premium stuff. The registration and login process should take in consideration the following features:
•	Users must be able to fill a register form to register into the forum. They will have to provide at least:
o	Nickname
o	Age
o	Gender
o	First Name
o	Last Name
o	E-mail
o	Password
•	The user must be able to connect using either the nickname or the e-mail combined with the password.
•	The user must be able to log out from any page on the forum.
Posts and Comments
This part is pretty similar to the first forum. Users must be able to:
•	Create posts
o	Posts will have categories as in the first forum
•	Create comments on the posts
•	See posts in a feed display
o	See comments only if they click on a post
Private Messages
Users will be able to send private messages to each other, so you will need to create a chat, where it will exist :
•	A section to show who is online/offline and able to talk to:
o	This section must be organized by the last message sent (just like discord). If the user is new and does not present messages you must organize it in alphabetic order.
o	The user must be able to send private messages to the users who are online.
o	This section must be visible at all times.
•	A section that when clicked on the user that you want to send a message, reloads the past messages. Chats between users must:
o	Be visible, for this you will have to be able to see the previous messages that you had with the user
o	Reload the last 10 messages and when scrolled up to see more messages you must provide the user with 10 more, without spamming the scroll event. Do not forget what you learned!! (Throttle, Debounce)
•	Messages must have a specific format:
o	A date that shows when the message was sent
o	The user name, that identifies the user that sent the message
As it is expected, the messages should work in real time, in other words, if a user sends a message, the other user should receive the notification of the new message without refreshing the page. Again this is possible through the usage of WebSockets in backend and frontend.

