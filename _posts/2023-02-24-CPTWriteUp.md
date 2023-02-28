---
toc: true
comments: true
layout: post
title: My CPT Write Up
description: Similating the Collegeboard written portion of the AP test for my project
permalink: /project/CPTwriteup
categories: [week 24, CPT project, role, collegeboard]
--- 

## Based on this [Collegeboard rubric](https://apcentral.collegeboard.org/media/pdf/ap22-sg-computer-science-principles.pdf)

- Row 1 (Program Purpose and Function): 
    - the purpose of my program is to aid ISPE students to stay organized and ensure they get credit for their class
    - my program works (functionality) by allowing users to input their workouts and corresponding grade, and see the following inputs on the page in an organized table
    - the user inputs a workout by typing their "Name", "Date of Completion", "Number of Hours Completed", "Grade" and click submit
    - the output of the program is that the data appears in a table below


- Row 2 (Data Abstraction): 
![how data is stored]({{site.baseurl}}/images/howrow2CPT.jpg)
<br>

![data in SQLite Table]({{site.baseurl}}/images/Row1ISPESQLITECPT.jpg)
<br>

![data is used]({{site.baseurl}}/images/usedrow2CPT.jpg)
<br>
    - name of collection type (database class): ISPE
    - data in this class is the data (workouts) that the user inputed


- Row 3 (Managing Complexity):
![ISPE Class]({{site.baseurl}}/images/howrow2CPT.jpg)
<br>

    - without the use of the class in the database, the inputed data would be very unorganized in a list and would only be stored locally. However, I could store the data in a list and use a rest API to connect the frontend and backend. However, it would be very tedious since I would have to manually add data to the backend. It would be much more difficult to update, debug, and add data.


- Row 4 (Procedural Abstraction): 
![Create function defined]({{site.baseurl}}/images/definecreateISPECPT.jpg)
<br>

![Create funtion used]({{site.baseurl}}/images/ISPEcreateCPT.jpg)
<br>

    - This function "create_ISPE" takes the iputted data (parameter) and iterates through the variables that the user inputs (name, date, duration, grade). It then defines them as constants, posts them, and autogenerates them into the table diplayed on frontend. This allows the data inputed by the user to actually show up in the table, carrying out the purpose of the program.


- Row 5 (Algorithm Implentation):
![class_read]({{site.baseurl}}/images/classreadCPT.jpg)
<br>

![frontend using data from class_read]({{site.baseurl}}/images/readISPECPTrow5.jpg)
<br>

    - This class in my API is defining a get funtion that recieves the data from the frontend, and jsonifies the data. It does this by going through a sequence where it first extracts all the exisiting data, reads it, and then rewrites it as a JSON format. The second piece of code pictured then fetches the data that is in JSON format by using GET methods. This frontend uses the funtion read_ISPE to refrense the class_read function in the backend. In order to do this, it goes through a series of conditionals (selection), to determine if the data is valid and ready to be added to the database. If it produces a response error, then the funtion is returned. If the data is valid and in the correct format, then it will be added to the table which will be displayed to the user.


- Row 6 (Testing): 
    - First call: The user inputs the workout, "John Doe, 1/27/2023, 2, A" (valid data) into the form and clicks submit
        - conditions being tested: checks if data is valid and if it can be added to the database
        - result: data will appear in the table below with the corresponding data
    - Second call: user enters the invalid data "B" into the field: "name"
        - Conditions being tested: checks if the data inputted is valid (more than 2 characters) to be put in the database
        - result: the program will alert the user "Name is missing, or is less than 2 characters, please refresh and enter a valid name"
