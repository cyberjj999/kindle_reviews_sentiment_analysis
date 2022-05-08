## This project is created as part of the [#CrystalizeMyLearning](https://www.linkedin.com/pulse/introducing-crystalizemylearning-movement-lye-jia-jun/) movement I founded where I seek to learn through writing

The sentiment analysis algorithm is as follows

1. Read the file source and extract individual reviews
2. For each review, we will tokenize the paragraph into word tokens using nltk.word_tokenize()
3. For each word in the reviews, we will identify the part of speech for each one of them using ntlk.pos_tag()
4. After obtaining the list of words along with their parts of speech, we will extract all adjectives into an adjective word list.
5. Following that, we will iterate through each adjective in the adjective word list and identify if that adjective is positive or negative based on our positive.txt and negative.txt files which contain a list of positive and negative words respectively.
    - If the adjective is positive, we will add 1 to the sentiment score of the review.
    - If the adjective is negative, we will subtract 1 from the sentiment score of the review.
6. If the final score is positive, we can safely assume that the review is positive. Also, the higher the score, the more positive it is.
