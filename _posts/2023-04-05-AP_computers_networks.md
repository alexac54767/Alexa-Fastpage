---
toc: true
comments: true
layout: post
title: Computers and Networks (Unit 4)
description: Add Definitions from Unit 4 Computer Systems and Networks
categories: [networks, week 29, computers]
week: 29
---

## Requirements
> Work through College Board Unit 4... blog, add definitions, and pictures.  Be creative, for instance make a story of Computing and Networks that is related to your PBL experiences this year.


### How a Computer Works
> As we have learned, a computer needs aa program to do something smart.  The sequence of a program initiates a series of actions with the computers Central Processing Unit (CPU). This component is essentially a binary machine focussing on program instructions provided.  The CPU retrieives and stores the data it acts upon in Random Access Memory (RAM). Between the CPU, RAM, and Storage Devices a computer can work with many programs and large amounts of data.

List specification of your Computer, or Computers if working as Pair/Trio
- Processor GHz: 2.50 GHz
- Memory in GB: 8.00 GB
- Storage in GB: 237 GB
- OS: Windows build: 19045.2728

Define or describe usage of Computer using Computer Programs. Pictures are preferred over a lot of text.  Use your experience.
- Input devices
- Output devices
- Program File
- Program Code
    - ![definitions of input, output, file, code]({{site.baseurl}}/images/definitions1.png)
- Processes: instances of a program running in a computer
- Ports: virtual points where network connections start and end
    - For example, here are the ports in my dockerfile that this page runs on when I run localhost
    - ![port example]({{site.baseurl}}/images/exports.jpg)
- Data File:
    - one format of a data file is a csv file (comma seperated values)
    - this is a csv file I have used previously in this calss
    -  ![csv file example]({{site.baseurl}}/images/csvfileexample.png)
