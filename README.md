# 🎬 React Movie App - TMDB API Integration

![App Screenshot](/src/assets/website-screenshot.png)

This is a React-based web application that fetches and displays the latest movies using [The Movie Database (TMDB)](https://www.themoviedb.org/) API. The app provides users with up-to-date information on newly released films, including movie posters, titles, release dates, and brief overviews.

## 🚀 Features

- 🔄 Retrieves real-time data from the TMDB API  
- 🖼️ Displays movie posters, titles, overviews, and release dates  
- 🔍 Search functionality to find specific movies by title  
- 📈 Trending movies section based on popular user searches  
- 🎯 Built with functional components and React Hooks  
- 📱 Fully responsive design for mobile and desktop  
- ⚡ Clean and minimal UI for smooth user experience  

## 🛠️ Tech Stack

- **Frontend:** React, JavaScript, HTML5, Tailwindcss  
- **API:** TMDB REST API  
- **Tools:** Axios or Fetch API, React Hooks (useEffect, useState, useDebounce)  

## 📦 Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/esmail36/movies-land.git
   cd movies-land


2. **Install dependencies:**
    ```bash
   npm install


3. **Get your TMDB API key:**
    ```bash
   Visit TMDB API and sign up or log in.
   Create a new API key from your dashboard.


4. **Create a .env file in the root directory and add your API key:**
    ```bash
   VITE_TMDB_API_KEY=your_tmdb_api_key_here


5. **Start the development server:**
    ```bash
   npm run dev

## ⚙️ Backend Setup with Appwrite (for Trending Movies)

This project uses **Appwrite** as a backend service to store trending movies based on user search frequency.

### 🔧 Appwrite Setup Instructions

1. **Create a project in Appwrite**
   - Go to [Appwrite Console](https://cloud.appwrite.io/) and create a new project.
   - Copy the **Project ID**.

2. **Create a Database**
   - In your Appwrite project, go to the **Database** section.
   - Create a new database and copy the **Database ID**.

3. **Create a Collection for Trending Movies**
   - Inside your database, create a collection named (e.g., `TrendingMovies`).
   - Add the following attributes (fields):
     - `searchTerm` → `string`, **required**
     - `count` → `integer`, **default: 1**
     - `poster_url` → `URL`, **required**
     - `movie_id` → `integer`, **required**
   - Copy the **Collection ID** after creation.

4. **Update your environment variables**
   - In the root of your project, locate or create the `.env.local` file.
   - Add the following keys and replace values with your own IDs:

     ```env
     VITE_APPWRITE_PROJECT_ID=your_project_id_here
     VITE_APPWRITE_DATABASE_ID=your_database_id_here
     VITE_APPWRITE_COLLECTION_ID=your_collection_id_here
     ```

5. **Install Appwrite SDK if not already installed**
   ```bash
   npm install appwrite

📂 Folder Structure

    movies-land/
    ├── public/
    ├── src/
    │   ├── components/
    │   ├── App.js
    │   ├── index.js
    │   └── ...
    ├── .env
    ├── package.json
    └── README.md

🧪 Future Enhancements

. 📚 Filter by genre, rating, and release year

. ⭐ Add detailed movie pages with trailers and reviews

. 🧑‍💻 User authentication and favorites list

. 🌐 Multi-language support

🙌 Contributing

Contributions are welcome! To contribute:

1. Fork the repository

2. Create your feature branch:
    ```bash
    git checkout -b my-feature
3. Commit your changes:
    ```bash
    git commit -m 'Add some feature'
4. Push to the branch:
    ```bash
    git push origin my-feature
5. Open a Pull Request

📄 License

    This project is licensed under the MIT License.

Made with ❤️ using React and TMDB API

    
---

Let me know if you'd like me to help you write a sample `.env` file, add deployment instructions (like for Vercel or Netlify), or include a live demo badge.
