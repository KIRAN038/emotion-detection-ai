
# emotion.py
from textblob import TextBlob

def detect_emotion(text):
    analysis = TextBlob(text)
    if analysis.sentiment.polarity > 0.3:
        return "😊 Happy"
    # ... (rest of the code)
