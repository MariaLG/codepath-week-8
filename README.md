# Project 8 - Pentesting Live Targets

Time spent: **X** hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:
* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each version of the site has been given two of the six vulnerabilities. (In other words, all six of the exploits should be assignable to one of the sites.)

## Blue

Vulnerability #1:  SQL Injection : the SQL sleep command makes the page stall for 5 seconds, whereas for the other 2 sites it was instantaneously loaded but defaulted to a blank page

Vulnerability #2:  Session Hijacking/Fixation : Once the session ID was changed from another browser, the updated session ID worked to log into the blue website, but not the other two

<img src="https://media.giphy.com/media/uU9tmrs5HIjvNNX4QA/giphy.gif" width="800">

## Green

Vulnerability #1: Username Enumeration : If the username isn't in the database, the returned script would be unbolded.  If it was, the returned script would be bolded. On other two sites, all returned comments are bolded regardless

Vulnerability #2: Cross-Site Scripting : Once the green site opened the cross site script, the pop-up appears, as compared to the other sites where just the comment appears

<img src="https://media.giphy.com/media/7SQUcT2Q4CvufzcnT2/giphy.gif" width="800">

## Red

Vulnerability #1:  Insecure Direct Object Reference : Once the url was manipulated to id=10, the red site brought you to a hidden page, whereas the other two just defaulted to the main salesperson page

Vulnerability #2: Cross-Site Request Forgery : Once the csrf token value was changed, in the red site it was still possible to update the name, but in the other two it gave an error message.

<img src="https://media.giphy.com/media/2wgWse5BRpcnyGmPK8/giphy.gif" width="800">

## Notes

Describe any challenges encountered while doing the work
constant error messages from the website during login even though login info was correct. 
