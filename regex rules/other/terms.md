# TO DO: Tina to finalize the set of words to use by picking from the scheduling_terms list

scheduling_regex_words = ['avail', 
                          'weekday', "weekend work", 'what time', 
                          'your address', 'would you like', 'what\'s the best',
                          'work for you','works for you', 'schedul','tomorrow',
                          'monday','tuesday','wednesday','thursday','friday','saturday','sunday',\
                          ' mon ', ' tues ', ' wed ', ' thurs ', ' fri ', ' sat ', ' sun ',
                          'can you make', 'give you a call', 
                          'when i can call you', 'an appointment',
                          'reschedule', 'would you like', 'to set up', 'this week', 'next week',
                          'can you ;make', 'me know when',
                          'give you a call', 'good for you', 'a good time',
                          'best for you', 'see u', 'your phone', 'see you at',
                          '7am','8am', '9am', '10am', '11am', '12pm', '1pm', '2pm', 
                          '3pm', '4pm', '5pm', '6pm', '7pm', '8pm', '9pm', '10pm',
                          '7 am','8 am', '9 am', '10 am', '11 am', '12 pm', '1 pm', '2 pm', 
                          '3 pm', '4 pm', '5 pm', '6 pm', '7 pm', '8 pm', '9 pm', '10 pm',
                          'at 7', 'at 8', 'at 9', 'at 10', 'at 11', 'at 12', 
                          'at 2', 'at 3', 'at 4', 'at 5', 'at 6', 
                          '7 :', '8 :', '9 :', '10 :', '11 :', '12 :', 
                          '1 :', '2 :', '3 :', '4 :', '5 :', '6 :',
                          '7:30', '8:30', '9:30', '10:30', '11:30', '12:30', '1:30',
                          '2:30', '3:30', '4:30', '5:30', '6:30',
                          '7:15', '7:45', '8:15', '8:45', '9:15', '9:45', '10:15', '10:45',
                          '11:15', '11:45', '12:15', '12:45', '1:15', '1:45', '2:15', '2:45',
                          '3:15', '3:45', '4:15', '4:45', '5:15', '5:45', '6:15', '6:45',
                          'january', 'february', 'march', 'april', 'june', 
                          'july', 'august', 'september', 'october', 'november', 'december',
                          ' jan ', ' feb ', ' mar ', ' apr ', ' jul ', ' aug ', ' sept ',
                          ' oct ', ' nov ', ' dec ']

scheduling_regex_words = ['avail', 
                          'weekday', "weekend work", 'what time', 
                          'your address', 'would you like', 'what\'s the best',
                          'work for you','works for you', 'schedul','tomorrow',
                          'monday','tuesday','wednesday','thursday','friday','saturday','sunday',\
                          ' mon ', ' tues ', ' wed ', ' thurs ', ' fri ', ' sat ', ' sun ',
                          'can you make', 'give you a call', 
                          'when i can call you', 'an appointment',
                          'reschedule', 'would you like', 'to set up', 'this week', 'next week',
                          'can you ;make', 'me know when',
                          'give you a call', 'good for you', 'a good time',
                          'best for you', 'see u', 'your phone', 'see you at',
                          '%dam', (d between 6-11), "([7-9]|[1][0-1])(am)",
                          '%dpm', (d between 1-12),
                          '%d am' (d between 6-11),
                          '%d pm' (d between 1-12),
                          'at %d' (d between 2-12),
                          '%d :' (d between 1-12),
                          'd:', (d between 1-23),
                          'january', 'february', 'march', 'april', 'june', 
                          'july', 'august', 'september', 'october', 'november', 'december',
                          ' jan ', ' feb ', ' mar ', ' apr ', ' jul ', ' aug ', ' sept ',
                          ' oct ', ' nov ', ' dec ']

display_info_multiple(scheduling_regex_words, 'is_scheduling')
- 80% precision, 77% recall, 3979


payment_regex_words = ['a check', 'the check', "cheque",
                       'debit card', 'check or cash', 'cash',
                       'credit card', 'paypal', 'venmo', 
                       'deposit', 'the contract and','do you accept',
                       'you can pay', 'do i pay', 'can i pay', 'should i pay',
                       'pay me', 'pay you', 'pay us',
                       'do you take', 'do you accept',
                        'payment', 'invoice'
                    ]

display_info_multiple(payment_regex_words, 'is_payment')
- 81% precision, 84% recall

['^.*(a check|the check|cheque|debit card|check or cash|cash|credit card|paypal|venmo|deposit|the contract and|do you accept|you can pay|do i pay|can i pay|should i pay|pay me|pay you|pay us|do you take|do you accept|payment|invoice|& quote).*$',
 '81%',
 '84%',
 366]