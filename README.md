# NLP_semantic_analysis

# Advanced Recommendation System with Semantic Analysis and Sentiment Analysis  

This project addresses the challenge of delivering personalized recommendations by integrating semantic analysis and comment-based sentiment analysis. It enables users to discover content relevant to their preferences and feedback sentiments while adapting in real time.

---

## Features  

1. **Semantic Search**  
   - Combines **BM25** keyword matching and **SBERT embeddings** for semantic similarity ranking.  
   - Prioritized search results based on likes and views.  

2. **Sentiment Analysis**  
   - Utilizes **HuggingFace’s sentiment analysis pipeline** to analyze video comments.  
   - Calculates the percentage of positive sentiments for ranking recommendations.  

3. **Video Management**  
   - Stores video metadata (title, description, likes, views, comments, and thumbnails) in MongoDB.  
   - Semantic search queries and matches are stored for faster retrieval.  

4. **User Interaction**  
   - Users can like videos and add comments (up to 200 characters).  
   - Real-time updates to MongoDB for likes and comments.  

5. **Administrative Automation**  
   - Batch processes pre-populated food-related search queries.  
   - Updates sentiment scores automatically.  

---

## Installation  

### Prerequisites  
- Python 3.8+  
- MongoDB (installed and running locally or remotely)  
- Required Python libraries: Install using `requirements.txt`.  

### Steps to Set Up  

1. Clone the repository:  
   ```bash  
   git clone https://github.com/your-repo/advanced-recommendation-system.git  
   cd advanced-recommendation-system  
   ```  

2. Install dependencies:  
   ```bash  
   pip install -r requirements.txt  
   ```  

3. Configure MongoDB:  
   - Update the MongoDB URI in `config.py`.  

4. Run the application:  
   ```bash  
   python app.py  
   ```  

5. Access the application at `http://127.0.0.1:5000`.  

---

## Application Flow  

1. **Homepage**:  
   - Users can search for videos using keywords.  
   - Displays search results based on semantic analysis or fallback title matches.  

2. **Video Details**:  
   - Shows video metadata, likes, comments, and positive sentiment percentages.  
   - Allows users to like videos and add comments.  

3. **Admin Automation**:  
   - Automatically processes batch queries and updates sentiment scores.  

---

## Output Examples  

### Example 1: Homepage Search  
Search for a video with the keyword "Authentic dosa recipe." Results are ranked by semantic relevance and likes/views.  

![Search Results]()  

---

### Example 2: Video Details  
A detailed view of a video, including likes, comments, and positive sentiment percentage.  

![Video Details]()  

---

### Example 3: Sentiment Analysis Results  
Sentiment analysis of comments, showing percentages of positive feedback.  

![Sentiment Analysis]()  

---

## License  

This project is licensed under the **MIT License**. See the `LICENSE` file for details.  

---

## Contributors  

- **Jagdeesh P** - [Your GitHub Profile](https://github.com/Jagdeesh-P)  


---

## Acknowledgments  

- **Hugging Face Transformers** for sentiment analysis.  
- **SentenceTransformers** for semantic similarity ranking.  
- **MongoDB** for efficient data storage.  
- Flask community for robust API development.  

