
# Amazon Alexa Reviews Sentiment Analysis
Amazon Alexa Reviews Sentiment Analysis refers to applying sentiment analysis techniques specifically to customer reviews related to Amazon Alexa, the virtual assistant developed by Amazon. With the increasing popularity of voice-enabled devices like Amazon Alexa, customers often share their experiences and opinions through written reviews on platforms such as Amazon's product pages, forums, or social media. Analyzing the sentiment of these reviews provides valuable insights into customers' perceptions, satisfaction levels, and areas of improvement for the Amazon Alexa product. It enables data-driven decision-making based on customer feedback and helps in enhancing the overall user experience of Amazon Alexa.

## Dataset
The dataset was initially retrieved from Kaggle under the title "Amazon Alexa Reviews". A [link](https://www.kaggle.com/datasets/sid321axn/amazon-alexa-reviews) to the dataset is provided, and this dataset can also be found in the repository. The dataset consists of a nearly 3000 Amazon customer reviews (input text), star ratings, date of review, variant and feedback of various amazon Alexa products like Alexa Echo, Echo dots, Alexa Firesticks etc.

### Features: 
The data features are as follows:
1. rating: Product rating.
2. Date: date on which the product was rated.
3. variation: variation of the product.
4. verfified_reviews: the verified reviews for the alexa.
5. feedback: 1 (Positive) or 0 (Negative).

## Steps Performed
1. Read the dataset.
2. Remove handle null values (if any).
3. Preprocess the Amazon Alexa reviews based on the following parameter:
    -  Tokenizing words.
    -  Convert words to lower case.
    -  Removing Punctuations. 
    -  Removing Stop words.
    -  Stemming or lemmatizing the words.
4. Transform the words into vectors using Count Vectorizer.
5. Split data into training and test data.
6. Apply the following models on the training dataset and generate the predicted value for the test dataset:
    -  Multinomial Naïve Bayes Classification.
    -  Logistic Regression.
    -  KNN Classification.
7. Predict the feedback for test data.
8. Compute Confusion matrix and classification report for each of these models.
9. Report the model with the best accuracy.