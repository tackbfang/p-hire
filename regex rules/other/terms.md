# Rejection Regex

unfortunately
hired
out
already
different
cancel
but i 
sorry, i 
so sorry
to cancel
hired someone
thanks again
different route
i just
have decided
i apologize
already hired
, sorry

, but i
keep you in mind
a different route
have to cancel
unfortunately, i
but i'm
i am not
i am sorry
sorry but
will keep your
will have to
to go with
need to cancel
to cancel this
have decided to
so sorry i
am so sorry
not going to
the future.
to cancel this
hired someone else
at this time
i have decided
we have decided
doesn't work

thank you for your time

rejection_regex_words = ['different route', 'have to cancel',
                         'keep you in mind for', 'hired someone else',
                         'keep your contact', 'to waste your time', 'offer, but i']

Precision: 100%, Recall 14%

Precision: 98%, Recall 15% with "need to cancel"

# Considering

considering_regex_words = \
['talk to my husband', 'i\'ll talk to', 'still in the process',
 'i\'ll get back', 'i\'ll think about', 'let me discuss with my wife',
 'let me discuss with my husband', 'let me discuss with my fiancé']

display_info_customers_multiple(considering_regex_words, 'is_considering')

Precision: 100%, Recall 4%
Precision: 89%, Recall 11%

# Follow-up

follow_up_regex_words = \
['were still interested in', 'still need anything', 'wanted to follow up',
 'wanted to check in', 'are you still interested', 'haven\'t heard back',
 'i wanted to check', 'you to see if', 'openings available', 'if you were still',
 'just checking in', 'follow up with you']

display_info_multiple_new(follow_up_regex_words, 'is_follow_up')

Precision: 89%, Recall: 22%







