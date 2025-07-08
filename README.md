
# Cosine Similarity - Single File Version

from sklearn.feature_extraction.text import TfidfVectorizer
from sklearn.metrics.pairwise import cosine_similarity

def calculate_cosine_similarity(text1, text2):
    # Create the TF-IDF vectorizer
    vectorizer = TfidfVectorizer()

    # Transform the texts into TF-IDF vectors
    tfidf_matrix = vectorizer.fit_transform([text1, text2])

    # Compute the cosine similarity
    similarity = cosine_similarity(tfidf_matrix[0:1], tfidf_matrix[1:2])

    return similarity[0][0]

if __name__ == "__main__":
    print("=== Cosine Similarity Calculator ===")
    
    # Example input texts
    text1 = input("Enter first text: ")
    text2 = input("Enter second text: ")

    # Calculate similarity
    result = calculate_cosine_similarity(text1, text2)
    
    # Display result
    print(f"\nCosine Similarity: {result:.4f}")
