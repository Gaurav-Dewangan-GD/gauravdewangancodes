---
title: "Find out GCD of Two numbers"
date: 2022-11-27T19:13:50+05:30
author: "Gaurav Dewangan"
draft: false
---

<!-- # Finding out the GCD of two numbers -->
---
The greatest common decimal(GCD) or highest common factor(HCF) of two numbers can be calculated as the highest common factor found in the factor list of the given numbers. The result found can also divide both numbers perfectly. In programming languages, several steps are constructed to implement this logic in various ways and some of them are listed down below.

Traditional Way:

For example,  let us take two numbers 12 and 18, the factor list for both numbers will look like these:
12 : [ 1,2,3,4,6,12]
18 : [1,2,3,6,9,18]

When we compare these two lists we can see some common elements appearing in both lists, like:

1,2,3,6

Among these, we found out that 6 is the largest value! i.e GCD of 12 and 18 is 6.

This approach can be implemented in a programming language by just following the above steps and creating an algorithm to implement it.

Naive Algorithm:
1. Find out factors of both the given element and store them in an array/list
1. Compare both the list and find out the common once
1. Store this element in a separate array/list
1. Print/return the largest value of that separate list


The python implementation of the fellow program will look like this:

<code>


Note. I have used a save_time variable to know the actual runtime of the program for further reference.

Although this approach will give us the correct result it will take a lot of time to run over large values and eventually also take up lots of memory space. We can optimize this approach a little further.

Since finding out factors means finding those elements that perfectly divide the given number say n and lie in its range(1 to n). So instead of running two loops, we can narrow it down to one loop. One more thing is that the loop should only run for a minimum of both the element present, as common factors can only be found till the least element value as seen in the above example.

Now we code it again but with modification and see the time taken also:

<code>


It takes eventually less time,but we have one problem that the common factor are stored always as a list and we only need the last element of the list. So instead of list we use a variable(python name) to assign the values. Therefore, the last value that will be reassigned to variable will be our answer.


<code>


See the code works a lot faster then earlier. But But But But!!! This operation can also can be optimized one step ahead to get the solution at an instant. Instead of running the loop in 0 to nth order we run the loop in reverse. Why? As the last element is our result so it will come first if we run the division/factor loop reverse. 

<code>


The code is optimized very well and is giving us the desired result

But programmer tend to use a better method then this because instead of using mathematics we are using properties of programming language and common logic to get our result.

To get a better approach read the below article


Hope You like this article about GCD of two numbers, if you have any feedback related to content discussed mail me anytime and if you want to contribute to this article for translation or corrections you can give me pull request in my github.

Thank You for reading, hope you learnt the whole concept well enough.

See you next time! Till then learn | understand | code 


