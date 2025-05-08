# 🧠 AI Image Generator 🎨

An AI-powered image generator app that allows users to generate images using natural language prompts, powered by OpenAI's DALL·E API. Built with a full-stack JavaScript architecture using React for the frontend and Express.js for the backend.

---

## 📌 Table of Contents

- [🧰 Tech Stack](#-tech-stack)
- [📸 Demo](#-demo)
- [📂 Project Structure](#-project-structure)
- [⚙️ Development Setup](#️-development-setup)
- [🚀 Deployment](#-deployment)
  - [Frontend (Netlify)](#frontend-netlify)
  - [Backend (Render)](#backend-render)
- [📄 License](#-license)

---

## 🧰 Tech Stack

- **Frontend**: React, Axios, CSS
- **Backend**: Node.js, Express, OpenAI API
- **API**: OpenAI DALL·E API
- **Deployment**: Netlify (Frontend), Render (Backend)

---

## 📸 Demo

> 🌐 [Live Demo (Netlify)](https://your-netlify-url.netlify.app)  
> ⚙️ [Backend (Render)](https://your-backend-url.onrender.com)

---

## 📂 Project Structure
ai-image-generator/
│
├── client/ # React frontend
│ ├── public/
│ ├── src/
│ ├── .env
│ └── package.json
│
├── server/ # Express backend
│ ├── index.js
│ ├── .env
│ └── package.json
│
├── README.md



---

## ⚙️ Development Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/ai-image-generator.git
cd ai-image-generator
```


2. Setup Backend (Express)
bash
Copy
Edit
cd server
npm install
Create a .env file:

ini
Copy
Edit
OPENAI_API_KEY=your_openai_api_key_here
Start the server:

bash
Copy
Edit
node index.js
The backend runs on http://localhost:8080.

3. Setup Frontend (React)
bash
Copy
Edit
cd client
npm install
Create a .env file in the client/ folder:

ini
Copy
Edit
REACT_APP_API_URL=http://localhost:8080
Start the React app:

bash
Copy
Edit
npm start
App runs on http://localhost:3000.

🚀 Deployment
✅ Frontend (Netlify)
Build the React app:

bash
Copy
Edit
npm run build
Push your code to GitHub and connect the repo to Netlify.

In the Netlify dashboard:

Set the build command: npm run build

Set the publish directory: client/build

Add environment variable:

ini
Copy
Edit
REACT_APP_API_URL=https://your-backend-url.onrender.com
Deploy!

✅ Backend (Render)
Go to https://render.com and log in.

Click “New +” → “Web Service”.

Connect your GitHub repo and select the server directory.

Fill in the service settings:

Build Command: npm install

Start Command: node index.js

Environment Variables:

ini
Copy
Edit
OPENAI_API_KEY=your_openai_api_key_here
Click Create Web Service.

Once deployed, copy the backend URL and update your frontend .env:

ini
Copy
Edit
REACT_APP_API_URL=https://your-backend-url.onrender.com
