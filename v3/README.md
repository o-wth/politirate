# Algorithm
For each platform, each numbered item is its own subscore. In the future, we may plan on analyzing sources together, so if a politician posts the same message on two platforms, we pool calculations. 

Notes on all platforms:
- beliefs: we may create another score to describe a politician's beliefs/place them on the political spectrum
    - topic modeling
- time: we should weight recent posts more than old posts

## Twitter

1. **meaning/sentiment**: politicians should be able to convey their ideas without sacrificig clarity
    - use BERT (see [🤗 Transformers](https://github.com/huggingface/transformers))
    - difficulties: sarcasm and/or satire if they are mocking another politician

2. **analytics**: retweets without comments, retweets with comments, replies, and the number of likes should all be factored into this score. Retweets with comments and replies should be analyzed for connotation. 
    - difficulties: threaded tweets

3. **pictures**: determine if a picture corresponds to its text
    - difficulties: on twitter people sometimes post screenshots of text to bypass the char limit
    - THIS IS A SERIOUS ETHICAL DISCUSSION; WE MAY NOT INCLUDE IMAGE ANALYSIS
