
# Chat_App:- Chat On
## Description of the Project
This chat application Chat On helps one effortlessly  communicate with people anywhere in the world by sending and receiving messages in real time.This project provides the instant communication functionality between users. The users have the capability to do one to one communication and also they can communicate with in groupwhich is the most fascinating feature of this app. As a cherry on the top, the  User Authentication feature of this project boosts up its reliability of the users on Chat On.


## Deployment

To deploy this project after cloning,  run

```bash
  node backend/server.js
```

Otherwise just click

  [Chat On](https://chat-app-doogle.vercel.app/)



## Technologies Used

Express version 4.18.2  
React version 18.2.0  
Mongoose version 6.7.2  
Nodemon version 2.0.20  
Socket.io version 4.5.4
## API Reference

#### Register User

```http
  POST /api/user/
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `User details` | `json` | Takes the User data to the Database |

#### To login

```http
  GET /api/user/login
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `User Details`      | `json` | fetch the User Details from the Database |

#### Searching the Doogle Registered Users  

```http
  GET /api/user?search=
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `User Id`      | `json` | Checks for the Id in the Database of Chat On |

#### Fetching Chats of a User

```http
  GET /api/chat
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `User chat`      | `json` | It fetches the whole chat of a User  |

#### Accessing Chats of a User

```http
  GET /api/chat
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `User chat`      | `json` | It helps to get access to the chat of the User  |

#### To create a group

```http
  POST /api/chat
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `Users and Group name `      | `json` | It helps to create the group in the app  |

#### To rename the name of the group

```http
  PUT /api/chat
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `Chat Id and Chat name `      | `json` | To rename the group name  |

#### To send a message 

```http
  POST /api/message 
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `content of the message `      | `json` | Sending of the messages  |

#### To receive the messsage 

```http
  GET /api/message:chatId
```

 | Type     | Description                       |
 | :------- | :-------------------------------- |
 | `json` | fetching all messages of the selected chat  |


## Features

- Real time messeges
- Sign up and Sign in for users
- Fullscreen mode
- Push Notifications
- Responsive layout
- Group Chat feature to form community


## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`MONGO_URI`

`JWT_SECRET`

`NODE_ENV`


## Tech Stack

**Client:** React, Chakra UI, Socket.io-client

**Server:** Node, Express, Socket.io


## Screenshots

The Login page-
![user_Login](https://github.com/Shashwat-pati/Chat-app/assets/99614901/1ba5c440-f462-47db-851b-901c6758d08d)

The Sign up page-
![user_signup](https://github.com/Shashwat-pati/Chat-app/assets/99614901/59cf171a-257a-45a2-93c9-6f9564ae96fe)

One-to-One Users Chat Interface-
![users_chat](https://github.com/Shashwat-pati/Chat-app/assets/99614901/6b562950-9128-41f9-92fc-fdd28ac9d422)

Group Chat Description-
![group_chat_desc](https://github.com/Shashwat-pati/Chat-app/assets/99614901/f421bda0-e4a6-4645-8605-06b46f8cca4c)

Group Chat Interface-
![group_chats](https://github.com/Shashwat-pati/Chat-app/assets/99614901/2325c94a-1052-4224-9e3c-7a76c6ccf297)

## Acknowledgements

 - [React JS](https://reactjs.org/docs/getting-started.html)
 - [Node JS](https://nodejs.org/dist/latest-v19.x/docs/api/)
 - [Express JS](https://expressjs.com/en/guide/routing.html)
 - [Mongoose ](https://mongoosejs.com/docs/guide.html)
 - [Chakra UI ](https://chakra-ui.com/getting-started)

