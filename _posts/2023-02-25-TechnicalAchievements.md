---
toc: true
comments: true
layout: post
title: Technical Achievements for my CPT Project
description: Describing the technical difficulties and acheievements of my project!
permalink: /project/technicalachievements
categories: [week 24, CPT project, role, collegeboard]
--- 

## Technical Achievements and Difficulties in my Project

[My feature's database file](https://github.com/avac54765/teambaddieflask/blob/main/model/ISPEs.py)
[My feature's API file](https://github.com/avac54765/teambaddieflask/blob/main/api/ISPE.py)

### Diffifulties and how we Overcame Them!

> Starting off with little knowlege on databases, this project was definitely difficult. By using the resources Mr. Mortensen gave us and a lot of troubleshooting/debugging, we were able to accomplish this project!
- having multiple classes within one database: we originally didn't understand that we needed different database files, we started off with one that had 4 different classes. It had worked and showed up correctly in our SQLite table, however, it made it very difficult to create and connect an API to it. Once we had seperate files, it was much easier to keep track of our work and add other elements.
![SQLite Table]({{site.baseurl}}/images/Row1ISPESQLITECPT.jpg)
- defining vars and notes schema for our projects (determining what type of input each var was going to be)
![ISPE defining notes schema]({{site.baseurl}}/images/howrow2CPT.jpg)
- SYNTAX! Trying to debug syntax was definitely a challenge. It took looking at errors, changing one thing at a time, and testing over and over again. Things like a capital letter or an underbar before a var made all the difference.
- Garbage Data: I spent lots of time trying to determine how I could make the API the most efficient in eliminating garbage data. However, with the input of others, I realized that one of the most effective ways to do this is to not allow the user to input incorrect values in the first place. So, I changed the HTML 5 input type on frontend to only allow the user to input certain options.
![ISPE API]({{site.baseurl}}/images/ISPEapiCPT.jpg)
- Setter/Getter Functions: These still confuse me a little. I understand that these funtions are necessary to create a var and to retrieve their data. However, editing them was difficult. I needed to take it much slower than I normally do, since it requires more attention to detail. Many elements needed to be added/changed between vars, and I made lots of little mistakes. These mistakes made it tedious to test and debugg my code.
![ISPE setters/getters]({{site.baseurl}}/images/setterandgetters.jpg)


### Our Main Strategies:
- Teamwork! If one member had an issue, we all tried to help and solve it.
- Sharing our mistakes and solutions: Many times if there was an issue in our code that was not a typo/misunderstanding, we all had the same issue. So, when we troubleshooted and debugged to form a solution, we shared that fix with the group.
- Comparing code: This strategy helped us greatly in this project. If one member's code was working as intended but another's had errors, we compared the code side by side to see if we could identify an error. We caught many mistakes/typos this way.