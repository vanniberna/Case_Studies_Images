# SingulierPluriel Case Study

![Screenshot from an LMS](https://raw.githubusercontent.com/vanniberna/Case_Studies_Images/main/SingPlur/lms_logo.png)

## Context

In many universities and educational settings, course instructors use *learning management systems* (henceforth LMS) to share materials with their students, communicate with them, and grade their assignments and exams. Some of the popular LMS currently in use in many institutions include — to name a few — **Blackboard**, **Moodle** and **Canvas**. Having been active as lecturer and language instructor in academic and adult-education contexts for multiple years now, I have used LMS regularly and became very acquainted with the ins-and-outs of their functioning as well as with their potential drawbacks. 

## Problem


Something I quickly noticed from the early days of my academic teaching is that many LMS are by now fairly old and present counterintuitive UIs with too many redundant categories and an unclear navigation experience. 

Just to give you an idea, the UI of a very widespread LMS I use in one of the universities where I teach looks like this:

![Screenshot from an LMS](https://raw.githubusercontent.com/vanniberna/Case_Studies_Images/main/SingPlur/bb.PNG)

Aside from the glut of ambiguosly labelled sections and elements (what is the difference between the "Announcemets" section and the "Dashboard"? In the "Build Content" dropdown menu, how can I know what differentiates a "File" from an "Item"?), there is also an issue in terms of information architecture. As a course instructor, one of the actions I perform most frequently in the LMS is uploading lesson materials for my students. Yet, in the LMS pictured above, I have to go through four steps in order to do so from the home page (Home Page > Courses > Semester > Learning Materials > Course), which tends to confuse a new user and slow down even habitual ones like me.
 
Being conscious of such issues with this type of tools, I deciced to pitch the creation of an LMS as a project to undertake during the UX curriculum at TechLabs Berlin, which I attended from November 2023 and April 2024. My pitch got accepted by the program leads, and I was soon joined by other attendees of the program who were taking the web development or the data science curricula. Thus, a team of 8 (4 webdev people, 2 data science people, me as UX designer, plus a mentor) was formed. We had little more that 2 months to create a first MPV of the LMS.

## Goal

With SingulierPluriel LMS, we wanted to create an LMS that trims superfluous categories, allows for speedy navigation and flow, assists users in performing their tasks quickly and efficiently, and allows course instructors to visualise important info on their courses graphically and intuitively. 

## Process 

I set out  to employ user research, competitor analysis, and user testing to prepare a prototype that would significantly reduce the quantities available in the LMS to grant for a more transparent information architecture and a speedier execution of habitual tasks like contacting students, uploading and editing course materials, or grading assignments. Given the limited amount of time we had for the project, my team also asked me to use my Figma prototype as a showcase to visualise functions that the web devs and the data science people did not have time to code in their prototype app, which was more focused on the use case of visiting the Course Page to create and edit modules with course materials.

## Results and deliverables

An interactive high-fidelity wireframe prototype that addresses the problems encountered in user research and in the competitor analysis.

## Status
Finished. After a battery of user testing, relevant and feasible feedback was implented into the prototype.

***. . .*** 

## Intro

![Screenshot from an LMS](https://raw.githubusercontent.com/vanniberna/Case_Studies_Images/main/SingPlur/worried_students.jpg)

*Ciao profesore, hope u are doing well, sry but i cannot find the assignment for Monday online can u pls send it to me? Gracie, M.C.*

This e-mail — in all the glory of its multilingual misspellings and grammar mistakes — has blessed me many times, in multiple incarnation, during my career as a lecturer and language teachers.

The details may vary, but the scenario is always the same: the student logs into our university's LMS and — if they have already gone through the conundrum of enrolling into the right course in the first place — spends minutes on end struggling to find lesson materials / assignment / exam info etc. ... most common end-result: student gets frustrated, writes me an e-mail, and I end up moonlighting as (unpaid) LMS tech support.

So I started wondering: How could we create an LMS tool that circumvents these problems? Enter **SingulierPluriel LMS**... 

## Research

I began by performing a thorough competitor analysis, reviewing a variety of existing LMS. As I said, I was already familiar with some of those due to my job as a course instructor in universities and language schools, but I also examined further examples from the competition (Blackboard, Canvas, Google Classroom…). Aside from registering the problems that were already addressed here (ambiguous labeling, unclear functions and sections, cumbersome IA etc.), I also took note of the things that did work in the competition, e.g. the prominent presence of a help function in Canvas or the agile UI of Google Classroom.

I then set out to poll course instructors and students regarding their experience with existing LMS via Google Surveys that I distributed in his network of colleagues and students. Student turnout was — somewhat surprisingly — much higher than the course instructor’s (30 respondents vs 9 respondents). The student surveys were also somewhat puzzling because an overall good rate of satisfaction with the existing LMS (Blackboard, in this case) was contradicted by a flurry of criticism in the sections that allowed for open comment. Both the student and teacher surveys, anyway, confirmed the pain points that I had established in the competitive benchmark, and also offered precious insight into the desiderata that the users had: aside from clearer and snappier navigation, many users wished (amongst other things) for a more modern and intuitive design, quicker upload of course materials, and the possibility to visualize an image preview for the materials they had uploaded.

Based on these responses, I then generated three distinct user persona — 2 for course instructors, 1 for a student user. The two course instructor personas differed in age and tech capabilities, which also meant that they had different goals with the LMS (the less tech-savvy one just wanted to use it as a directory for course materials, the more technically versed one wanted to use it to have an interesting digital extension to their classroom environment). I accordingly generated scenarios and user stories to match these personas.

![Screenshot from an LMS](https://raw.githubusercontent.com/vanniberna/Case_Studies_Images/main/SingPlur/Maxine_Persona.PNG)

![Screenshot from an LMS](https://raw.githubusercontent.com/vanniberna/Case_Studies_Images/main/SingPlur/Loredano_Persona.PNG)

![Screenshot from an LMS](https://raw.githubusercontent.com/vanniberna/Case_Studies_Images/main/SingPlur/Josephine_Persona.PNG)

Finally, I set out to boil down the categories of the SingulierPluriel LMS to 4 possible sections (Courses, Communication, Announcements, Grades Center) and to conduct card-sorting interviews using a tool called Optimal Workshop. Users were asked to place a variety of possible tasks connected to the LMS (e.g. upload an assignment, schedule an exam etc.) into those 4 categories.

![Screenshot from an LMS](https://raw.githubusercontent.com/vanniberna/Case_Studies_Images/main/SingPlur/Card_Sorting.PNG)

One important insight garnered from these card-sorting interviews was that the split between Communication and Announcements tended to create the most confusion, so I decided to fuse them into a single section.

## Designing SingulierPluriel LMS

I thus proceeded to generate a user flow for the main user we had in mind as a team (the course instructor) performing a very mundane action inside of an LMS: creating a module in which to upload course materials.

![Screenshot from an LMS](https://raw.githubusercontent.com/vanniberna/Case_Studies_Images/main/SingPlur/user_flow.png)

User flows like this helped me in kickstarting the design process. During the early phases of designing the app, one major gripe was settling on a common UI library with WD, so that the components generated by UX in Figma would be easily consumable by developers. We settled on Chakra UI, and we did some testing by creating some samples and passing them back and forth between UX and WD in order to see how we could work together with the Chakra component library.

![Screenshot from an LMS](https://raw.githubusercontent.com/vanniberna/Case_Studies_Images/main/SingPlur/chakra_stuff.PNG)


… all of this testing did not necessarily prepare us for all the roadblocks that WD would face while trying to recreate the UI on their end, but it did speed things up a bit and through the Chakra plugin for Figma I found out I could also generate some CSS code with info about color, width, height etc. that could be useful for the devs.

## Prototyping 

![Screenshot from an LMS](https://raw.githubusercontent.com/vanniberna/Case_Studies_Images/main/SingPlur/finalprot_imago.PNG)

Anyway, through the design journey, we managed to go from the very first (admittedly appaling) hand-drawn wireframe sketches (which I will here withhold for the benefit of your pupils!) to low- and mid-fidelity wireframes and and lastly - after creating a proper stylesheet, making some graphical adjustments, and making sure that colour contrast was more accessibility-friendly — I put together a high-fidelity Figma prototype, taking into account my team's and mentor's feedback.

![Screenshot from an LMS](https://raw.githubusercontent.com/vanniberna/Case_Studies_Images/main/SingPlur/prototype_imago.PNG)

Here you can see our prototype in action - including a dynamic help function that allows one to take a journey through the functionalities of each page. Please note that the Figma prototype only includes the Course Instructor side, whereas the app developed by WD has two main roles, Course Instructor and Student.

METTERE VIDEO

You can also test our high-fidelity Figma prototype [here](https://www.figma.com/proto/dfZykUktjrsipShxE2xHRv/Screwaround-File?type=design&node-id=1162-1904&t=eArMoH8ZFlA4ilZs-1&scaling=scale-down&page-id=1153%3A1903&starting-point-node-id=1162%3A1904&hotspot-hints=0&mode=design).


### User Testing
<p align="center"><img src="./UX/Blogpost_Images/img_12.PNG"></p>

Lastly, UX administered a battery of user tests, asking potential users (all of whom are professionally active as lecturers or teachers) to perform tasks inside of the high-fidelity prototype while thinking aloud about what they were doing. These interviews have already provided a variety of alleyways we could take moving forward, e.g. streamlining things like the close buttons across the app to allow for more internal UI coherence; creating a skippable tutorial that opens up the first time a user logs into the LMS; offering an easy language option / accessibility mode with more visual cues, etc.

But most users showed a lot of enthusiasm and interest, remarking that SingulierPluriel seems way more accessible and immediate than what they are used to. They were also quite interested into the graphical dashboard functionality allowing to visualise data about a course (student attendance, performance, feedback etc.), which was the DS contribution to our project.

### UX Tech Stack
Figma for designing, Chakra UI kit to obtain ready-made components that are easily consumable by WD (though these components had to be largely modified by me to be of any use or interest at all…), Optimal Workshop for conducting card sorting interviews, Typescale for scaling fonts and typefaces.

https://uxdesign.cc/applying-ux-research-to-a-small-e-commerce-website-a-case-study-89e4b6a1cd2f