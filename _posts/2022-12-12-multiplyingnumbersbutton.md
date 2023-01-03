---
toc: true
comments: true
layout: post
title: multiplying javascript button 
description: button for group 6 hacks
permalink: /collegeboard/students/groupsix/multiplicationbutton
image: /images/thumbs up.jpg
categories: [week 15]
---

## Multiplying 2 Numbers
<button id="enter" onclick="print(a,b)">Multiply</button>
<p id="result"></p>
<script>
    function print(a,b) {
        document.getElementById("result").innerHTML = a * b
    }
    var a = 1
    var b = 2
</script>

```html
<!-- function is called here -->
<button id="enter" onclick="print(a,b)">Multiply</button> 
<p id="result"></p>
<!-- javascript -->
<script>
    function print(a,b) {
        document.getElementById("result").innerHTML = a * b // math
    }
    // variables are defined
    var a = 1
    var b = 2
</script>
```