- Inspect Running Code: using the debugger feature to see what is going on in your code, step by step
- Inspect Variables: using the debugger feature to see when a variable is created, used, and what is assigned to it
- [My debugging example from the 2.4 lecture](https://alexac54767.github.io/Alexa-Fastpage/debugging/crud)


![Computer Hardware]({{site.baseurl}}/images/cpu.jpg)


### The Internet
> Watch/review College Board Daily Video for 4.1.1

- Essential Knowledge
    - A  <span style="color: red;">computing device</span> is a physical artifact that can run a program. Some examples include computers, tablets, servers, routers, and smart sensors.
    - A <span style="color: blue;">computing system</span> is a group of computing devices and programs working together for a common purpose.
    - A <span style="color: orange;">computer network</span> is a group of interconnected computing devices capable of sending or receiving data.
    - A <span style="color: orange;">computer network</span> is a type of computing system. 
    - A <span style="color: green;">path</span> between two computing devices on a computer network (a sender and a receiver) is a sequence of directly connected computing devices that begins at the sender and ends at the receiver.
    - <span style="color: purple;">Routing</span> is the process of finding a path from sender to receiver.
    - The <span style="color: pink;">bandwidth</span> of a computer network is the maximum amount of data that can be sent in a fixed amount of time.
    - <span style="color: pink;">Bandwidth</span> is usually measured in bits per second

- Complete Vocabulary Matching Activity.  Incorporate this into your learnings from year.  To analyze measure path and latency use `traceroute` and `ping` commands from Linux Terminal.  
    - <span style="color: green;">Path</span> 
    - <span style="color: purple;">Route</span> 
    - <span style="color: blue;">Computer System</span>
    - <span style="color: red;">Computer Device</span>
    - <span style="color: pink;">Bandwidth</span>
    - <span style="color: orange;">Computer Network</span>

> Watch/review College Board Daily Video 4.1.2

- Complete True of False Questions
    - ![4.1.2 True/False Questions]({{site.baseurl}}/images/4.1.2TrueFalse.jpg)

- Essential Knowledge
    - The internet is a computer network consisting of interconnected networks that use standardized, open (nonproprierary) communication protocols.
    - Access to the internet depends on the ability to connect a computing device to an internet connected device.
    - A protocol is an agreed-upon set of rules that specify the behavior of a system.
    - The protocols used in the internet are open, which allows users to easily connect additional computing devices to the internet.
    - Routing on the internet is usually dynamic; it is not specified in advance
    - The scalability of a system is the capacity for the system to change in size and scale to meet new demands.
    - The internet was designed to be scalable
    - Information is passed through the internet as a data stream. Data streams contain chunks of data, which are encapsulated in packets. 
    - Packets contain a chunk of data and metadata used for routing the packet between the origin and the destination on the internet, as well as for data reassembly.
    - Packets may arrive at the destination in order, out of order, or not at all
    - IP, TCP and UDP are common protocols used on the internet.
    - The world wide web is a system of linked pages, programs, and files.
    - HTTP is a protocol used by the world wide web
    - The world wide web uses the internet

- Go over AP videos, vocabulary, and essential knowledge.  Draw a diagram showing the internet and its many levels. A preferred diagram would using your knowledge of frontend, backend, deployment, etc.  Picture would highlight vocabulary by illustration. The below illustration have some ideas

![Full Stack]({{site.baseurl}}/images/fullstack.png)

- My diagram:
    - ![My diagram]({{site.baseurl}}/images/TheInternet.png)
    - ![Group's Diagram]({{site.baseurl}}/images/CSP Full Stack Diagram.png)



- Often we draw pictures of machines communicating over the Internet with arrows.  However, the real communication goes through protocol layers and the machine and then is trasported of the network.   For College Board and future Computer Knowledge you should become familiar with the following ...

```
     User Machine  <---> Frontend Server <---> Backend Server
    +-----------+         +-----------+         +-----------+
    |  Browser  |         |  GH Page  |         |   Flask   |
    +-----------+    ^    +-----------+    ^    +-----------+
    |    HTTP   |    |    |    HTTP   |    |    |    HTTP   |
    +-----------+    |    +-----------+    |    +-----------+
    |    TCP    |    |    |    TCP    |    |    |    TCP    |   
    +-----------+    |    +-----------+    |    +-----------+
    |     IP    |    V    |     IP    |    V    |     IP    |
    +-----------+         +-----------+         +-----------+
    |  Network  |  <--->  |  Network  |  <--->  |  Network  |
    +-----------+         +-----------+         +-----------+
```

The "http" layer is an application layer protocol in the TCP/IP stack, used for ***communication between web browsers and web servers***. It is the protocol used for transmitting data over the World Wide Web.

The "transport" layer (TCP) is responsible for providing reliable data transfer between applications running on different hosts.  The TCP protocol segments the data into smaller ***chunks called "segments"***. Each segment contains a sequence number that identifies its position in the original stream of data, as well as other control information such as source and destination port numbers, and checksums for error detection.

The "ip" layer is responsible for packetizing data received from the TCP layer of the protocol stack, and then ***encapsulating the data into IP packets***. The IP packets are then sent to the lower layers of the protocol stack for transmission over the network.

The "network" layer is responsible for ***routing data packets between networks*** using the Internet Protocol (IP). This layer handles tasks such as packet addressing and routing, fragmentation and reassembly, and ***network congestion*** control.


### Fault Tolerance
> Watch both Daily videos for 4.2

- Complete the network activity, summarize your understanding of fault tolerance.
    - Example 1:
        - ![Fault Tolerance ex 1]({{site.baseurl}}/images/FT1.jpg)
        - This example is fault tolerant since there are at least 2 paths to every letter. That way, if one path would go out, the network would still have ways to access the letter.
    - Example 2:
        - ![Fault Tolerance ex 2]({{site.baseurl}}/images/FT2.jpg)
        - This example is not fault tolerant. The letter F only has one path to access it. That means that if it goes out, F would be cut off completely, making the network is not fault tolerant.
    - Example 3:
        - ![Fault Tolerance ex 3]({{site.baseurl}}/images/FT3.jpg)
        - This example is not fault tolerant since A to G only has one path. If it were to go out, the letter A would be competely cut off. This means that the network is not fault tolerant. 
    - I have learned that when looking to see if a network is fault tolerant, you have to investigate all of the parts. In both of these examples that aren't fault tolerant, only one letter is the issue. Every other piece has multiple paths to it. So, you have to look carefully to ensure a network is in fact, fault tolerant.
    - Question 1:
        - ![Fault Tolerance question 1]({{site.baseurl}}/images/FTq1.jpg)
        - No matter how many paths are available for data to take in a network, it will only end up using one. This means having a fault tolerant network is "unecessary" in this situation (nothing goes wrong, fragile netowrk).
    - Question 2:
        - ![Fault Tolerance question 2]({{site.baseurl}}/images/FTq2.jpg)
        - Adding a connection between A and B would allow A to have more than 1 path, making the network fault-tolerant.

### Parallel and Distributed Computing
> Review previous lecture on Parallel Computing and watch Daily video 4.3.  Think of ways to make something in you team project to utilize Cores more effectively.  Here are some thoughts to add to your story of Computers and Networks...

- What is naturally Distributed in Frontend/Backend archeticture?  
    - Data is naturally distributed between Frontend and Backend architecture. The frontend focuses on the user experience while the backend makes that happen (makes it work).

- Analyze this command in Docker: ```ENV GUNICORN_CMD_ARGS="--workers=1 --bind=0.0.0.0:8086"```.   Determine if there is options are options in this command for parallel computing within the server that runs python/gunicorn.  Here is an [article](https://medium.com/building-the-system/gunicorn-3-means-of-concurrency-efbb547674b7)
    - in order to incorporate parallel computing, I could increase the amount of workers. As long as the amount of workers is less than or equal to 2 times the CPU plus one. Adding more workers allows for more for python applications to be opened at once, therefore using parallel computing.


> Last week we discussed parallel computing on local machine.  There are many options.  Here is something to get parallel computing work with a tool called Ray.
- Review this [article](https://www.anyscale.com/blog/writing-your-first-distributed-python-application-with-ray)...  Can you get parallel code on images to work more effectively?  I have not tried Ray.

- Code example from ChatGPT using squares.  This might be more interesting if nums we generated to be a lot bigger.

```python
import ray

# define a simple function that takes a number and returns its square
def square(x):
    return x * x

# initialize Ray
ray.init()

# create a remote function that squares a list of numbers in parallel
@ray.remote
def square_list(nums):
    return [square(num) for num in nums]

# define a list of numbers to square
nums = [1, 2, 3, 4, 5]

# split the list into two parts
split_idx = len(nums) // 2
part1, part2 = nums[:split_idx], nums[split_idx:]

# call the remote function in parallel on the two parts
part1_result = square_list.remote(part1)
part2_result = square_list.remote(part2)

# get the results and combine them
result = ray.get(part1_result) + ray.get(part2_result)

# print the result
print(result)

```