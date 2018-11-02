### Understanding why recall is down

- fixed the logic of first messages
- experiment with different keywords
- look at cases where 

- 7% of follow ups are first messages
- 74% recall for 1 day+, 30% precision

### Even after 14 days
Precision:  41%
Recall:  21%

-> look into why the precision is so low for those...

14 days...
looked at all the conversations (low precision for time gap)
(20 of them in 5 minutes), can look at 80 in 20 minutes. Time box to 10am

### Then look at the conversations that you missed in Regex
- look into 100 of them as well
- look at them for 20 minutes

# things to improve precision / recall
- not another category explicitly (e.g. reviews)
- can segment customer vs pros, usually pro that follows up
- different regexes for different segments / even categories
- e.g. wedding planning / DJ can take more time
- sentiment -> follow-ups have a more positive sentiment
- combine phrases like "how are you" with more than 14 days
- phrases like 'follow-up' may just need 2 days
- we are building a model at that point

- will finish looking into both manually and then summarize the list of reasons and the percentages


# things to do
- take like half an hour to clean it up

- fix the predict_followup function to include regex words
- so to easily change the words and see the precision and recall

- adding more regex (e.g. still in need) (1h)
	- figure out a function to do that instead of manually looking at it
	- picking up efficiency 
	- do that later though, cuz there are lots of variables

- create separate rules for customers + pros
- improved the precision by 2%, decreased recall by 1%
- find a way to make the function more efficient

- now play with different tracks and predict on a row by row basis...
- customers vs pros
	- customer regex words, pro regex words
	- get regex thing working in general before splitting customer and pro regex words
	- then split by time
	- add more stuff, still opportunity there...
- different phrases with different time
	- segregate certain phrases with different times
	- e.g. how are you can be longer
	- different categories

# done
- hours in addition to days (12, 18) (30 minutes) (DONE)
- make precision / recall function (DONE)
- message does not contain review (DONE) 
	- exclude regex (30 minutes)
	

- think about how to work more effiently in general...