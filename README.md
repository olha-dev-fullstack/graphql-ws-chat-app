# GraphQL Job Board
This is a simple GraphQL chat app build with websockets which allows authenticated users to chat in real time.

## 🚀 Features

- **User Authentication**: Sign-in functionality.
- **Messages**: Create and send messages in chatroom 

## 🛠️ Tech Stack

### Backend

- **JavaScript**
- **Apollo Server**
- **GraphQL**
- **Knex**
- **SQLite**
- **WebSocket**

### Frontend

- **React.js**

## 📜 GraphQL Schema

```javascript
type Query {
  messages: [Message!]
}

type Mutation {
  addMessage(text: String!): Message
}

type Subscription {
  messageAdded: Message
}

type Message {
  id: ID!
  user: String!
  text: String!
}

```

## 📦 Project Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/olha-dev-fullstack/graphql-job-board
   ```
2. **Install dependencies:**
   ```bash
   cd client
   npm install

   cd server
   npm install
   ```

5. **Start the server:**
   ```bash
   cd client
   npm start

   cd server
   npm start
   ```

## 🎯 Usage Instructions

- Access the frontend to sign in and manage vacancies at http://localhost:3000
- GraphQl Playground to test API: http://localhost:9000/graphql
