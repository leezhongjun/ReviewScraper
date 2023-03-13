# Review Scraper
Website that scrapes Google for product reviews and runs sentiment analysis on result descriptions

LIVE at [reviewscrper.streamlit.app](https://reviewscrper.streamlit.app/)!

TIP: Be specific e.g. `PS5 console` not `PS5`

## What it uses
 - *Huggingface* for sentiment analysis
    - Uses `LiYuan/amazon-review-sentiment-analysis` for 1-5 star rating
    - Uses `cardiffnlp/twitter-roberta-base-sentiment-latest` for positive/neutral/negative
 - *Apify* for scraping Google
 - *Streamlit* for hosting the website
 - *WordCloud* for word clouds

## Demo
![screencapture-of-website](https://user-images.githubusercontent.com/80515759/224652314-b8b04b45-7e98-407a-b243-5c22447be745.png)

## How to host locally
1. Install requirements
```
pip install -r requirements.txt
```
3. Make an account on [Apify](https://apify.com/)
4. Create the file `/.streamlit/secrets.toml` with the contents:
```
APIFY_TOKEN='YOUR_API_TOKEN'
```
2. Run `main.py`
```
streamlit run main.py
```

## References
 - Inspired by [nus-sentiment](https://github.com/nus-sentiment/nus-sentiment)


