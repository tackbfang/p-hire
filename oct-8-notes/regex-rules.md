# Regex Rules

- develop rules by Friday morning
- ultimately need to label others, like location, time, and address

e.g. 
- "on my way" 99%
- "payment" etc.

https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285

# Goal
- aim for high precision
	- understand precision and recall
- okay with trading off recall / coverage

1. come up with rules
	- contains "" key words
	- e.g. "review" "reviews" = hire
2. test them on the data set, "hire" vs "not hire"
	- how good are the rules 

# Rules
- try the most basic one
- include see you, 


have a score for pros only
- "hire" + "hired" + "hiring" + see you" "see u" + "review" + "reviews"

"see you" -> indicates that meeting has happened, there is a confirmation of meeting, but not necessarily

- length of the conversation

the higher the score, the better.

- actually look at whether "on my way" is present


# On my way

Not perfect because sometimes it won't work


# False Positive Cases
- they looked at the place for a quote but didn't actually get hired
	- gave a quote afterwards
- but they did meet
- it's not that they weren't hired... it's just that we don't have more information


- also think that sentiment analysis can be a signal.

# Regex Phrases that have high precision
- understand regex more

# 100% Precision
- let's do it (100%)
- review
- r'^(?=.*hired)(?=.*payment)'
- hired + payment
- hired + cash
- confirmed +
- see you on + review
- on my way + review
- on our way + review
- on the way + review
- on my way + cash
- on my way + check
- on the way + cash
- on our way + cash / check
- be there + pay (89%), count = 8
- be there + a review / quick review 100% (4)
- be there + review (88%) (7)
- be there + review  + not reviewed = 100%

- some combinations are promising... just need to get more for now

# read up on different regex expressions and then coming up with ideas...
- testing out exactly what I want...

# Questions
- having trouble using regex... there are lots of tutorials online but doesn't teach me what I need... a lot are character based as opposed to word based...
- 


# Alternative Ideas:
- use NLTK to tokenize words, 
	- word and text tokenizer
	- n-grams
	- parts of speech tagger
	- named entity recognition
- sentiment analysis
- build a model with word scoring
- 


