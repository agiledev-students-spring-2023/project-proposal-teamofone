# Project Proposal

## Project title

Albert Registration Assistant

## What and why?

As NYU students, we all use Albert for course registration. However, we may also need to search up additional information like what’s the professor’s rating/comments from previous semesters and which course fulfill major/minor/core requirement to be able to make our decisions. Also we will encounter situations where we have time conflicts between courses and the shopping cart on Albert does not allow us to pre-assign a ranking of preference for the course we selected to enroll.

In order to solve the problems addressed above, I plan to build is an auxiliary system which can provide additional and organized information on courses (e.g. course prerequisite, major/minor/core fulfillments, professor ratings, etc.) to assist NYU students in planning their course registration on Albert. This software system will serve as a pre-planning page for NYU students to organize their course plans with all the useful information at hand. It will save users the time to go over all the webpages searching for course information (Albert), professor comments/ratings (NYU Rate my professor), course fulfillment (major bulletin), etc.. Moreover, this system will also allow users to visualize their course calendar so as to check whether there will be any time conflicts. Last but not the least, the system will allow users to create multiple personalized course plans and rank them based on the user’s preference so that they won’t hesitate over which course to choose as substitution when their first-choice is no longer available.

## For whom?

This software will be tailored for NYU students who use Albert for course registration but find it not convenient enough for course planning.

## How?

Like Albert, this system will have a search page where the users can search for courses by keywords. As the course search result, the system will display a list of available courses in the chosen semester with the following information provided:
1. course number, course title (e.g. CSCI-UA 201 Computer Systems Org)
2. graded by which college/department (e.g. CAS Graded)
3. professor & rating, keywords from comments (e.g. “clear grading criteria”, “participation matters”, etc.)
4. Course schedule + location (e.g. Mon, Wed 9.30 AM - 10.45 AM at CIWW 101)
5. Course prerequisites (e.g. CSCI-UA 102 WITH A GRADE OF C OR BETTER)
6. Course fulfillment (e.g. CS major Core Requirements)
7. Total credits (e.g. 4 credits)

**Note:**
1. All course information above can be found on Albert except for feature (3) and (6). However, due to different capitalization and formatting, some of the information are not clearly visible on the Albert page.
2. Feature (4) course schedule (if chosen) will be reflected on the user’s personalized calendar page at its corresponding time block.
3. Feature (3) on professor rating&comments will also provide a hyperlink to link to the corresponding page of this professor on NYU Rate my Professor website with more detailed comments.

Like Albert, the system will allow users to select courses into their “shopping cart”. And by clicking on each course in the shopping cart, the detailed information about this course will reappear for the user to review.

Then on the personal page, the system will allow users to create their own course plans by dragging a course from their shopping cart and then drop it onto their course calendar. It will also allow users to create multiple course plans and give them a ranking order based on preference.

## Scope

The building of the described system will include 4 steps in general:
1. Retrieve data from the following platforms (requires web scraping technique or through this [Course System API] (https://anypoint.mulesoft.com/exchange/portals/nyu-0/aa8378b5-ce36-4c80-94a1-2e6042908e1a.central-it/course-sys-api/) offered by NYU)
    1. Albert
    2. NYU Rate my professor
    3. NYU major bulletin
2. Pre-data processing & build databases for the courses
3. Construct the user interface
4. Connect frontend to backend
Time can be allocated for programmers to learn necessary techniques and follow the above 4 steps to build the software.
The work of retrieving and preprocessing data and building pages/functions of the software can be done simultaneously and distributed among 4-6 programmers based on their areas of expertise.