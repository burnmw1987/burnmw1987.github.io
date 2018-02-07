---
layout: post
title: My first project - The start of the Utilities Collection
---

My first post, about my first project, and my first dive in to C#. As part of my daily role I have been writing some OpenEdge test classes. Unfortunately, the built in test unit runner wasn't working properly - sometimes it would correctly display the results of the run; and other times it wouldn't. This gave me a start point for my first C# project - write a small utility to read in the standard XML output from the unit test and display the results in a sensible, usable and reliable form.

And so the Utilities Collection was born!

The code itself is a mish-mash of things that I've pulled together, and I'm still working out how and why some parts work how they do - but it's a start. It can be found on my GitHub [here](https://github.com/burnmw1987/UtilitiesCollection) should you wish to have a peek in to it.

It allows for an XML file to be read in from a user defined location (it also then watches the file and reloads it whenever it is updated):

![Utilities Collection - Opening screen]({{ site.baseurl }}/images/UtilitiesCollection_Initial.png)

It then analyses the file and displays the XML in a user friendly and colour coded fashion:

![Utilities Collection - First Display]({{ site.baseurl }}/images/UtilitiesCollection_FirstDisplay.png)

Any test failures that have occurred can be selected to view the associated stack trace:

![Utilities Collection - Failure]({{ site.baseurl }}/images/UtilitiesCollection_Failure.png)

Any test errors can also be selected to view the associated stack trace:

![Utilities Collection - Error]({{ site.baseurl }}/images/UtilitiesCollection_Error.png)

It's still a bit of a work in progress, so I may come back to it in the future, but for now it fulfills the original brief and is more reliable than the built in test runner.

Some possible future enhancements could be:

* Display total number of tests run, tests failed and tests errored
* Store location of last used XML file
* Be expanded to accept different types of Unit test output
