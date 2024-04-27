# I320D-NLP-Final-Project
Pipeline to produce a model which recommends hotels to users based on user input


The code follows a pipeline to recommend hotels to a user based on user input. The reviews are imported from the dataset that we are using, found on Kaggle here: https://www.kaggle.com/datasets/juhibhojani/hotel-reviews. The reviews are preprocessed and cleaned. Then, sentiment analysis is performed using VADER, and aggregated so each hotel has a score, with positive scores indicating positive sentiment and the number indicating strength. The positive reviews are put into a new dataset that we give recommendations from. Then, sentiment analysis is performed on the review column to generate sentiment embeddings for each review, and for the user query. All review vectors are compared to the review vectors based on cosine distance, and the 5 most similar (lowest distance) hotel matches are given to the user in order of similarity. Finally, we evaluate our models for accuracy. 
