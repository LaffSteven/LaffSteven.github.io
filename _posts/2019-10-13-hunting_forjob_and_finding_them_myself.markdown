---
layout: post
title:      "Hunting for Jobs and Finding Them Myself!"
date:       2019-10-13 22:41:37 -0400
permalink:  hunting_forjob_and_finding_them_myself
---


I just spent the last week learning to scrape websites for data in an effort to build a job-hunting program. Sample assignments and code-alongs are a good starting point, but the real learning seems to start when you start building programs for yourself. I decided that my first solo project should be something that I might actually use later on. Pulling a list of software jobs from Craigslist might e a good thing to do, seeing as how I’m doing this software engineering boot-camp.

That decision takes care of the first step: What? But the trick coming up was going to be the “How?”.
Well, luckily, some very smart people have built some very cool tools that let us pull data from the HTML code of websites. Craigslist in this case, which leads to a new problem… How do I navigate the HTML of a real-life website? What unforeseen challenges await in the CSS? Wait...how will someone actually use this program? Lets do that first.

First thing is first, I had to build the interface. Using a command line interface, I get the the desired search area with a zip code and search distance. These get put into a custom url that conforms to the websites search parameters. This produces a list of jobs. Nice! But here comes the hard part. Breaking down the page to get the container that hold those results. The target in this case, was the link in each item that would take me to the full page for each job. This was something I hadn’t done before; pulling each individual list item out of an unordered list. No indexes, no id value, just the "list item" tag to start me off. It took me longer than it should of, and I should have asked for help, but I got it figured out. Once the links to the pages were sorted out, scraping the desired attributes from the job pages was just some trial and error in using the Nokogiri functions.

But hey, perseverance paid off, and here is some proof, a short video of showing off and doing a little work on the program.
[https://youtu.be/SLqtqunFb7o](http://)
