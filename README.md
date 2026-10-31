# 🎬 Cinemate AI – LLM-Powered Movie Recommendation System

**Cinemate AI** is an intelligent movie recommendation system that helps users discover movies based on their interests and natural-language preferences. It combines Large Language Models (LLMs), Natural Language Processing (NLP), and content-based filtering to deliver personalized movie recommendations through an interactive web interface.

The system uses **Google FLAN-T5** to understand user queries, **TF-IDF and Cosine Similarity** to identify relevant movies, and the **TMDB API** to retrieve movie posters and additional information.

## ✨ Features

- **AI-Powered Recommendations:** Understands movie preferences written in natural language.
- **LLM Integration:** Uses Google FLAN-T5 for interpreting user requests.
- **Content-Based Filtering:** Recommends movies using TF-IDF vectorization and cosine similarity.
- **Movie Search:** Search for movies by title.
- **Real Movie Posters:** Fetches movie posters from The Movie Database (TMDB).
- **Movie Information:** Displays descriptions, ratings, genres, release years, and director information when available.
- **Interactive Interface:** Provides a modern, dark-themed interface built with Gradio.
- **Personalized Discovery:** Helps users explore movies based on genres, themes, and interests.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| Google Colab | Development environment |
| Hugging Face Transformers | LLM integration |
| Google FLAN-T5 | Natural-language understanding |
| Scikit-learn | TF-IDF and cosine similarity |
| Pandas | Dataset processing |
| MovieLens Dataset | Movie and rating data |
| TMDB API | Movie posters and metadata |
| Gradio | Interactive web interface |

## 🧠 How It Works

1. **User Input:** The user enters a movie title or a natural-language request.
2. **Preference Understanding:** FLAN-T5 processes the request and extracts relevant preferences.
3. **Feature Extraction:** TF-IDF converts movie descriptions and genres into numerical vectors.
4. **Similarity Calculation:** Cosine similarity identifies movies that match the user's preferences.
5. **Movie Retrieval:** The system retrieves relevant movie information and posters using TMDB.
6. **Recommendation Display:** Gradio presents the recommended movies in an interactive interface.

## 📸 Application Preview

Add screenshots of your application to a folder named `screenshots` and display them here.

```markdown
![Cinemate AI Home Page](screenshots/home.png)
![Movie Recommendations](screenshots/recommendations.png)
```

## 📂 Project Structure

```text
Cinemate-AI/
│
├── screenshots/
│   ├── home.png
│   └── recommendations.png
│
├── Cinemate_AI.ipynb
├── requirements.txt
├── README.md
└── .gitignore
```

*Update the filenames above to match your actual repository files.*

## 🚀 Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/Cinemate-AI.git
cd Cinemate-AI
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Configure TMDB API

Create an account at [The Movie Database (TMDB)](https://www.themoviedb.org/) and obtain an API Read Access Token.

If you are using Google Colab, add your token under **Secrets** with the name:

```text
TMDB_ACCESS_TOKEN
```

Access it securely in Python:

```python
from google.colab import userdata

TMDB_ACCESS_TOKEN = userdata.get("TMDB_ACCESS_TOKEN")
```

Never upload your API token or other private credentials to GitHub.

### 4. Run the Project

Open `Cinemate_AI.ipynb` in Google Colab, execute the notebook cells in order, and launch the Gradio application.

## 💬 Example User Queries

Try entering natural-language requests such as:

- Recommend science-fiction movies about space and aliens.
- Suggest action movies with fighting and adventure.
- Recommend romantic movies with emotional stories.
- Find horror movies about ghosts.
- Suggest movies about artificial intelligence and robots.
- Recommend movies similar to Interstellar.
- Find family-friendly animated movies.
- Suggest mystery and thriller movies.

## 📊 Dataset

This project uses the **MovieLens ml-latest-small dataset**, which contains movie information and user ratings.

Dataset: [MovieLens – GroupLens Research](https://grouplens.org/datasets/movielens/)

Movie posters and additional movie metadata are retrieved through the TMDB API.

## 🔮 Future Improvements

- User accounts and personalized watchlists.
- Favorite movie functionality.
- Advanced hybrid recommendation algorithms.
- Improved recommendation accuracy using user feedback.
- Movie trailer integration.
- Deployment as a public web application.
- Multilingual natural-language movie search.

## 👨‍💻 Development

Developed as an AI-powered movie recommendation project at **Xvision**.

## 🙏 Acknowledgements

- [Hugging Face](https://huggingface.co/) – FLAN-T5 model and Transformers library.
- [MovieLens](https://grouplens.org/datasets/movielens/) – Movie recommendation dataset.
- [The Movie Database (TMDB)](https://www.themoviedb.org/) – Movie posters and metadata.
- [Gradio](https://www.gradio.app/) – Interactive web application framework.
- [Scikit-learn](https://scikit-learn.org/) – Machine learning tools.

## 📜 TMDB Attribution

This product uses the TMDB API but is not endorsed or certified by TMDB.

## 📄 License

This project is intended for educational and non-commercial purposes. Add a suitable open-source license if you intend to distribute the project under specific reuse terms.

---

⭐ **If you find Cinemate AI interesting, consider giving this repository a star!**
