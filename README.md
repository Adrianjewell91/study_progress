# study_progress
What I have studied since Oct 18th, 2017. Most recent additions are first.

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
  
 
