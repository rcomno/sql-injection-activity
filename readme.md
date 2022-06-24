## SQL Injection Assingment Answers

###### Rocco Mannino June 24 2022

_Wasn't sure if these where nessicary to include or not._

#### 1 Given what you already know about SQL, can you spot our vulnerability?

Guessing that because there isn't any sort of filtering/restrictions on the HTML side to prevent the insertion of text that could be
converted to code that if someone where to insert text that can be read as code it would be. Also the fuction that takes the password/
username in has no filtering either.

#### 2 What happened?

'1'='1' inserted in to password:
Page displayed the error message. Terminal displayed UN/PW and query as expected along with error messages.

'unknown' inserted in to password:
Same as above neither affected the default UN/PW.

_Addendum: 'unknown' was worng format as was '1'='1'_

unknown' inserted in to password:
Same as above neither affected the default UN/PW.

'1'='1 inserted in to password:
Same as above neither affected the default UN/PW.

#### 3 Taking your best guess, what do you think happened?

All caused error out puts to the terminal based on reading those outputs it appears to be messing around with
the json files and the express framework(api?) itself. Also it looks like it may have thrown the error due to
trying to pull a '1'='1'/'unknown' password where there was none. Honestly I'm not really sure what I'm looking
at and google is't being helpful so can't really say whats going on.
