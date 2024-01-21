# Gamers at risk

#> sysgerm

# Intro

Whats up guys, my name is sysgerm and today we will be digging into the recent security bug that has been found in CS:GO 2 and how this affected millions of people.

# What is XSS?

Now you will probably be wondering, what even is XSS and why is it so dangerous? 

Cross-Site Scripting (XSS) is a security vulnerability that occurs when an attacker injects malicious scripts into a web application, which are then executed by the browsers of users visiting the affected site. This exploitation enables the attacker to compromise the integrity of the website, potentially extracting sensitive user information, such as login credentials or personal data. 

As u can see, this is not at all nice to find in a game with such an active player base and large player base, a lot of people were affected.

# The Works

Now that you know the basics of XSS you must of thought, well where did this vulnerability lie and how was this found?

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/cdd43e84-c0c3-4876-b7cb-e1ae164f0956/860b124d-7002-4033-a2ae-3bf28961ac4d/Untitled.png)

XSS is found in input fields, and that was also the case with CS:GO 2. The payload itself was placed into the username field and it got executed when doing a vote kick. The vote kick message box uses Valve’s Panorama UI which allowed HTML injection into the UI.

Being XSS, you could do a lot with this, it went from executing a simple video from YouTube to grabbing all the ip’s of the players in your lobby and more. The sky really was your limit.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/cdd43e84-c0c3-4876-b7cb-e1ae164f0956/367f2ae4-553f-406f-87d4-9f60e68c9564/Untitled.png)

# Can I play CS:GO 2

A couple days ago Valve released a small 7MB update that reportedly fixes the vulnerability and causes any inputted HTML to be sanitized to a regular string. 

So to answer your question, yes you can now safely play the game again.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/cdd43e84-c0c3-4876-b7cb-e1ae164f0956/ca0688f8-72ee-4558-9e8b-53fbecc050fa/Untitled.png)

# Outro

So, gamers, that wraps up our dive into the CS:GO 2 security scare. It's sysgerm here, keeping you in the loop on all things hacking. Remember, the recent XSS vulnerability might have shaken things up, but with Valve's quick response and that 7MB patch, you can get back to fragging safely.

Happy hacking!