# Estatia 🏡

**Estatia** is a full-stack real estate web application where users can browse, list, and save properties, chat with landlords, and explore listings via interactive maps.


## 🚀 Features

- 🔐 User authentication (JWT-based login / logout)
- 🏠 Property listing with filtering (type, price, city, etc.)
- 📌 Map integration using Leaflet & React-Leaflet
- 💬 Real-time messaging with Socket.io
- 🗂️ Save / unsave posts
- 🧾 User profile and post management
- 🌐 Responsive UI built with React + SCSS


## 🛠️ Tech Stack

| Layer       | Tech                                                   |
|-------------|--------------------------------------------------------|
| Frontend    | React, React Router, SCSS, Axios, Leaflet              |
| Backend     | Node.js, Express, Prisma ORM, JWT, Cookie Parser       |
| Database    | MongoDB (via Prisma)                                   |
| Real-time   | Socket.io                                              |
| Deployment  | On progress   |


## 📁 Project Structure

```

full-stack-estate/
│
├── client/          # Frontend (React + Vite)
├── api/             # Backend (Express + Prisma)
├── socket/          # Socket.io server
└── README.md

````


## 🧪 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/estatia.git
cd full-stack-estate
````

### 2. Set up environment variables

Create `.env` files in `api/` and optionally `client/`:

**api/.env**

```env
DATABASE_URL=your_mongodb_connection_url
JWT_SECRET_KEY=your_jwt_secret
CLIENT_URL=http://localhost:5173
```


### 3. Install dependencies

#### Backend

```bash
cd api
npm install
```

#### Frontend

```bash
cd ../client
npm install
```

#### Socket Server

```bash
cd ../socket
npm install
```


### 4. Run the development servers

In separate terminals:

#### Start Backend

```bash
cd api
npx nodemon app.js
```

#### Start Frontend

```bash
cd client
npm run dev
```

#### Start Socket Server

```bash
cd socket
node app.js
```


## ✅ API Endpoints Overview

| Method | Endpoint             | Description                |
| ------ | -------------------- | -------------------------- |
| POST   | `/api/auth/register` | Register new user          |
| POST   | `/api/auth/login`    | Login and set token cookie |
| POST   | `/api/auth/logout`   | Clear auth cookie          |
| GET    | `/api/posts`         | Fetch filtered listings    |
| GET    | `/api/posts/:id`     | Get single post detail     |
| POST   | `/api/posts`         | Create new listing         |
| DELETE | `/api/posts/:id`     | Delete a listing           |


## 📷 Screenshots 

| Welcome Page | Listing Page | Profile Page |
|--------------|---------------------|------------------|
| <img width="1469" alt="image" src="https://github.com/user-attachments/assets/83f031b9-505d-4fe4-8a7b-d52a20b57357" /> | <img width="1469" alt="image" src="https://github.com/user-attachments/assets/9f4abb87-32e2-44fc-a41f-af5e37b784b7" />
 | <img width="1469" alt="image" src="https://github.com/user-attachments/assets/e8d3f1ad-fc90-4b65-87ba-7276684792a0" /> |



## 📄 License

This project is licensed under the MIT License.
Feel free to fork and customize for learning or portfolio purposes.

## 🙌 Acknowledgements

This project is built upon the **Full Stack MERN Real Estate App** tutorial created by [Lama Dev](https://www.youtube.com/@LamaDev).
Sincere thanks to Lama Dev for the open-source educational content and inspiration.

Additional customization, improvements, and deployment are made independently for portfolio and learning purposes.
