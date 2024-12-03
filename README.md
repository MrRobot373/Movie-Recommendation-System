# Netflix-recommender-system-deployment

## 🎬 Content-Based Movie Recommendation System 🎥

This project is a **Content-Based Movie Recommendation System** that recommends movies based on a given movie's details (e.g., genre, cast, and other related information). The system uses **Cosine Similarity** to suggest similar movies based on the movie attributes. It also provides detailed information about the movie and its cast, including profiles, biographies, and ratings. The user interface mimics Netflix's design to provide a seamless and engaging experience for users.

---

### Features:
- **Movie Recommendations**: The system suggests similar movies based on the movie's genre, cast, and plot.
- **Movie Details**: Provides detailed information about the selected movie, including its genre, rating, release date, runtime, and status.
- **Cast Information**: Displays detailed profiles of the actors in the movie, including their biography, birthday, and place of birth. You can click on any cast member to view more details.
- **Rating & Reviews**: The system also displays the movie's rating based on user votes. It includes a list of recommended movies, based on the input movie.
- **User-Friendly Interface**: The design follows Netflix's UI principles, with easy navigation and a responsive layout.

---

### Key Technologies Used:
- **Python** (Flask Web Framework)
- **Scikit-learn** for **Cosine Similarity** and machine learning
- **HTML/CSS** for building the responsive and interactive UI
- **Bootstrap** for responsive design
- **IMDb API** for fetching movie data (optional for external reviews)
- **BeautifulSoup** for web scraping IMDb reviews (for older versions)

---

### Project Structure:
1. **main.py**: The Flask app that handles routes, data processing, and recommendation logic.
2. **templates/**: Contains the HTML files for rendering the main page and the recommendation page. 
   - `home.html`: Main landing page for entering movie names.
   - `recommend.html`: Displays movie recommendations and detailed information.
3. **static/**: Stores static assets such as CSS files, images, and JavaScript files used for frontend functionality.
4. **main_data.csv**: The dataset containing movie information, including genres, cast names, and movie descriptions, which is used to create movie recommendations.

---

### How It Works:
1. **Input**: The user enters the name of a movie into the search bar.
2. **Recommendation**: Based on the movie name, the system calculates **Cosine Similarity** to recommend movies with similar content, including similar genres and actors.
3. **Details**: Once a movie is selected, the system displays detailed information, including movie ratings, cast details, and a list of recommended movies.
4. **Responsive UI**: The UI is designed to be fully responsive, making it usable on desktops, tablets, and mobile devices.

---

### Key Screens:
- **Home Page**: The user enters the movie name in a stylish, centered search bar.
- **Movie Details Page**: Shows detailed movie info like its genre, rating, cast, and a section for recommended movies.
- **Cast Details Modal**: Click on any cast member to get their full biography, birthday, and place of birth.

---

### How to Run:
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/content-based-movie-recommender.git
   cd content-based-movie-recommender
   ```
   
2. **Install Dependencies**:
   Make sure you have Python 3.x and Flask installed.
   ```bash
   pip install -r requirements.txt
   ```
   
3. **Run the Application**:
   ```bash
   python main.py
   ```
   Visit `http://127.0.0.1:5000/` in your browser to interact with the application.


### Future Improvements:

- Add more movies and interactive elements like movie trailers, director details, etc.
- Add collabrative and hybrid model for recommendation of movies
