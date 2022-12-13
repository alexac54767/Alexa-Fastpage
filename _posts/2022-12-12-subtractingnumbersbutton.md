---
toc: true
comments: true
layout: post
title: adding javascript button 
description: button for group 6 hacks
permalink: /collegeboard/students/groupsix/subtractionbutton
image: /images/thumbsup.jpg
categories: [week 15]
---

## Subtracting 2 Numbers
<button id="enter" onclick="print(a,b)">Subtract</button>
<p id="result"></p>
<script>
    function print(a,b) {
        document.getElementById("result").innerHTML = a - b
    }
    var a = 1
    var b = 2
</script>

```html
<!-- function is called here -->
<button id="enter" onclick="print(a,b)">Subtract</button> 
<p id="result"></p>
<!-- javascript -->
<script>
    function print(a,b) {
        document.getElementById("result").innerHTML = a - b // math
    }
    // variables are defined
    var a = 1
    var b = 2
</script>
```