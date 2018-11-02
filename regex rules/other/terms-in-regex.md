# Scheduling

Precision: 80%
Recall: 77%

scheduling_regex_words = ['avail', 
                          'weekday', "weekend work", 'what time', 
                          'your address', 'would you like', 'what\'s the best',
                          'work for you','works for you', 'what works', 
                          'schedul','tomorrow',
                          'can you make', 'give you a call', 
                          'when i can call you', 'an appointment',
                          'reschedule', 'would you like', 'to set up', 'this week', 'next week',
                          'time for you',
                          'can you make', 'me know when', 'how about',
                          'give you a call', 'good for you', 'a good time',
                          'best for you', 'see u', 'your phone', 'see you at',
                          '([6-9]|[1][0-1])((am)|(a.m)|( a.m))',
                          '([1-9]|[1][0-2])((pm)|(p.m)|( p.m))',
                          '([7-9]|[1][0-1])( am)',
                          '([1-9]|[10])( pm)',
                          '(at )([2-9]|[1][0-2])',
                          '([1-9]|[1-2][0-2])(( :)|(:))',
                          'monday','tuesday','wednesday','thursday','friday','saturday','sunday',
                          ' mon ', ' tues ', ' wed ', ' thurs ', ' fri ', ' sat ', ' sun ',
                          'january', 'february', 'march', 'april', 'june', 
                          'july', 'august', 'september', 'october', 'november', 'december',
                          ' jan ', ' feb ', ' mar ', ' apr ', ' jul ', ' aug ', ' sept ',
                          ' oct ', ' nov ', ' dec ']

display_info_multiple(scheduling_regex_words, 'is_scheduling')

"^.*(avail|weekday|weekend work|what time|your address|would you like|what's the best|work for you|works for you|what works|schedul|tomorrow|can you make|give you a call|when i can call you|an appointment|reschedule|would you like|to set up|this week|next week|time for you|can you make|me know when|how about|give you a call|good for you|a good time|best for you|see u|your phone|see you at|7am|8am|9am|10am|11am|12pm|1pm|2pm|3pm|4pm|5pm|6pm|7pm|8pm|9pm|10pm|7 am|8 am|9 am|10 am|11 am|12 pm|1 pm|2 pm|3 pm|4 pm|5 pm|6 pm|7 pm|8 pm|9 pm|10 pm|at 7|at 8|at 9|at 10|at 11|at 12|at 2|at 3|at 4|at 5|at 6|7 :|8 :|9 :|10 :|11 :|12 :|1 :|2 :|3 :|4 :|5 :|6 :|1:|2:|3:|4:|5:|6:|7:|8:|9:|10:|11:|12:|13:|14:|15:|16:|17:|18:|19:|20:|21:|22:|monday|tuesday|wednesday|thursday|friday|saturday|sunday| mon | tues | wed | thurs | fri | sat | sun |january|february|march|april|june|july|august|september|october|november|december| jan | feb | mar | apr | jul | aug | sept | oct | nov | dec ).*$"

# Payment

Precision: 81%
Recall: 84%

payment_regex_words = ['a check', 'the check', "cheque",
                       'debit card', 'check or cash', 'cash',
                       'credit card', 'paypal', 'venmo', 
                       'deposit', 'the contract and',
                       'you can pay', 'do i pay', 'can i pay', 'should i pay',
                       'do we pay', 'can we pay', 'should we pay',
                       'pay me', 'pay you', 'pay us',
                       'do you take', 'do you accept',
                        'payment', 'invoice']

'^.*(a check|the check|cheque|debit card|check or cash|cash|credit card|paypal|venmo|deposit|the contract and|you can pay|do i pay|can i pay|should i pay|do we pay|can we pay|should we pay|pay me|pay you|pay us|do you take|do you accept|payment|invoice).*$'

display_info_multiple(payment_regex_words, 'is_payment')

# Rejection

['^.*(different route|have to cancel|keep you in mind for|hired someone else|keep your contact|to waste your time|offer, but i|need to cancel|different direction).*$',
 '98%',
 '15%',
 48]

["^.*(different route|have to cancel|keep you in mind for|hired someone else|thanks anywaykeep your contact|to waste your time|offer, but i|different direction|look elsewhere|selected another|no thanks|do not contact me|went with another|holding off|(i'm sorry).*(i don't think)|(can't make it).*(sorry)|(sorry).*(good luck)).*$",
 '100%',
 '17%',
 53]* star added to avoid pink syntax highlighting


## figure out how to write all this..
'thank you ..., but'
'thanks ..., but'
'thank you... however'
'unfortunately... not available'
- 'selected another'
'i'm sorry... i don't think'
'can't make it... sorry'
'but i appreciate'
'sorry... wasted your time'
'sorry... good luck'

- lots of phrases used in other categories, especially rescheduling

# Considering

["^.*(talk to my husband|i'll talk to|still in the process|i'll get back|i'll think about|let me discuss with my wife|let me discuss with my husband|let me discuss with my fiancé).*$",
 '89%',
 '11%',
 24]

["^.*(talk to my husband|i'll talk to|still in the process|i'll get back to you|i'll think about|let me discuss with my wife|let me discuss with my husband|let me discuss with my fiancé|still deciding).*$",
 '93%',
 '11%',
 25]


# Follow-up

["^.*(were still interested in|still need anything|wanted to follow up|wanted to check in|are you still interested|haven't heard back|i wanted to check|you to see if|openings available|if you were still|just checking in|follow up with you|wanted to reach out|checking to see).*$",
 '87%',
 '25%',
 184]

["^.*(were still interested in|still need anything|wanted to follow up|wanted to check in|are you still interested|haven't heard back|i wanted to check|you to see if|openings available|if you were still|just checking in|follow up with you|wanted to reach out|checking to see|(just).*(follow).*(up)|have you decided|(want).*(to).*(verify)|following up to see|did you decide|wanted to reach out to see|[(haven't)|(hadn't)] heard back]).*$",
 '85%',
 '31%',
 225]

- difficult because it looks like the job details and scheduling categories
