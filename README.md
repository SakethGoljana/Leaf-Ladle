# Leaf & Ladle Restaurant Website 🍃🥄

Welcome to the **Leaf & Ladle Restaurant Website**, a vibrant web platform that serves up the flavors of our vegetarian paradise right at your fingertips! Craving a zesty Indian curry, a savory Chinese stir-fry, or hearty American comfort food? Leaf & Ladle makes it a breeze to browse menus, order meals, track deliveries, and reserve tables at our two cozy branches: **Dreamwood** and **Heavengarden**. Crafted with beginners in mind, this project is a tasty mix of modern web tech, intuitive design, and a sprinkle of veggie-inspired charm! 🌱

---

## 🌟 Project Overview

Leaf & Ladle isn’t just a website—it’s a digital dining experience! Customers can:
- **Sign in as a guest** or use **Google Sign-In** to jump into the action with ease.
- **Explore cuisines** like Indian, Chinese, and American, adding dishes to a cart.
- **Checkout seamlessly** for pickup or delivery at either branch.
- **Track orders in real-time**, from “Cooking” to “On Its Way!”
- **Reserve tables** with dynamic availability, securing a spot for your next meal.

This project is a beginner-friendly guide to building a full-stack web app, packed with clear code, detailed workflows, and a dash of culinary creativity. Whether you’re a coder, a foodie, or both, Leaf & Ladle invites you to fork, clone, and savor the experience!

---

## 🥗 Tech Stack

Our recipe for success blends the freshest web technologies:
- **Frontend**:
  - **HTML**: The structure of our digital dining room.
  - **CSS**: Stylish, responsive designs that look as good as our dishes taste.
  - **JavaScript**: The magic behind pop-up menus and instant cart updates.
- **Backend**:
  - **Node.js + Express**: The kitchen crew handling orders and reservations.
- **Database**:
  - **MongoDB Atlas**: A cloud-based pantry storing menus, orders, and bookings.
- **Authentication**:
  - **Google OAuth 2.0**: Secure, one-click sign-in with Google accounts.
- **APIs**: The waiters shuttling requests between frontend and backend.
- **Deployment**: Ready to serve on platforms like Heroku or AWS.

---

## 🍴 Features That Sizzle

Leaf & Ladle is loaded with features to make your dining experience smooth and delightful:
- **Guest Sign-In & Google Sign-In**: Dive in as a guest with a quick name or email (optional), or sign in securely with your Google account in one click.
- **Cuisine Pages**: Browse beautifully organized menus by cuisine, complete with mouthwatering images and prices.
- **Cart Management**: Add, tweak, or remove dishes with real-time cost updates.
- **Checkout**: Pick pickup or delivery, choose a branch, and place your order in a snap.
- **Order Tracking**: Follow your meal’s journey from kitchen to doorstep with live status updates.
- **Table Reservations**: Book a table at SproutHaven or VerdantVale, with real-time availability checks.

---

## 🚀 Getting Started

Ready to cook up this project on your local machine? Follow these steps to get Leaf & Ladle simmering:

