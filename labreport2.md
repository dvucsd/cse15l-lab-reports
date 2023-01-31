# Week 2 Lab Report

**Part 1**

<img width="489" alt="image" src="https://user-images.githubusercontent.com/122562133/215589039-17a46749-aa2b-49dc-925a-d3da0b7741d1.png">


<img width="546" alt="image" src="https://user-images.githubusercontent.com/122562133/215588788-04344dbb-e97d-4b5a-9e50-db1fe6513054.png">
The method handleRequest is called in both screenshots.
The argument takes in the url and processes it to obtain the path. The path specifies the message that is being inputted by the user,
which is then stored in parameters. So the value is 'Hello' and 'How are you' for the screenshots respectively. Then, this is concatenated to the string s.
We have an empty string initially, so in the first screenshot, s is 'Hello', but 'How are you' is added on a new line in the second screenshot. 

<img width="607" alt="image" src="https://user-images.githubusercontent.com/122562133/215588875-d6b05f79-bd69-4844-98de-63287becaa2a.png">

---
**Part 2**

In lab 3, the buggy program ArrayExamples has a method called reversed which is described to "returns a new array with all the elements of the input array in reversed
order".

This is a test I ran which does induce a failure:

`@Test` \
 `public void testReversed2() {` \
   `int[] input1 = {3, 2, 1};` \
   `assertArrayEquals(new int[]{ 1, 2, 3}, ArrayExamples.reversed(input1));`
 `}` 

The input is {3,2,1} and the expected output is {1,2,3}, however the program returns {0,0,0}

---
This is a test I ran which is successful:

`@Test` \
 `public void testReversed2() {` \
   `int[] input1 = {0, 0, 0};` \
   `assertArrayEquals(new int[]{ 1, 2, 3}, ArrayExamples.reversed(input1));`
 `}` 

The input is {0,0,0} and the expected output is {0,0,0}, however the program returns {0,0,0}

---
Screenshot of failing test in terminal: \
<img width="633" alt="image" src="https://user-images.githubusercontent.com/122562133/215584333-455650a8-f5dc-48af-a5f6-f836c5215efa.png">

Screenshot of successful test in terminal: 

<img width="923" alt="image" src="https://user-images.githubusercontent.com/122562133/215584822-6cae3b2c-b50e-45ec-b3e3-2051fe53cfcd.png">

---
This is the original buggy code:

`static int[] reversed(int[] arr) {` \
    `int [] newArray = new int[arr.length]; ` \
    `for(int i = 0; i < arr.length; i += 1) { ` \
        `arr[i] = newArray[arr.length - i - 1];` \
    `}`\
     `return arr;`\
`}`

Here is the updated code that works:

`static int[] reversed(int[] arr) {` \
    `int [] newArray = new int[arr.length]; ` \
    `for(int i = 0; i < arr.length; i += 1) { ` \
        `newArray[i] = arr[arr.length - i - 1];` \
    `}`\
     `return newArray;`\
`}`

Previously, the code was buggy as each individual element in the original array was being assigned as elements from the newArray, which was initialised to 0. 
So therefore by returning arr, it would return an array of original length of all 0s. I have fixed this by making the newArray be assigned the index of arr.length - i - 1
from arr,and returning the newArray, which would return the correct, reversed output.

---
**Part 3**

One new thing that I learnt in lab 2 is the basics of how to process a url and start a web server on a local machine. I also learnt how to interact with it 
by adding characters in the path, which would create changes on the page.

