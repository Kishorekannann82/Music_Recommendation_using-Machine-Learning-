#🎵 Music Recommender System 🎧
This project is a Music Recommender System built using Streamlit, Spotify API, and machine learning techniques. It recommends songs similar to the selected song, along with their album cover images.

🚀 Features:
Recommend top 5 similar songs based on the selected song.

Displays album cover images using Spotify API.

Easy-to-use Streamlit web interface.

Uses pre-trained similarity model for fast recommendations.

📂 Project Structure:
│
├── app.py                     # Main Streamlit app script  
├── df.pkl                     # Pickled dataset containing song and artist info  
├── similarity.pkl             # Pickled similarity matrix (precomputed)  
├── requirements.txt           # Required Python libraries  
└── README.md                  # Project documentation  
🔧 Technologies Used:
Python

Streamlit

Spotipy (Spotify API wrapper)

Pandas

Pickle (for model persistence)

⚙️ How It Works:
Loads the dataset of songs and pre-computed similarity matrix.

Accepts song input from the user via dropdown.

Computes the most similar songs using the similarity matrix.

Fetches album covers from Spotify API using spotipy.

Displays recommended songs with images.

🎯 How to Run Locally:
Clone the repository
git clone <your-repo-url>
cd <your-repo-folder>
Install dependencies
pip install -r requirements.txt
Run the Streamlit app
streamlit run app.py
✅ Spotify API Setup:
Create an app on the Spotify Developer Dashboard.

Copy the CLIENT_ID and CLIENT_SECRET.

Replace them in your app.py:

CLIENT_ID = "your_client_id"
CLIENT_SECRET = "your_client_secret"
📦 Requirements:
streamlit  
spotipy  
pandas  
numpy  
scikit-learn  
📌 Note:
The models (df.pkl and similarity.pkl) are required to run the app.

Make sure your Spotify API credentials are valid.

💡 Future Improvements:
Add search functionality by artist or genre.

Improve recommendation algorithm using deep learning models.
