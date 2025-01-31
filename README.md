Chatbot Project

A chatbot built using OpenAI's ChatGPT API, Flask/FastAPI, and React.

Features

Conversational AI chatbot using OpenAI API

Backend with Flask or FastAPI

Frontend with React and Bootstrap

Real-time chat experience

Project Structure

chatbot-project/
│── backend/               # Flask or FastAPI backend
│   ├── app.py            # API logic
│   ├── requirements.txt  # Dependencies
│── frontend/              # React frontend
│   ├── src/
│   │   ├── components/    # React components
│   │   ├── pages/         # Page routing
│   │   ├── App.js         # Main entry
│   │   ├── index.js       # ReactDOM render
│   ├── package.json
│── .env                   # API keys
│── README.md

1. Backend Setup

Installation

cd backend
pip install fastapi uvicorn openai python-dotenv

Run FastAPI Server

uvicorn app:app --reload --port=5000

2. Frontend Setup

Installation

cd frontend
npm install

Run Frontend

npm start

3. API Usage

Endpoints

Method

Endpoint

Description

POST

/chat

Sends user input to OpenAI and gets response

Example Request

curl -X POST http://localhost:5000/chat -H "Content-Type: application/json" -d '{"message": "Hello"}'

4. Deployment

Deploy Backend

Flask: Use Render / Railway.app / Heroku / AWS Lambda

FastAPI: Use Deta, Railway, or Docker

Deploy Frontend

Netlify or Vercel:

npm run build

Upload the build/ folder.

5. Environment Variables

Create a .env file in the backend directory:

OPENAI_API_KEY=your_api_key_here

6. Next Steps

Add authentication (JWT/OAuth)

Save chat history (MongoDB/PostgreSQL)

Improve UI with Material UI / Bootstrap

License

This project is licensed under the MIT License.

Author

Developed by https://github.com/subhashsoni99.