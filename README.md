# study_progress
What I have studied since Oct 18th, 2017. Most recent additions are first.

## 11/8

At this point, going to pairboarding has been really helpful for me, in considering new toy problems regularly. My plan is to keep going twice a week and attend the DandI roundtable discussion until I get hired and start a new position. It's a great social atmosphere. Today's problems were tough - the first one required discovering the math trick when writing out a pattern. The second one required a lot of questioning to determine valid inputs and possible outputs. Very challenging problems. 

## 11/7

I did the tryplebyte interview on a whim, but I knew what was coming. It was actually a challenging, and valuable experience. Things I forgot to know: 1. Traverse a linked-list in a hashmap's bucket, and just wait until you reach the value you're looking for 2. Bloom filters tell you whether something is in a set (not really sure when do use that) 3. To find the kth largest element in a binary search tree, just do reverse order traversal.

IMSLP offered to let me work on their project. That will be satisfying.

## 11//6 

Two interesting algorithms crossed my path today. The first is the Bellman Ford algorithm - I understand how it works but I don't know how to conceptualize the proof that is always works. The second is the Boggle Board question, where the optimized solution is to dfs the board but using a prefix tree to narrow my traversal. Tomorrow, I will undertake my first systematic exploration of the Bellman Ford algorithm with the help of a lecture from MIT. Walking through the process will be super helpful.  At this point, my goals is to study algorithms everyday, write code, and try to get a job using codesignal and my referrals. I will also do the tryplebyte interview once's I've built a kanban and tic tac toe using web components, using the JR architectural pattern (writing all business logic with CSS), I haven't done any front end since I stopped working. I will also offer to contribute the IMSLP website, as they need some serious help with their UI. At the very least, it needs to be mobile responsive. 

## 11/5 

This post will attemp to explain the solution to the CodeSignal Problem: flightPlan, which I completed in Ruby today. I solved eleven out of twelve tests and hard coded the last one because of the way I treated the problem. My solution was O(n^2) because of the boilerplate needed to set up the test, but there was an O(m * log n) solution that I'm trying to understand on CodeSignal, and here I will try to explain how it works. The solution is to create a graph where the edges are the flights and the vertices are the cities, then go through the graph to find out how soon we can get from source the destination. Start with the source, and then store a hash of the valid destinations mapped to the arrival time at that destination. Then start again but with the earliest flight, and look again. Be sure to delete the origin after searching it, and update any current nodes with an earlier arrival time if it exists (in other words, if I go from Chicago to Denver, but can get to Denver sooner if I go through a connecting city, then account for that option). According to method, we will find the shortest route to the destination if we keep iterating until land at the destination. As long as we choose, out of the current possible destinations available so far, the earliest one, we will find the shortest route to the destination. in other words, there will never be a time where we find a route to the destination but it is the suboptimal route, because we will first check other destinations that are arriving earlier, and if they provide a link to the destination, we will update the destination mapping with the earlier arrival time. Brilliant. 

My solution was not good - I built a graph that linked all flights to valid previous flights, and then checked whether we could trace a flight back to the origin, starting with the earliest arrival. Not space efficient, time complexity is polnomial. 

## 11/4

Looking through my linkedIn account, I suddenly realized just how many engineers I've met in SF, and how many great companies have hired my connections. I've also notice how some people found companies that matched their interests, and it made me wonder what exactly is my best thing. Recently, I've been teaching music to some students, and doing that has made me a lot more interested in music again. Additionally, I've been composing some pieces, and I've enjoyed that. Even more, I know that I'm a coder with this skill and ability, and perhaps I've supposed to get back into research for AI, the ideas have been percolating for a long time but not come to fruition, except with Theorizer. Now however, since starting to work a litle bit with Tor, I've realized that the same amount of work and energy would be required in both fields, but my interested in the mind and the humanities is very strong, and something I continued doing through WSI, and there has to be a way for me to engage with the humanities as a coder, and of course the first thing I think is AI - understanding the mind, how it works, what it does and how it does it. The pursuit of describing the mind, is it something I've been doing since the beginning, and what could I do from here to continue that journey - well, the answer is obviously to go back to school, or acquire the money to begin an investigation of questions myself - which are naturally: how can the mind create a work of music that is excellent? How can a mind interpret a musical score? How is language understood in the mind? What should I do next here? How do the neurons work? How do the connections work? What is my place in the process of understanding these questions? Why is there violence? The spiritual questions - what is my place in understanding these questions? What is the right thing for me to do next in this world of software and my love for music and the arts? 

