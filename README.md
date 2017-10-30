# Project 8 - Pentesting Live Targets

Time spent: **X** hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:

[X] Username Enumeration

[X]Insecure Direct Object Reference (IDOR)

[X] SQL Injection (SQLi)

[X] Cross-Site Scripting (XSS)

[ ] Cross-Site Request Forgery (CSRF)

[X] Session Hijacking/Fixation

Each version of the site has been given two of the six vulnerabilities. (In other words, all six of the exploits should be assignable to one of the sites.)

## Blue

Vulnerability #1: SQL Injection (SQLi)

Vulnerability: The Salesperson page allows user to inject SQL code into the id number. To recreate replace the id number to   %27%20OR%20SLEEP(5)=0--%27 will inject the SQL code after 5 seconds. 

GIF Walkthrough: 

<img src="https://github.com/dhruvp5/CodePathCyberSecWeek8/blob/master/Asg8_2.gif?raw=true" alt="gif">


Vulnerability #2: Session Hijacking/Fixation

Vulnerability: This exploit allows an user to gain access to the blue site without actually logging into it. When you have Red and Blue site up, you can login into Red Site and you can gain access to the Blue Site automatically by clicking the login button into the Blue Site.

GIF Walkthrough: 

<img src="https://github.com/dhruvp5/CodePathCyberSecWeek8/blob/master/Asg8_6.gif?raw=true" alt="gif">


## Green

Vulnerability #1: Username Enumeration

Vulnerability: When an username is entered, like "jmonroe99" with a random passoword, the user will recieve an error stating      that the login was unsuccesful in a bold font. When a random username is typed in with a password the error message is popped up without the bold font. A random attacker can figure out the usernames in the database using this exploit.

GIF Walkthrough: 

<img src="https://github.com/dhruvp5/CodePathCyberSecWeek8/blob/master/Asg8_0.gif?raw=true" alt="gif">

Vulnerability #2: Cross-Site Scripting (XSS)

Vulnerability: Entering an XSS Attack in the "Feedback" section of the "Contact" will store the attack in the database. So, when the admin tries to access the feedbacks in order to answer any questions, they unlock the trap which in this case is just a normal pop-up. Whereas, site Red and Blue have protection against this vulnerability which will store the attack as a text and not run the XSS attack like the green site.

GIF Walkthrough: 

<img src="https://github.com/dhruvp5/CodePathCyberSecWeek8/blob/master/Asg8_3.gif?raw=true" alt="gif">

## Red

Vulnerability #1: Insecure Direct Object Reference (IDOR)

Vulnerability: Site Red has the information for two users not blocked. Therefore, information for users with "id=10" and "id=11" have their information out to the public before time or for people that are not working with the company anymore. Whereas, site Green and Blue have the users id blocked. This way only the people currently working with the company have their information out for the public to look at. This exploit can be easily be used for user data breach or other instances of information leak.

GIF Walkthrough: 

<img src="https://github.com/dhruvp5/CodePathCyberSecWeek8/blob/master/Asg8_1.gif?raw=true" alt="gif">

Vulnerability #2: __________________


## Notes

Describe any challenges encountered while doing the work
