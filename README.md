# study_progress
What I have studied since Oct 18th, 2017. Most recent additions are first.

## 11/2 
1. Today begins my investigation into classification of pitches and ways to detect patterns from them. 

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
  
 
