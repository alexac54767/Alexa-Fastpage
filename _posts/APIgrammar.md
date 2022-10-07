---
toc: false
comments: true
layout: post
title: Grammar/Spelling API
description:This API will help the users of our final project to have good spelling and grammar.
permalink: /markdown/1
image: /images/thumbs up.jpg
categories: [week 7]
---

{% include nav_data.html %}

import requests

url = "https://dnaber-languagetool.p.rapidapi.com/v2/languages"

headers = {
	"X-RapidAPI-Key": "7798c19b40msh9672054d4a4cb3cp176d9cjsn9d6a5cf1b9bf",
	"X-RapidAPI-Host": "dnaber-languagetool.p.rapidapi.com"
}

response = requests.request("GET", url, headers=headers)

print(response.text)