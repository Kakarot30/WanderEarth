# WanderEarth - Travel Listings Web App

WanderEarth is a full-stack web application for sharing, discovering, and reviewing travel listings. Users can create accounts, add new listings with images, leave reviews, and manage their own content. The app uses Node.js, Express, MongoDB, EJS, Cloudinary for image storage, and Passport.js for authentication.

---

## Features

- User authentication (register, login, logout)
- Create, edit, and delete travel listings
- Upload listing images (stored on Cloudinary)
- Leave reviews and ratings on listings
- Delete reviews (with proper permissions)
- Flash messages for user feedback
- Responsive UI with Bootstrap

---

## Tech Stack

- **Backend:** Node.js, Express.js, MongoDB, Mongoose
- **Frontend:** EJS, Bootstrap
- **Authentication:** Passport.js (Local Strategy)
- **Image Uploads:** Multer, Cloudinary, multer-storage-cloudinary
- **Validation:** Joi
- **Session Store:** connect-mongo

---

## Prerequisites

- [Node.js](https://nodejs.org/) (v16 or above recommended)
- [MongoDB](https://www.mongodb.com/) (local or Atlas)
- [Cloudinary](https://cloudinary.com/) account (for image uploads)

---

## Environment Variables

Create a `.env` file in the root directory and add the following:

```
ATLASDB_URL=your_mongodb_connection_string
SECRET=your_session_secret
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_KEY=your_cloudinary_api_key
CLOUDINARY_SECRET=your_cloudinary_api_secret
```

---

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/wanderlust.git
   cd wanderlust
   ```

2. **Install dependencies:**

   ```bash
   npm install
   ```

3. **Set up your `.env` file** as described above.

4. **Run the app locally:**

   ```bash
   npm start
   ```

   or

   ```bash
   node app.js
   ```

5. **Visit the app:**
   Open your browser and go to [http://localhost:8080](http://localhost:8080)

---

## Folder Structure

```
Majorproject/
│
├── models/           # Mongoose models (Listing, Review, User)
├── routes/           # Express route files
├── controllers/      # Route controllers
├── views/            # EJS templates
│   └── listings/     # Listing-related views
├── public/           # Static assets (CSS, JS, images)
├── utils/            # Utility functions (error handling, etc.)
├── schema.js         # Joi validation schemas
├── app.js            # Main application file
├── cloudconfig.js    # Cloudinary configuration
└── .env              # Environment variables (not committed)
```

---

## Usage

- Register a new account or log in.
- Create a new listing with an image.
- Browse all listings, view details, and leave reviews.
- Edit or delete your own listings and reviews.

---

## Troubleshooting

- **Image upload errors:** Check your Cloudinary credentials in `.env`.
- **Database errors:** Ensure MongoDB is running and the connection string is correct.
- **Port in use:** Change the port in `app.js` if 8080 is already in use.

---

## License

This project is for educational purposes.

---

## Credits

- [Colt Steele's YelpCamp](https://www.udemy.com/course/the-web-developer-bootcamp/) inspired structure
- [Bootstrap](https://getbootstrap.com/)
- [Cloudinary](https://cloudinary.com/)

---

**Happy Traveling!**
