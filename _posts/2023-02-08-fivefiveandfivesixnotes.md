---
toc: true
comments: true
layout: post
title: 5.5 and 5.6 (Legal and Ethical Concerns/Safe Computing) Notes/Reflection
description: Taking notes and reflecting on the 5.5 and 5.6 lessons.
permalink: /collegeboard/chapterfive3
categories: [week 22, collegeboard, notes]
--- 

## 5.5 Legal and Ethical Concerns
- License Communities, License Types
    - **closed source** (capitalism, make $): pay to use
    - **open source** (ex: GPL/MIT License): can go grab (concerns: can use but can't sell)
- Digital Rights
    - terms and conditions
    - music
- Patents
    - can pantent phrases like "app store"

### Summary:
> Every company needs to make a living. With capitalism, one of the best ways to do that is with closed source licenses. However, open sourced licenses allow for the code to be more community based. There are more contributions and the code is more useful. However, if you use open sourced code, you cannot sell your product. Similarly, there are digital rights. Every time you accept terms and conditions on your phone/comupter, you are accepting digital rights. Another example of digital rights is licensing to music on your phone. If I pirate music from Beyonce, I am not following her digital rights and she gets less money.

- Flask/Backend License:
![flask license]({{site.baseurl}}/images/flasklicense.jpg)

- Frontend License:
![project license]({{site.baseurl}}/images/Fitness4Baddieslicense.jpg)

- Team Fastpage license:
![team fastpage license]({{site.baseurl}}/images/teambaddieslicense.jpg)

- Personal Fastpage license:
![personal license]({{site.baseurl}}/images/personallicense.jpg)

- My team and I chose the open source MIT license for all our projects and for our personals. However, our frontend repository already had the "Apache" license so we left that one in place. The MIT license allows anyone to edit, ditribute, or use it personally or commercially, as long as they give us credit. We believe this is the best option for us since we are not working on anything top secret, and we would love community input and support.



## 5.6 Safe Computing
- never ride skateboard and compute at the same time!
- concerns with computing: 
    - malware
    - phishing attacks
    - identity theft
    - stolen information (passwords, credit cards, bank accounts)
    - Personal Identifiable Information (PII) can be beneficial or harmful
- encription:
    - two-factor authentication (2FA)
    - ^ ex: sending email with code/link

## Hacks

- Describe PII you have seen on project in CompSci Principles.
    - In APCSP, I have seen PII. I think the most common are our names, github usernames, and information that we put in our projects (such as tester data that is our actual information).

<br>

- What are your feelings about PII and your personal exposure?
    - I always feel a little nervous about having my information out. But, I do put myself out there with things like social media so my name and some basic info (such as DNHS, class of 2024, my cheerleading organization/team) are open to the world to see. I realize that is probably a little more risky, however, it allows others to connect with me (like if a cheerleader from the same organization found my account). Also, my common email happens to be my first, middle, and last name all in one. I have been told that it is dumb to be giving out that information, but I have yet to stop using that email.

<br>

- Describe good and bad passwords? What is another step that is used to assist in authentication.
    - a good password is one that has many characters, both letters and numbers, and symbols. It is more difficult to guess and come up with. Bad passwords are either very common and not intricate, or contain personal information. For example, if I made my password alexac, it would be very bad since my name is very accessible (PII).

<br>

- Try to describe Symmetric and Asymmetric encryption.
    - Symmetric encryption only uses one key to encrypt/decrypt. It is a form of security, but isn't as strong as Asymmetric encryption. Asymmetric encryption uses two different keys, a public and secret key, to encrypt and decrypt. 

<br>

- Provide an example of encryption we used in AWS deployment.
    - When creating and deploying our projects in AWS, we used Asymmetric encryption. We had to generate the public and secret keys and then add them to our repositories. 

<br>

- Describe a phishing scheme you have learned about the hard way. Describe some other phishing techniques.
    - There have been many phising schemes on instagram lately. The hackers try to sound personal and like your friend. There was one I fell for a long time ago where one of my "friends" on insta direct messaged me a link that they claimed had a "bad photo" of me. Theyt made it sound urgent and I was curious. In order to "view the photos" you had to sign into your instagram account. I tried to multiple times, but lucklily forgot my password. Ava then pointed out to me that it was clearly a scheme, and that I should avoid clicking on anything suspicious on instagram dms.