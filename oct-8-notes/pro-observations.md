### Customer Insights
- takes probably 60 minutes. I finished about 1/12 of it in 5 minutes.
- took about 4h

I'd say 90% of the cases have one of these. It's also possible to not be hired and still have these.

#### Payments
- check +5, cheques, cash +3, credit card +2, debit +1
- invoice +4
- [down] payment +3
- deposit +3
- charges / charging +2 
- a dollar amount (e.g. $250) +1
- pay +1
- receipt +1
- agreement +1
- warranty

#### Gratitute
- good work +1 
- [thank you for] feedback
- working with you

#### Meeting
- see you [at]... / see u \[date / time\] +27
- be there [date / around] [shortly] +19, is there, almost there here / get there(compared to here from Customers) / here 
- on my way / on the way / on our way +10
- meeting / meet [you] +3 
- arrive [by] +3
- let me in
- in route
- [at your] house / home +1 
- late / few minutes behind
- eta

#### Review

- [leave us a/ thank you for] review  +111
	- lots of automated reviews / maybe not actually hires
	- the automated ones include a link, usually
	- eliminate the automated reviews
- [thanks for leaving a] rating +1

- sometimes pro ask the customers to review with the exact same message

#### Confirmation of Hiring
- [mark us as ] hire / hired / hiring +24 (not unhire)
- confirm /confirmed / confirming +8
- contract +7
- book (booking request) +4
- appointment +4
- choosing [company name / me/us] +4
- done / getting done / completed +2
- all set +2
- let's do it +1 / can do it
- request / reserve +1
- good to go
- can do it / let's do it

#### Job Progress
- finishing / finished +2
- treatment

#### Scheduling
- [full / physical] address +9
- [your phone] number +6
- schedule / reschedule / scheduled +4
- [date / time] [is great] +3
- looking forward +1
- contact me
- reaching out
- cell / text / message me
- available 
- getting started
- speaking with you / talk to you soon 
- sounds good / works for me / this works / works great
- call if [you have any questions]


#### Recurring
- refer

#### Misc
- sent you a new version of your resume
- details 


# Random / Context-based
- k

# Overall Observations
- giving an address is pretty good
- a lot of people are confused about how to mark as hire
	- why don't we just have a strong UI for hired as opposed to guessing?
- some I don't think are hires
- the overall hire rate is smaller, because not all pros will accept.
- a lot more use of the word  from the pro... it's really important for them


# Tech
- use NLP techniques
- wordcloud
- fastText / neural text classification. fastText is pretty easy, I think my friend applied it in a weekend. It's not a huge task. It's not neural network based. I'd like to try using it.
- can use NLTK or other libraries to find some bi-grams or tri-grams related to the key words
- suggest alternative for 


maybe it wouldn't be a bad proxy to instead ask for a review
- 2x rate that Thumbtack pros ask for review

- 

# Thoughts
I've looked at about 200 on the pro side
- I would say about 80% have on of the key words
- I would also say that not hires would not have something like that... except maybe "hire" it can be 
- I think a classifier like fastText or a neural text classifier that's trained on conversation data would be very good

# My Suggestions
- instead of spending 3 weeks on a label and finding definitions
- I can create a decent heuristic rule and we can use it as a baseline
- we can build a classifier with fastText that is NOT neural network based

In total, I can create heuristics / NLP rules and then create a fastText classifier in like 2 weeks
- neural networks / fastText finds these patterns for us
- I don't think we can get 4 times the result by reading more heuristics
- can use it as a testing set
- V1 would be done Oct 26 instead of Nov 30
- I think we should automate as many of the conversation flow as possible, like in Lemonade
- If we have an easier way of hiring then we don't have to do predictions

# Questions
- what are existing baselines? 
- what specific metrics are we looking at?
	- high precision, okay recall
- what are we optimizing for? e.g. precision, accuracy, recall, etc.


Present what I've found so far with one word terms...
- we can't use see you as a signal because either:
	- they 
	- 

# Bid IDs
df[df.bid_id == 58486280]


https://stackoverflow.com/questions/37011734/pandas-dataframe-str-contains-and-operation