# Project 8 - Pentesting Live Targets

Time spent: **X** hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:

[X] Username Enumeration

[X]Insecure Direct Object Reference (IDOR)

[ ] SQL Injection (SQLi)

[ ] Cross-Site Scripting (XSS)

[ ] Cross-Site Request Forgery (CSRF)

[ ] Session Hijacking/Fixation

Each version of the site has been given two of the six vulnerabilities. (In other words, all six of the exploits should be assignable to one of the sites.)

## Blue

Vulnerability #1: __________________

Vulnerability #2: __________________


## Green

Vulnerability #1: Username Enumeration

Vulnerability: When an username is entered, like "jmonroe99" with a random passoword, the user will recieve an error stating that the login was unsuccesful in a bold font. When a random username is typed in with a password the error message is popped up without the bold font. A random attacker can figure out the usernames in the database using this exploit.

GIF Walkthrough: 

<img src="https://github.com/dhruvp5/CodePathCyberSecWeek8/blob/master/Asg8_0.gif?raw=true" alt="gif">

Vulnerability #2: __________________


## Red

Vulnerability #1: Insecure Direct Object Reference (IDOR)

Vulnerability: Site Red has the information for two users not blocked. Therefore, information for users with "id=10" and "id=11" have their information out to the public before time or for people that are not working with the company anymore. Whereas, site Green and Blue have the users id blocked. This way only the people currently working with the company have their information out for the public to look at. This exploit can be easily be used for user data breach or other instances of information leak.

GIF Walkthrough: 

<img src="https://github.com/dhruvp5/CodePathCyberSecWeek8/blob/master/Asg8_1.gif?raw=true" alt="gif">

Vulnerability #2: __________________


## Notes

Describe any challenges encountered while doing the work