Working on FlightPlan on code signal - it's a DFS problem, but good god why do I have to rewrite DFS again? 

## 11/2 

Progress with TOR. I have successfuly run the Tor client from my mac, and used an industry browser to connect to an onion service. I have accomplished the same thing on my linux box, with the added bonus of having built Tor from source and run it locally. I have concluded that running a relay might be too expensive for me, but that incentivizes me to find someone who is running one successfully and learn from them. My next task is to make a sucessful API request from Postman or similar, which did not work yesterday. I was able to hit tor but it interpreted the postman request as an HTTP request, which of course it is, but someone all other traffic interfaces correctly with the TOr client. I will investigate this further. Once i do it on mac, I then need to do it on my linux box. 

My goals for the contributing to Tor are threefold: 1. To learn a low level langauge (C), to learn more about web infrastructure, to build my credentials, to investigate my interest in security, and of course keep my coding skills sharp. 

Additional work for me includes re-learning Ruby and algorithms so that I can pass interviews. My google interview rejected me because I couldn't consider all the test cases up front, so my goal in solving algorithms will be to do a better job of this, and of course keep learning new ways to solve them. 

I need to some metric of how I know when I'm ready to apply to Dropbox, I'm not sure. I think a good metric would be when I complete codesignal interview practice? I don't really know. I just need to do it alot. I think in one week, I will reassess my readiness. 

Lastly, today is my birthday, and my resolution for this year, is to approach every action from a place of gratitude. I used to be a lot happier because I had more gratitude, and if I were to change in my life, it would simply to be happier more often, and the way I do that is by actively have gratitude for what I have, so that is my plan. 

## 11/1

It's back on the job search for Adrian Jewell. My paid internship completed successfuly with lots of valuable lessons learned. There are so many things worth learning but the most important task is to get a new job, a really good one with smart teammates, organized management, challenging technical problems, and potential for growth and professional development. My interest is in software companies or working directly with scientists.  

My side project during my job search will be contributing to the Onion Router. The next steps in this process are to run the client locally, make an API request, and then build the client locally from source and make a successful api request. 

## 2/22 

Interesting problems : Parse Words (from Tony), Word Search (from April), 

## 2/19 
Today I studied in-order traversal in constant space. It's called Morris traversal - so beautiful. I want to get a firm grasp of algorithms before starting in two weeks. I think I will do this. That's 43 problems to get the fundamentals.  

## 2/18
For the next two weeks, the best thing for me is to get a stronger grasp of JS fundamentals, working with the browser, the DOM, HTTP requests, testing framewors (Jest Enzyme, Mocha, Karma, Jasmine). Working with D3 might be something worth doing, for my own education. Another project is a really good idea, and working with D3 is a good way to get a solid take on the fundamentals again. So finish react-crypto-graph is week and then do something next week with D3. The testing frameworks, I keep wanting to do them but they're such a pain in the butt. Just comment your code well. 

## 2/17

I got a job - now the real work begins. It's time to start thinking long term about this career. 

## 2/15, 2018 

Actively interviewing - Boston, SF, another today- no time to make git commits. Studied a lot of algorithsm. My mind is rushing. Hoping to settling things asap. 

## 2/9, 2017
I'm looking for a better way to detect when linked in is on the feed. I can't detect an object, because a new instance is created when I reload the feed window, so I can't do MutationObserver. I also cannot use Proxy because I cannot set window.location to a proxy with location and a handler. So right now, I'm just listening to window.location.href and checking it's value. Browsers need an #onhashchange for window.location.href 

