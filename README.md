# Weather Tweet Hashtag Prediction

This project aims to develop a Machine Learning model that analyzes tweets about the weather and predicts relevant hashtags. The model categorizes each word in the tweets into three groups: "Sentiments," "When," and "Kind."

## Categories

1. **Sentiments**: Describes the emotions related to the weather (e.g., happy, sad, neutral).
2. **When**: Indicates the timing of the weather event (e.g., past, present, future).
3. **Kind**: Describes the type of weather (e.g., stormy, thunder, lightning).

### Example
For the tweet "Yesterday’s stormy weather was extremely frightening":
- **Sentiments**: "extremely frightening"
- **When**: "Yesterday"
- **Kind**: "stormy"

## Model Architecture

The project uses a Many-to-Many Encoder-Decoder Sequence Model with LSTM networks:

## Data Source

The dataset for this project is sourced from the [Kaggle](https://www.kaggle.com/competitions/crowdflower-weather-twitter/data).

## Project Structure

- **train.csv**: Training data containing tweets, locations, and confidence scores for 24 labels across the three categories.
- **test.csv**: Testing data with tweets and locations.
- **Twitter Hashtag prediction over weather report tweets.ipynb**: Jupyter notebook to create and train the model, predicting hashtags from input tweets.
- **contractions.pkl**: Dictionary of contractions and their expansions.

## Usage

1. Train the model using the Jupyter notebook.
2. Use the trained model to predict hashtags from new tweets.
