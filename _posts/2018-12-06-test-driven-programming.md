---
layout: post
title: Test Driven Programming
categories: Senior_Seminar
---
Several experienced programmers have emphasized the importance of test driven programming to me. I never understood the imporatnce of this ideaology until the last summer. I believed that code makes something new but tests only validate what has already been written. This was not a exciting especially because I had to work through the input to arrive at the output.

Test driven programming is very different from code that has been tested. The former is a way of writing software, it is a methodology while the latter is a necessary part of software development. Untested code can never be considered complete.

I found these rules [online](https://medium.freecodecamp.org/test-driven-development-what-it-is-and-what-it-is-not-41fa6bca02a2) that describe test driven programming very well:

  - *You are not allowed to write any production code unless it is to make a failing unit test pass.*
  -*You are not allowed to write any more of a unit test than is sufficient to fail; and compilation failures are failures.*
  - *You are not allowed to write any more production code than is sufficient to pass the one failing unit test.*

This can be simplified as:

- *Write only enough of a unit test to fail.*
- *Write only enough production code to make the failing unit test pass.*

So every functionality starts with code that would make the existing code fail (because it has not been implemented). These tests cover all the functionality of the code but the minimum number of tests to cover all the cases is write. After this phase, the smallest amount of code is written to pass these new test cases. FUnctionality is developed in this manner until the software is ready.

Teams benefit a lot from this methodology because the coder is not biased by their own work. It also helps save time by ensuring that the programmer actually understand the tasks and have though about them thoroughly. This also leads to good testing practices all while sacrificing a bit of dev times. In the long run. studies have indicated that time is actually saved because there are less bugs in the code and thus much less debigging
