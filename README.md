
# 📰 Fetch News Summarizer

### Generate summaries of news articles or blog posts using Google's language model Pegasus via 🤗 HuggingFace's API. 

Pegasus is an encoder-decoder style transformer, specifically trained for abstractive summarization tasks. For this app I used the checkpoint: [google/pegasus-cnn_dailymail](https://huggingface.co/google/pegasus-cnn_dailymail), trained on the CNN-Dailymail corpus.

## About this app

```
streamlit run main.py
```

Step1. Paste the URL of the article and click "Fetch article".

Step2. Enter huggingface API and click "submit", everytime you paste the new article need to click both "Fetch article" and "submit" button.

Also, you will need an API key from **HuggingFace**. In case don't have one already, follow these steps:
- Create a [free account](https://huggingface.co/join) or [login](https://huggingface.co/login)
- Go to **Settings** and then **Access Tokens**
- Create a new Token (select 'read' role)
- Paste your API key in the app's text box



![image](images/example.png)


- - -
**Considerations:**
- The model works best with articles in English
- Articles behind paywall restrictions can't be accessed
- Longer articles require more processing time and resources
- It may not be possible to scrape some websites

