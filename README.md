🛍️ E-Commerce Full Stack Project

This is a Full Stack E-Commerce Application built using Node.js, Express, MongoDB, and React.
It includes three parts:

Backend Server
Frontend Website
Admin Panel

Backend Setup
1️.Open Backend in Terminal

Open the project folder in VS Code.

Right-click on the backend folder → Open in Integrated Terminal.

Run:

npm install


2️.Setup Environment File (.env)

Create a file named .env inside your backend folder and paste the following content:

JWT_SECRET = "greatstack"
ADMIN_EMAIL = "admin@example.com"
ADMIN_PASSWORD = "greatstack123"

MONGODB_URI = "-------- Paste Your Mongo URI Here --------"

CLOUDINARY_API_KEY = "-------- Paste Cloudinary API key --------"
CLOUDINARY_SECRET_KEY = "-------- Paste Cloudinary SECRET key --------"
CLOUDINARY_NAME = "-------- Paste Cloudinary cloud name --------"

STRIPE_SECRET_KEY = "-------- Paste Stripe Secret key --------"

RAZORPAY_KEY_SECRET = '-------- Paste Razorpay Secret key --------'
RAZORPAY_KEY_ID = '-------- Paste Razorpay key Id --------'


⚠️ Important Notes:
Do not use @ in your MongoDB password.
Do not add / at the end of your MongoDB URI.
Keep this file private (add .env to .gitignore).

3️.Setup Cloudinary for File Storage

Create an account at Cloudinary
Go to your Dashboard.
Copy: Cloud Name, API Key, and API Secret.
Paste these values in your .env file under the Cloudinary section.

4️.Setup MongoDB Atlas
Sign up at MongoDB Atlas
Create a New Project.
Go to Database → Build a Database.
Choose Free (M0) tier → select your Region.
Create Username & Password (avoid using @ in password).
Whitelist your IP: 0.0.0.0/0.
Click Connect → Compass → Copy your Connection String.
Paste it into the .env file replacing <username> and <password>.

5️.Setup Stripe
Create an account at Stripe
From your Dashboard, copy your Secret Key.
Paste it into .env as:
STRIPE_SECRET_KEY=your_stripe_secret
6️⃣ (Optional) Setup Razorpay

Create an account at Razorpay
.

From the Dashboard, copy your Razorpay Key ID and Secret Key.

Paste them into .env:

RAZORPAY_KEY_ID=your_key_id
RAZORPAY_KEY_SECRET=your_secret_key

7️.Run the Backend
npm run server

Keep this terminal running before starting the frontend or admin panel.

Frontend Setup

Right-click on the frontend folder → Open in Integrated Terminal.

Run:
npm install
npm run dev


Once the terminal displays a URL (usually http://localhost:5173), open it in your browser.

Admin Panel Setup

Right-click on the admin folder → Open in Integrated Terminal.

Run:
npm install
npm run dev

Once the terminal displays a URL (usually http://localhost:5174), open it in your browser.

Project Run Order

1️.Start the Backend first.
2️.Then run the Frontend.
3️.Finally, run the Admin Panel.
