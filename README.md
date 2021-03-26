# Reddit 'wallstreetbets' Web Scraper

<h3 align="center">About The Project:</h3>
<p align="center">
  <a href="https://github.com/bgregory0913/Machine_Learning-Credit_Risk">
    <img src="stocks-mobile.jpg" alt="stocks-mobile" align="center">
  </a>
</p>

### Project Overview:
_This project is an example of using Reddit’s PRAW API to read posts from the subreddit “wallstreetbets” and return the most popular stocks_

The tool was written with Python in Jupyter Notebook and uses the SMTP library and MIME module to send an email containing the top mentioned stocks.

  * First, a connection is made to Reddit's Python API (PRAW) using the API key reddit provides when you create a developer account.
  * Then we loop through the 'wallstreetbets' subreddit and append the title and content of the first 500 posts to a pandas DataFrame.
  * Next, we loop through each post and merge the post's title and content. After that, another loop to iterate through each word in the post and exclude a list of pre-defined "stop words" (and not the NLP stopwords I'll mention in another post). These would be words we don't care about and just want to toss out.
  * Finally, the words are appended to a dictionary and the process is repeated for every post; additionally, when a repeated word is added to the dictionary, it's "frequency" count is increased by 1.
  * Once this is all complete, the data is put into a DataFrame and sent to an email address securely through a TLS connection.


### Built With:

This project is written with Python on Jupyter Notebook and uses the Reddit PRAW API.

* [Python](https://www.python.org/)
* [JupyterNotebook](https://jupyter.org/)
* [Reddit PRAW](https://praw.readthedocs.io/en/latest/)



## Contact:

Blake Gregory - [LinkedIn](www.linkedin.com/in/blake-greg) - blake.gregory@tilineum.com