### Prerequisites
- **Node.js** (LTS version) from [nodejs.org](https://nodejs.org).
- A **MongoDB Atlas** account (free tier works!) for cloud storage.
- A **Google Cloud Console** account to set up OAuth 2.0 credentials.
- A web browser (Chrome, Firefox, or Safari) and a stable internet connection.
- A pinch of enthusiasm for coding and vegetarian cuisine! 😄

### Installation
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/<your-username>/leaf-and-ladle.git
   cd leaf-and-ladle
   ```

2. **Install Dependencies**:
   ```bash
   npm install express mongoose google-auth-library
   ```

3. **Set Up MongoDB Atlas**:
   - Sign up at [mongodb.com/cloud/atlas](https://www.mongodb.com/cloud/atlas).
   - Create a cluster and get your connection string (e.g., `mongodb+srv://<user>:<pass>@cluster0.mongodb.net/leafandladle`).
   - Update `server.js` with the connection string.

4. **Set Up Google OAuth**:
   - Go to [console.developers.google.com](https://console.developers.google.com).
   - Create a project, enable the Google+ API, and generate OAuth 2.0 credentials (Client ID and Secret).
   - Add your Client ID to the frontend (`auth.js`) and Secret to the backend (`server.js`).
   - Set authorized redirect URIs (e.g., `http://localhost:3000/auth/google/callback`).

5. **Run the Backend**:
   ```bash
   node server.js
   ```
   The server will fire up on `http://localhost:3000`.

6. **Serve the Frontend**:
   - Open `index.html` in a browser or use a local server:
     ```bash
     npx http-server
     ```
   - Visit `http://localhost:8080` to see the homepage.

7. **Test the Magic**:
   - Click “Sign In” to try guest login or the Google Sign-In button.
   - Browse cuisines, add items to your cart, and reserve a table!

---

## 🛠️ Project Structure

Here’s a peek at the ingredients in our codebase:
- **`index.html`**: The homepage, your entry to the Leaf & Ladle experience.
- **`auth.js`**: Powers guest sign-in, Google Sign-In, and session management.
- **`add-to-cart.js`**: Handles cart additions and updates.
- **`checkout.js`**: Turns carts into orders with a flourish.
- **`server.js`**: The backend maestro, serving APIs like `/api/menu`, `/api/reservations`, and `/auth/google`.
- **`styles.css`**: Responsive styles that make the site shine on any device.

---

## 🌿 Contributing

We’d love for you to add your own spices to Leaf & Ladle! To contribute:
1. Fork the repository.
2. Create a branch for your feature (`git checkout -b feature/amazing-new-idea`).
3. Commit your changes (`git commit -m "Added a pinch of awesome"`).
4. Push to your branch (`git push origin feature/amazing-new-idea`).
5. Open a Pull Request and share your flavor!

Check out the [SRS](SRS_LeafAndLadle_Restaurant_Website_Beginner_Guide.markdown) for detailed requirements and workflows to guide your contributions.

---

## 🍵 Beginner’s Guide

New to coding? Leaf & Ladle is your perfect sous-chef! Our [SRS document](SRS_LeafAndLadle_Restaurant_Website_Beginner_Guide.markdown) is a beginner-friendly treasure trove, offering:
- **Step-by-step workflows** for every feature (e.g., how Google Sign-In works).
- **Code snippets** with clear comments to demystify the tech.
- **FAQs** to troubleshoot common hiccups (e.g., “Why doesn’t my Google button work?”).
- **Tips** for setting up and extending the project.

### Getting Started with Google Sign-In
- **What’s Google Sign-In?** It lets users log in with their Google account, saving time and adding security. Think of it as a VIP pass to Leaf & Ladle!
- **How to Test It**: Click the “Sign in with Google” button on the homepage. You’ll be redirected to Google’s login page, then back to the site with a “Welcome, [Your Name]!” message.
- **Troubleshooting**: If the button doesn’t work, check your Client ID in `auth.js` and ensure the redirect URI matches in Google Cloud Console. Use browser DevTools (F12) to spot errors.
- **Try Extending It**: Add a profile picture display using the Google user’s avatar from the OAuth response.

Start small—try tweaking the Google Sign-In button’s style or adding a new cuisine—and watch your coding skills bloom!

---

## 📜 License

This project is licensed under the MIT License. Feel free to use, modify, and share, just like a family recipe passed down with love.

---

## 🙌 Acknowledgments

- **Google Cloud**: For secure and seamless OAuth authentication.
- **Vegetarian Foodies**: For inspiring a platform that celebrates plant-based deliciousness.
- **Open-Source Community**: For tools like Node.js, Express, and MongoDB that make projects like this possible.

---

## 📬 Contact

Got questions or ideas? Reach out on GitHub or drop by our virtual kitchen at **Dreamood** or **Heavengarden**. Let’s cook up something extraordinary together!

Happy coding, and bon appétit! 🍲