## 2/8
How do proxies work?

## 1/30
James is a good guy, and linked lists are challenging.


## 1/29

Remember to reset your indices variable when you're testing a while loop in pry. Also, remember certain special Ruby hash functions. They add a certain convenience to working with them, but also can be complicated. 

## 1/26

I had a chance to go through some Code from a hack-a-thom competitor. They built a blockchain from scratch in Python. It was cool to read. They implemented a simple proof-of-word hash algorithm. Very interesting. It basically runs a hashing function, incrementally adding bits to the thing being hashed, until the first 5 digits come out 0000, takes about 20 seconds. THey also attempted a merkle root tracker, which didn't really do the job because it they just kept a single hash of all the transations, rather than build a tree data structure (tisk tisk).  Still very intersting to read. 

## 1/25

The HiR position is taking up a portion of my time. The next things on my mind are to keep working on algorithsms, and stay focused on Ruby and JS as my languages. Improve my skill with them and stay focused. The other thing for my to do is write a webapp that removes my web feed on LinkedIn. This is the next things on my goal of becoming a security expert. That is the next thing on my mind. 

## 1/12

Working thorugh map decode again was an experience. The solution worked for the test cases, but how someone came up with the solution is still beyond me. It really blows my mind. More practice is required.

## 1/8

There's more to say about algorithms. This weekend, I tackled mapDecode from Google's database of algorithms, and also worked with my friend on a problem called swapLexOrder. Both questions were quite tricky.  Figuring out swapLexOrder made sense after reading through a solution, but mapDecode still doesn't make sense.  

