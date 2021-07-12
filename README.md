<<<<<<< HEAD
# MicrosoftEngage-TeamsClone

Realtime, Multi-Peer Video calling and chat app with websockets and WebRTC using Node.js, Express and Socket.io with Vanilla JS on the frontend with a flexible and intuitive GUI.
The app uses WebRTC for peer to peer connection which facilitates Video sharing between the peers. The sockets help in connecting multiple peers and transferring messages between them. 

## Features
1. Predefined Room-wise conferences.
2. Current Room User lists.
3. Video Conferencing using WebRTC and Websockets for Multi-Peer network.
4. Messaging feature in the App.
5. Video and audio toggle.

## Dependencies
1. Nodejs
2. Express Js
3. React Js
4. Firebase
5. WebRTC API
6. Socket IO

## Future Scope
1. Screen Sharing.
<<<<<<< HEAD
2.User Authentication
=======
2. User Authentication
3. Games
>>>>>>> 9195de62c0e71fcc0439bca3c846d21f0139929f

## Usage
```
<CMD in the main folder>
> npm install
> npm start

Go to localhost:3000
```

## How does it work
The user will enter the Room name and the User name. Every user is given a unique user ID(UUID). A new WebRTC peer is defined.
Then, the script will check if the user is the first one to enter the room, If so, it will create a new connection request to other peers. And wait for other peers to connect. It creates a description and sends it to the server using socket.io. The server then broadcasts the message to all the peers in the room.
If, the user was not the first one to join the room, then the script will listen to all the messages broadcasted by the server. If there is a description , the WebRTC peer will create an answer and send it to the server to broadcast. If the answer is received by other peers then they send ICEs. And exchanges their video and audio streams.
Once the connection between is established they can exchange chat messages too using socket.io.



