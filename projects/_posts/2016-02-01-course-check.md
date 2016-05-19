---
title: "Course Check"
subtitle: "A small desktop app that assists professors transitioning learning managment systems"
layout: post
categories: projects
tag: Product & UI Design
permalink: /projects/course-check
---

What happens when a proof-of-concept prototype becomes as useful as working software? 

# My Role

A squad of us at <a href="http://collectivelymade.com" target="_blank">the collective</a> assembled again to assist the University in designing a quick and effective solution to ensure a smooth transition of learning managment systems. I was in charge of translating the abstract goals into concrete solutions. I took part in problem identification, architecting the end-product, designing the interface, and implementing the public facing code.

# The Challenge

The ITS department is planning to undergo a university-wide transition from blackboard to canvas LMS. During the transition, ITS wants to try to downsize the amount of storage that each course uses up. To do this, they set limits on file sizes and identified other file types that would either take up excessive space, or cause file corruption when opening in the new LMS.

# The Discovery

#### The app doesn't need to download anything

Most of our background has been in web-based technology so initial ideas were: set up a site professors could upload their course files to and the system would respond by listing the problem files. Course files can be very large sometimes, which meant uploading several gigabytes could be a very problematic experience. We also questioned the availability of server space we would have access to, again, given how large these files can get and how many faculty members are going to be checking their courses. 

Insights from our discovery work indicated many areas where a web-based solution was rather inelegant and created more issues than it solved.

During this investigation phase, we were writing and testing scripts that could run through a course file and flag certain file types/file names. We were running these scripts locally on an example file, which led us to a conclusion: If we made this into a Desktop app, there would be no need to download anything, we just needed the user to identify the file they wanted the system to check. 

Enter <a href="electron.atom.io" target="_blank">electron</a>; A way in which we could make a cross platform desktop application using the web technologies we were already proficent in. An app that ran locally on the user's machine removed the unknowns we were having about users' internet connectivity. It also saved us from having to ensure the app would work on (almost) every modern web-browser (some professors are still on IE 6 😭). 


# The Solution

<img src="/img/work/CourseCheck.png" />

We built CourseCheck. It's a tiny electron app that can live on a user's desktop. You download your course file from blackboard and use the app to identify the course file on your machine. The app identifies the issues and presents the user with the file name, location, and potential problems they may have when transitioning to canvas. Instructors use this tool to make edits to their files to ensure a smooth and painless transition to the new system.

<img src="/img/work/CourseCheck2.png" />

# The Impact

CourseCheck is fast. A majority of the scans take less than one second. 

Development was fast & cheap. We built this within a standard dev-cycle which kept costs low. The ITS department was able to get a solution they needed quickly without having to go through the tumultuous process of board bureaucracy & descision making.

CourseCheck is modualar. We tried to make the app as foundational as possible so that in the coming months when more departments start switching over, features like automation can be added to the app.
