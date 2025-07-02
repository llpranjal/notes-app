# Notes App

A full-stack notes application built with React, Express, and PostgreSQL.

## ✨ Features

- Create, read, update, and delete notes
- Clean and responsive UI
- RESTful API backend
- PostgreSQL database with Prisma ORM

## 🚀 Tech Stack

**Frontend:**
- React 18
- TypeScript
- Vite
- CSS3

**Backend:**
- Node.js & Express
- TypeScript
- Prisma ORM
- PostgreSQL

## 🛠️ Installation

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd notes-app
   ```

2. **Install dependencies**
   ```bash
   # Install frontend dependencies
   cd notes-app
   npm install
   
   # Install backend dependencies
   cd ../notes-app-server
   npm install
   ```

3. **Set up the database**
   ```bash
   # Create a .env file in notes-app-server directory
   echo "DATABASE_URL=postgresql://username:password@localhost:5432/notes_db" > .env
   
   # Run database migrations
   npx prisma migrate dev
   npx prisma generate
   ```

## 🏃‍♂️ Running the Application

1. **Start the backend server**
   ```bash
   cd notes-app-server
   npm start
   ```
   Server will run on `http://localhost:5000`

2. **Start the frontend (in a new terminal)**
   ```bash
   cd notes-app
   npm run dev
   ```
   Frontend will run on `http://localhost:5173`

## 📡 API Endpoints

- `GET /api/notes` - Get all notes
- `POST /api/notes` - Create a new note
- `PUT /api/notes/:id` - Update a note
- `DELETE /api/notes/:id` - Delete a note

## 📁 Project Structure

```
notes-app/
├── notes-app/          # React frontend
│   ├── src/
│   └── package.json
├── notes-app-server/   # Express backend
│   ├── src/
│   ├── prisma/
│   └── package.json
└── README.md
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).