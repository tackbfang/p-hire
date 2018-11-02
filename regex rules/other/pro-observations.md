# Today
Categories:
* location ('Location')
* contact information ('Contact Information')
* scheduling - meeting or job ('Scheduling - Meeting or Job')
* price ('Price')
* payment ('Payment')

For each category, 
0. get a dataframe with all the columns (DONE)
1. run NLTK (DONE)
2. read through the messages to get a sense of ideas ()
3. come up with precision rules ()

# Checking hire again
- then do scheduling, price, payment


# Things to do
- get a dataframe with columns message, bid id, and then is_location, etc. get all the labels (20 min)
- run NLTK on all of them
- come up with precision rules...

### Obervations of Pro Hires
- key words from messages that resulted in hire
- 1114 cases

- not going through every single one, just scan
- find location APIs that can do that...
- maybe nltk or some data science ones... like beautiful soup or some crawling

- find most common words, and find most common bi-grams, tri-grams, etc.
http://www.nltk.org/book/ch06.html
-> do that for all the categories today
-> look into some examples of hire
## 1.3

- Location, address, [LOCATION] + not hired, exact address, send address, need the address, get the address,
- get addresses from NLTk or topics
- meet with you, meet me, let's meet, lets meet, like to meet
- miles, be there
- located in / at / near
- \n for addresses
- arrival time
- our apartment
- I live in 
- quote
- where is [] at?
- my home

-> extracting information from text
-> analyzing sentence structure
-> classify text

# Text Data
- document retrieval
- document classification
- sentiment analysis
- topic detection
	- spinn3r
- clustering, represent text as feature vectors
- turning text into a feature vector
	- bag of words (try it in NLTK)
	- raw text -> bag of words
- there are just too many corner cases...
- maybe there are other datasets in existence already

https://docs.google.com/presentation/d/13tKhGKcik-pwb24GfgSQo3D9MkjYprS-TtgfQhIwujE/edit#slide=id.g2a0284f6fd_0_246
