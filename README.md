📊 Local Business Dashboard

This is a full-stack application that helps simulate how a local business might appear online. It generates a dynamic SEO headline, rating, and review count based on the business name, location, and industry.

Built with React (frontend) and Express.js (backend) — both running in a single project folder.

🧩 Tech Stack

Frontend: React, Tailwind CSS

Backend: Node.js, Express.js

Communication: REST API (fetch), CORS

Run Mode: Localhost

✨ Features

📥 Business form to enter name, location, and industry

🌟 Simulated rating and review count

🧠 Industry-based SEO headline generation

🔁 Regenerate headline feature

🎨 Responsive design using Tailwind CSS

🔄 Loader during API calls

🛠️ Getting Started (Local Setup)

1. Clone the repository

To get a local copy up and running follow these simple steps:

git clone https://github.com/harikarthik1/Local-business-dashboard.git
cd Local-business-dashboard

2. Install dependencies

Install all required packages for both frontend and backend:

npm install

3. Create .env file in root

Add the following line to a new .env file to connect your frontend to the backend:

REACT_APP_API_BASE_URL=http://localhost:5000

4. Run the backend (Express server)

Make sure your backend API is running:

node index.js

✅ You should see:Server running on http://localhost:5000

5. Run the frontend (React)

Start your React development server:

npm start

✅ It will run at:http://localhost:3000

📡 API Endpoints

📬 POST /business-data

Request:

{
  "name": "Cake & Co",
  "location": "Mumbai",
  "industry": "bakery"
}

Response:

{
  "rating": "4.5",
  "reviews": 185,
  "headline": "Why Cake & Co is Mumbai's Sweetest Bakery in 2025"
}

🔁 GET /regenerate-headline

Query Example:

/regenerate-headline?name=Cake%20%26%20Co&location=Mumbai&industry=bakery

Response:

{
  "headline": "Locals Crave Cake & Co – The Best Bakery in Mumbai"
}

📂 Folder Structure

Local-business-dashboard/
├── node_modules/
├── public/                 # Static frontend files
├── src/                    # React components and pages
├── index.js                # Express backend API
├── .env                    # Environment variable for API base URL
├── .gitignore
└── README.md