swapLexOrder askes the solver to find the lexicographically greatest string given pairs of indices that can be swapped. The insight (which is really the best way to describe it) is to understand that pairs of indices that having common indices can be grouped into a larger pairs, and so the the strategy is the build these larger clumps with sets, sort the letters in these clumps, and then put them back into the string at their new positions. The two insights are thus: 1. Understanding clumping of indices (it's kind of a threading concepts. ie. 1/4, and 2/4, means that you can swap 1/2/4 between themselves), and secondly that you can sort them and the 'sum of lexicographically sorted parts' will yield the lexicographically sorted whole. 

MapDecode is a number story. The solution is something like six lines in Ruby, and it is fundamentally a dynamic programming task, but with a catch, given a few things. I haven't figured out how to get to the solution, despite having memorized it. So I won't share any more until I have it down. 

## 1/5
Sitting down to crack algorithms really hard for me. There is a technique there, and I have to keep doing it. It's hard.

## 1/4

Presenting Heaps with the man Cory. 

## 1/3
There are a lot of open source projects out there and it would be great to find a good one. I've hit up two of them. One of them had an issue I couldn't replicate because the instructions were quite vague. The other one is rather obscure, so I'm going to keep looking for other ones to start looking.

The allure of learning python is strong, but I'm not going to touch python unless it relates a project that excites me, and I'll just use the doc to get syntax info, but I don't really anything about how python works, is compiled, written under the surface, or anything like that. 

Security, is also a definite interest of mine, security is definitely how I'm going to further my dev as a software engineer. 

## 1/2

Some strategies that work when using algorithms.
1. Using Dynamic programming to store a result "so far" so that previous results don't have to be recalculated against and a gain.
2. Using a hash to store references to things, instead of having to find them again.
3. Using Metadata to store information so the the information doesn't have to be found again. 
4. Sorts that do things faster (heap sort, quick sort, trees) 
The fundamental strategies here are to add a little bit of extra space inorder to save on a whole lot of speed.

## 12/31 
Happy new year. I never thought this whole 'new year' thing meant anything, but it actually has given me a lot to consider. Recently I was able to clarify my priorities in life, not that they were any different, but it wasn't until recently that I realized that I had forgotten them amidst the rush of completing App Academy and becoming a software developer. For the duration of my time at App Academy, I allowed myself to shift my priorities from that of health to that of complete focus on the course. When the course ended, I forgot to shift back to my normal priorities, which is fundamentally to be in good health (broadly put).  I realized i wasn't happy because I had forgoten about this. I was nervous about becoming a sedentary and not living an active life, a vibrant life. What was motivating my actions? Well, it wasn't the foundation of what I believe society should be based on, which is people's health. 

I am also discovering more about scaling web applications. I've learned about Apache Spark, Hadoop, NGinx, Ec2, Elasticbean stalk, and docker. I don't understand all of this, but basically, there are two major things that need ot happen when scaling a website. The first is that traffic needs to be routed across different machines, and the second is that machines need to be able to communicate with each other. Autoscaling products like Elastic Beanstalk handle distributing the traffic, and then programs like Hadoop and Spark, and Elastic Search coordinate multiple processing nodes as if they were a single computer to process large amounts of data, for all sorts of purposes. Not really sure how that works, but it does. I think the fundamental idea is processing data like Tencent's 700 TB of daily data from WeChat (I think) requires some special datastructures...all of which is outside of the scope of frontend development where I am now entering the field of computers.  

## 12/30
I am becoming aware of two things - the first is my interest in computer security. It is more interesting to me than Artificial intelligence because I am not that excited about my work in AI (as I am only interested in it as it relates to music, which I don't exactly enjoy studying intellectually), and because there are many people very hard at work on AI who are far more accomplished than me...it seems that I am always doomed to be a generalist, being interested in many different things. Additionally, my very first work in computer programming as a young teenage was in computer security, so in a sense I am coming full circle to my original interest in computers. I think that is a good sign, and it also gives me a focus for companies during job search.  So, my decision is to refocus my energies back into Ruby on Rails and Javascript (what I learned in the first place). Rails IS indeed a scalable service, as Lumosity has pointed out, and my forays into Python have shown me something very interesting about all of that and the diversity of languages and frameworks out there. Fundamentally, however, my fluency is with Ruby and Javascript, so I should go hard into that and pursue my interests and apply to jobs using that stack. I think a good project would be to build another full stack application, put it on AWS, make it scalable as I was thinking with the previous project.  If I want to "go deeper", I can start to reverse engineer the Ruby language itself, and start applying my interests in security, as well as study the C code for Ruby, and start making an open source contribution to a project. I think that's a fine avenue for exploration while job hunting. I can also market those skills as a freelancer. I can definitely build websites with Ruby and Javascript into something really useful and powerful, so I will go back to that after having explored a while, which I am prone to do for some odd reason. 

The other things on my mind is greedy algorithms. Highest Product in O(n) time and HouseRobber in O(n) time are two example of greedy algorithms.  I have learned their strategies but am not 100% confident about how the strategies were arrived at.  Additionally, I have come to the conclusion that a trick for reaching an optimal solution is to consider what must minimally be done in order to solve a problem. Probably, that minimal time complexity is the optimal time complexity, if I know the correct strategy (greey algorithm in this case). 

Something I'd like to do next is load a Rack server on AWS, or load a rails application and connect it to a database and then load test it and see what happens. 

## 12/29
It's been a restful holiday season, and I am recommitting to job search in SF.  I came out here to change my life, and now I am going to finish what I started in the new year - get a job as a software engineer. I've made progress with my understanding of algorithms, and I've gained some topical knowledge in machine learning and put forth some effort into my music analysis application. Next steps in include building out the interface for Theorizer, and turning it into a fully functional SPA. This includes adding authentication so users can keep track of scores, score uploading, and a better neural network. The ultimate goal of this application is a fully functional music theory analysis program for users who want to make theoretical sense of this incredible wealth of piano music. The first step, however, is to simply get the score to sync with the keyboard.

Additionally, I have more work to do on the neural network. It needs to be able to tell chord type, along with chord name. I think this will require a table of output (Chord name, and then chord type, or simply a long list 11 pitches times 8, maj min, aug diminished, dom7, min7, maj/min 7, maj7).  I think it will also require a convolutional neural network. More on that later. 

Lastly, I am interested in the scaling project. 

Fundamentally, however, I need to get a job with a company that I really want to work for. So what am I going to do? 

## 12/15
1. I've been spending my time as a placements TA. I've seen a number of projects come to fruition, and that has been satisfying. These include a machine learning Django Application, as well as two full stack Ethereum Blockchain DApps. I've also acquired some familiarity with the MERN stack: Mongo, Express, React, Node. 

2. Today, I launched an AWS t2.micro instance, and connected with it through SSH. I used this tutorial: https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EC2_GetStarted.html?icmpid=docs_ec2_console, and followed a supplementary tutorial inside of it in order to set up some prerequisite things (a VPC and a Security GROUP).  Before you do this tutorial, be sure to sign up for AWS. 

3. When you connect to your t2.micro instance, in the cloud, you have to use SSH connection through the terminal. Once you're connected, it's just like being in terminal. And that's it. The next goal is to actually run something on it, and get information back, probably a simple or rack backend. 

4. Put a simple node js serve on it that returns 'hello world'. Used this tutorial after I launched the instance. https://hackernoon.com/tutorial-creating-and-managing-a-node-js-server-on-aws-part-1-d67367ac5171

5.


## 12/7
1. Man, I've been working hard with helping the students on their javascript projects. I'm learning about D3, more about asynchronicity in Javascript, and some really hard bugs, that I couldn't solve. 

## 12/6

1. Grading full stack projects.

## 12/5

1. I'm a placements TA now. I need to remember to keep committing something every day. 

2. Todays algorithm was rotateSquare(matrix): Rotate a square matrix 90 degrees, but in constant space. It's tough but it can be done!

## 12/1
1. It's December, and a lot has happened. I did a hackathon to learn solidity and ethereum, and I finally feel good about being a full-stack engineer. 
2. I also did an algorithm called call back throttler, a very hard question. 

## 11/26

1. Today I learned about super cookies, and how the allow a website to view all of your browser history between two visits to your website. This is very powerful! 


## 11/25

1. There is node package called https, it makes a request and then takes a callback. In order to read the body from the response, you have to set the `res.setEncoding('utf8')`, and use `res.on('data', (body) => {//do something});`, and this was something very new to me, because I had never used node. Should tell Alex about it. Check the docs for more info. 

## 11/24
1. Cursors are variables that store how many rows a SQL query has return thus far. It makes batched queries possible.
2. Connect postgresql to Django. YAY! Not that hard actually.

3. Websockets are some kind of connection to a server, but I'm not sure how they are different from regular server client relationships.

## 11/20
1. Studied the regular expressions, algorithm. It was SO beautiful!

## 11/16
1. Today I am going to code up a neural network. Yesterday, I watched Ned do it with the Enron data set, and today, I am going to do one myself, and then I am going use my own dataset using musical chords. My neural network will be able to distinguish chords. I will create my own training and validation set and test it, then I will put the whole thing on github for the world to see and hire me.  

  1. The first thing I have done is set up my environment using this tutorial: https://machinelearningmastery.com/setup-python-environment-machine-learning-deep-learning-anaconda/
  
  2. 

## 11/15
1. This morning, I have done some research into Neural Networks.  This research came out of yesterday's lectures in neural networks using forward and backward propagation, using logistical regression equations at each node. I probably butchered some of the wording there, but the gestault is that I watched Ned code up a neural network and it's was pretty cool. I want to learn this stuff, and do something interesting with it. One of the most interesting things I've seen in a long time. 

2. There are many kind of neural networks. Today I learned about LSTM neural network, that can handle long-term dependencies. ie. "I grew up in France...I speak fluent FRENCH," where is FRENCH is the accurately predicted word. This could also be applied ot music analysis where we're given I IV V ( . ), where () is replaced by 'I', the tonic chord. This is what always happens.  I miss music so much, and I'm not really sure what to do next with all of this tech out there. 

3. We also learned about Boolean functions, upone which I believe all of computing is based. Didn't know that. 

4. I have also started to explore vanilla Javascript implementations of MVC frameworks, upon learning how many JS libraries are in existence. I need to develop my vanilla JS more. 

5. Lastly, I have discovered the breadth of libraries and websites that help musicians work with music. There is SoundSlice, a musicXML renderer, there is ABJAD and Mingus, for manipulation of notes with Python, and there are a few PDF - MusicXML slices, but it seems that they are not too developed. MusicXML scores are not in abundance it seems, and when I transform Traumerei to MusicXML, most of the notes are there but the rhythm is not perfect.   Kenta suggested putting making the first step toward a better renderer by shifting midi files to more uniform rendering. 
 

## 11/14 
1. Topological Sort algorithm is beautiful.

## 11/13
1. The algorithm for finding the median of two sorted arrays is quite beautiful, if I could figure out how to do it with code.

## 11/12

1. Sometimes typos can happen in the most unexpected places. Today, I was working on some code, and I kept getting wrong outputs. I realized that I had written my test case incorrectly. So, actually, my code was working just fine, and it was the text input that was wrong. That was so frustrating! They always happen where you least expect it.


## 11/11

1. I have decided to channel my energies into the study of a personal challenge.  There is so much to learn in technology and there is way more to know than there is in a lifetime to learn. This is much like music, there is a enough music/tech for a lifetime, but not enough lifetime for music. And so, given my love for music, I can only continue to pursue the tech through my love of music, and as such, will put forth all of my non-job searching time into the study of a personal project related to music. This is very important to me for the sake of making a contribution to music in the best way that I can, in order for people to learn more about it and appreciate it through the aid of technology, which has already revoluntionized the way humans access information. 

2. The first things that I have discovered to day, is a partially beautiful rendition of the Girl with a Flaxen Hair, the midi file is done OKAY, and the score looks terrible when rendered from a free app that i discovered. 

3. I have discovered a number of music rendering services - lilypond, midi, VexTab, and some music notation applications in the browser. They all seem to do it a little bit different, and I do not know how to fit them to my purposes. 

4. Lastly, today I worked on SQL. Remember that HAVING is akin to making a WHERE statement, but after you have grouped the results. IT's like being picky about the groups you show, after you've grouped them.

## 11/10

1. I worked on a coding challenge from Ankissam. I won't share the solution here :).
2. I read about machine assembly language and Java. I read a solution in Java, and I think I want to learn Java, because I am interested in the backend of software engineering. Actually, I'm more interested in the machine language interface. Manipulating registers is like manipulating keys on a keyboard. 

## 11/9

1. I studied the algorithm for finding the longest substring without repeats. Use the hash to keep track of previous inputs, then, when you hit a repeat value. Move the left-point to the character past the first appearance of the number. Keep track of the distance between pointer1 and pointer2. I didn't get it work, and that was frustrating.  
2. I learned about heaps and quicksort in constant time. Two very important sorts.
3. I learned about Naive Bayes equation for sorting a dataset. We use Naive Bayes in conjunction with gradient descent to find the phi values such that the proability of the dataset is as high as possible.  Notes that this is not reinforcement learning, this was called supervised learning.
4. I also learned a bit about SQL, which is getting more and more interesting.


## 11/8
1. I used a linked-list today to perform arithmetic addition (not the most stimulating algorithm) in javascript.  I messed up the composite logic statement.  I said while (it is true that both are not null), while I meant to say (at least one is is not null), and that a was a very sublte point.
2. Additionally, I am moving into being interested in backend development. I really like that stuff, and I'm going to now push towards that goal by studying algorithms and data structures everyday, and also will be working on backend work, like Rails and Active Record lite, reviewing SQL, and building a project with more complex API on my project. 

3. Because I am interested in being a backend developer, I am now going to list all of the things that I think I am supposed to be able to do. I learned a number of things from talking with John, and listening to Ned's lectures, and now I'm am going to put them out here in an effort to organize myself for the next project. 
    1. The first theme I remember is that systems designers need to trade off two things. I forgot what those two things are.     2. I remember that a very important thing in distributed systems is how they actually distribute the system.. Sharding, load balancing, are two key words from this talk.   There are multiple ways to do it, and it comes down to the hardware.  
    3. Now, getting back to the full-stack. There are many ways to connect the API with the frontend. API's can be designed and organized in a number of ways. We've been using RESTful routes for CRUD functions, getting back JSON objects, and making SQL queries using a relational database. There is also GRAPHql, and Apollo, and Graph databases, and there are also NoSQL databases like MongoDB. I made my own little noSQL database with I Ching.  Interfaces like Graph QL and Elastic Search make it easier to get data and organize it. Relational databases have their strengths and weaknesses too, but I"m not sure what they are. 
    4. The backend is more-or-less composed of the API/Router, the Controller, and the Database. The MVC is one way to understand this linkage.  I think this very cool and interesting.
    5. There are some things that I need to learn
            1. How to prevent hackers to getting at my information.
            2. How to use AWS to host a database.
            4. How to use different kinds of databases and frameworks (Express/Mongo, Django, LAMP, GRAND) and perhaps use them. 
            5. Understand a query language, lIke Elastic Search. 
            5. Understand scaling an application in production.
    6. understand other API paradigms( "whatever-works", RPC, hyper-media, and query-based), but it seems to me that there's really only RESTful, whatever-works, and query-based.
    7. I should go to some SQL meetups and backend stuff, and talk with DIllon's friend.
    8. The TOR browser is about security, and that is also interesting to me. Working in cyber security could be cool. 
    9. So where do I start? Algorithsm, fundamentals, and then start a project. 
    10. Keep reading about things that are of interest. And find a meet up or group to keep discussing things.

    11. My studies in SQL have taken me into the realm of nested queries. Apparently you can use the ALL statement to find rows that are related to all of the other rows in some way. Very interesting. 
    
## 11/7
1. Today, I had a lot of conversations.  I'm feeling conflicted about how to structure my time, and am I don't know what really excites me about software development. I want to start my next project and apply to backend positions using SQL and the backend Framework, but it seems that I have prepared more for the front end roles. Yet, I'm more excited about seeing the backend be put together. So I need to figure out how to structure my time. 
2. Also, I miss playing the piano and I wish I could just play the piano and share that with the world and have a community of musicians to be around. That would be the best thing ever. How can I do that? I need to learn back end development. 

## 11/6

1. Leetcode solutions are very intereseting.  Move O(n^2) to O(n) by using a hashmap in the Two Sum solutions, and then do something clever. 

## 11/3

1. Last night, I wrote a test that one of my async actions called the correct action-creator. We learned that .fail() is part of Ajax and .catch is part of Promise. My async action did indeed call the correct action creator, but Jest, the testing framework, would not recognize the .fail() portion, so I had to change it .catch(). The problem is that I used .fail() in all of my async actions, and switching it to breaks the functionality (at least in login()), so, basically, this test is not going do it's job. 

## 11/2 
1. Today begins my investigation into classification of pitches and ways to detect patterns from sets of them. The first task to generate random sets of intervals and extract out the intervals that exist.  
2. This repo is staying for the secret of potentially using this information to make money, but I will share the general situation here. The goal is to use machine learning to analyze musical information. The end result is that users can better understand musical scores and not be intimidated by their complexity.  
3. I build a random musical interval generator and a short program to extract the intervals. The intervals are generated randomly, but it may not necessarily be true in a musical compositions. There in fact may be many of intervals, and they will be organized hierarchically, both by register.  I think that the idea behind DAC (from switzerland) is that the computer was fed information (in the form of melodies), and they simply detected the patterns between the pitches, and then created one usein the statistical information regarding information about which pitch would come next. My goal is to feed the computer information, and then have it say something relevant about the piece using the language of music theory.  
4. One other idea on my mind is for the use to be able to select notes and for the computer to say something useful about those notes. The user selects those notes, and then the computer takes a look at them (say no more than a measure or two), and the computer deciphers it. 

## 11/1 

1. Lilypond and Abjad are tools for producing and modifying musical scores. They seem quite powerful. Abjad can select portions of music and manipulate them. I need to discover if Abjad can evaluate portions of the musical text and say something userful about it. 

2. Javascript class syntax is very different between es5 and es6. 

## 10/31
0. Machine Learning lectures begin today. Learn how to find a linear regression.!
    1. Some notes on Python and matlib: The first is that some of these function take vectors, and we are performing vector addition. For example, if I set x_delta = (x_value- x0); return 1 + x_delta + b, I am actually returning an array of points, despites the fact that it is not explicitly written in array form. This, I believe is vector addition. 

1. Word Chains is a very interesting problem involving a hash and iterative process for traversing a dictionary.
2. Spiral Print is a way to print the values of a square in a spiral order. Remember to use pop and shift-like methods to make your life easier. There is an elegant way and a non-elegant way to do things!

## 10/28

1. Remember that closures pass values by reference, not by value. The solution is to use Immediately Invoked Function Expressions. 

## 10/27

1. Nan means that the value of a variable does not fit into the IEEE stand for representing numbers.
2. Hoisting is a special quality in Javascript. 

## 10/25

1. Dynamic Programming is hard.  
2. 'this': In javascript, 'this' is the object in which the function is being called. It's a lot like 'self' in ruby, and it can be changed and manipulated with binding. By default, 'this' is the window. 
3. Goal: Load react on my django frontend with out using create-react-app, just use webpack and install the dependencies using npm.
4. Lesson: When a Django view loads assets, it needs to be told where to find them in the project's settings.py. This is how a react page can find the bundle.js file when using webpack.

## 10/24
1. Follow the transloadit tutorial to upload a file to S3 bucket. Goals:
  1. Hide the S3 bucket information.
  2. Display uploaded waveforms through react.
  3. Upload through React. 

## 10/23

1. Flex-end: Start at the end of the main axis;
2. Align-self: aligns a single item in a flexbox.
3. +x: One of three annotations on a variables for the number of coercion to a specific number.
4. NGINX: A server application, like Apache or Puma.
5. Immutable Data Structures: A new way of storing information is such a way that the data structure is not rebuilt everytime    in new memory - the goal is the make apps run faster. 
6. How to optimize delivery of static assets: Bust cachining with query versioning, use a CDN (if everyone is around the world), or minify your files (using a plugin, not manually)
7. In Ruby, nil can be compared with strings.

8. Graphs are interesting.
9. Please help me put waveforms into Piano Cloud.

## 10/22: 
1. Built a React skeleton. Need to memorize webpack config file. 
2. IDE - Integrated Development Env.
3. JVM - Java Virtual Machine

## Previously 

10/17:
Today I studied Linked Lists, and yesterday (10/16) I studied Dynamic Arrays. 

10/18:
Today, I studied Heap Sort.

10/19
Today I studied 
  1.  Contest versus Scope: 
  
  Context is object dependent, while scope is function dependent. For example, this.variable is calling a variable in the context of a specific object (which could be the window). Scope determines what variables a function can access (which can vary depending on the kind of function defined in Javascript.)
  
  2. What is the event loop?
  
  The event loop allows Javascript to make asynchronous calls. When an async call is made, it is processed in a separate thread, and only when it returns is it placed in to the queue to be processed.
  
  3. Bind vs Call vs Apply? 
  
  All three are ways of binding the context of the function so that it can be called in another context. Using Bind returns a new function that can be called with the arguments requiredd by the bound function. Call and Apply return the function immediately within the context described, the difference is in how arguments are passed. Call uses splat and Apply uses an array. 
  
  4. Binary Search Trees and QuickSort in O(n) space. 
  
 
