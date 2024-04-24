# Club Hub

[Clubs At Manoa GitHub Organization](https://github.com/Clubs-At-Manoa)

## Table of contents

* [Overview](#overview)
* [Approach](#approach)
* [Use Case Ideas](#use-case-ideas)
* [Beyond The Basics](#beyond-the-basics)
* [Deployment](#deployment)
* [Milestone1](#milestone-1-mockup-development)
* [Mockups](#mockups)
* [Milestone2](#milestone-2-functional-development)
* [Milestone3](#milestone-3-final-project) 

## Overview

The problem: UH Manoa has over 200 Registered Independent Organizations, plus many more that do not have this “official” status but are nonetheless active organizations. Unfortunately, there is no easy way for students to learn (a) what student clubs (both registered and unregistered) exist, what they do, and how to get further involved.

The solution: The Club Hub application will provide a centralized directory for UH Manoa student clubs. UH Manoa students can login to browse a well organized directory of all current student clubs, with brief descriptions, meeting times and locations, URLs to their websites (if any), contact information for officers, and a few select photos.

* Three primary collections (Profiles, Projects, Interests) as well as three "join" Collections (ProfilesInterests, ProfilesProjects, and ProjectsInterests) that implement many-to-many relationships between them.
* Top-level index pages (Profiles, Interests, and Projects) that show how to manipulate these six collections in various ways.
* Initialization code to define default Profiles, Interests, and Projects and relations between them.
* A simple Filter page to illustrate how to perform simple queries on the database and display the results.
* Use of Meteor Methods to illustrate how to simplify implementation of multiple collection updates.
* Use of indexes to enforce uniqueness of certain fields in the collections, enabling them to serve as primary keys.
* Authentication using the built-in Meteor accounts package along with Sign Up and Sign In pages.
* Authorization examples: certain pages are public (Profiles, Projects, Interests), while other pages require login (AddProject, Filter).
* Use of Meteor Assets to initialize the database (helpful when initialization exceeds settings file size limits).

### Approach

Club Hub has three user roles, all of whom login with their UH ID. Regular users browse the directory. Club Admins have the ability to edit the data associated with their club. Super Admins make sure site content is appropriate and grant “club admin” privileges to selected users.

The site should not simply support browsing by a list of clubs in alphabetical order, but should also allow filtering by interest area. For example, “athletic” clubs, “art” clubs, “music” clubs, etc. A club can belong to multiple interest areas.

Users can specify interest areas, and be notified when a new club is created matching that interest area (or an existing club adds that interest area).

Admins can monitor the site for inappropriate content, and create new categories of musical tastes, capabilities, and goals.

Note: if you choose this idea for your final project, you cannot name it “Club Hub”. Come up with a different name for your final project.

Some possible mockup pages include:

* Landing Page
* User home page
* Admin home page
* Club admin home page
* Browse clubs by interest area(s)

### Use case ideas

Whether the following bullet points list all pages or not, the completed use case should show an end-to-end scenario of using the system.

* New user goes to landing page, logs in, gets home page, sets up profile. (How do they learn how system works?)
* Admin goes to landing page, logs in, gets home page, edits site.
* User goes to landing page, logs in, looks for clubs of interest.
* Club admin goes into site, updates their club profile.

### Beyond the basics

After implementing the basic functionality, here are ideas for more advanced features:

* Upload club data from the CSV version of the RIO spreadsheet.
* Notify admins when club data changes, so they can review for appropriateness.
* Provide “expiration date” for club listings (either one semester or one academic year). To retain a listing, the club admin or admin must login and click a “renew” button for the club to re-list it in the site.
* Allow students to rate clubs.

### Deployment

[Clubs At Manoa deployed application via Digital Ocean](http://146.190.35.7/)

### Milestone 1: Mockup development

The goal for Milestone 1 is to get our project up and running.

Our TODOs include:

* Add a link to our Team Contract
* Deploying our system to digital ocean
* Create a landing page
* Create a login area on the landing page
* Create a mockup for the user home page
* Create a mockup for the admin home page
* Create a mockup for the club admin home page
* Create a mockup of page to browse clubs by interest area(s)

Milestone 1 was managed using [Clubs At Manoa GitHub Project Board M1](https://github.com/orgs/Clubs-At-Manoa/projects/2/views/1)

### Mockups
<div class="text-center p-4">
  <img width="500px" 
       src="app/public/images/Mockup_D_Landing.png" 
       class="img-thumbnail" >
  <img width="500px" 
       src="app/public/images/Mockup_Landing.png" 
       class="img-thumbnail" >
  <img width="500px" 
       src="app/public/images/Mockup_Login.png" 
       class="img-thumbnail" >
  <img width="500px" 
       src="app/public/images/Mockup_Register.png" 
       class="img-thumbnail" >
  <img width="500px" 
       src="app/public/images/Mockup_D_NewUser.png" 
       class="img-thumbnail" >
  <img width="500px" 
       src="app/public/images/Mockuo_D_User.png" 
       class="img-thumbnail" >
  <img width="500px" 
       src="app/public/images/Mockup_D_Admin.png" 
       class="img-thumbnail" >
  <img width="500px" 
       src="app/public/images/Mockup_interest.webp" 
       class="img-thumbnail" >
</div>

### Milestone 2: Functional development

Our TODOs include:
* Significantly improve the functionality and quality of application beyond M1.
* Significantly improve software engineering process beyond M1.
* Four pages in addition to the Landing page should be available in the deployment.
* At least one page in the deployment should read data from the database (i.e. from MiniMongo).
* At least one page in the deployment should write data to the database (i.e. using a form).

Milestone 2 was managed using [Clubs At Manoa GitHub Project Board M2](https://github.com/orgs/Clubs-At-Manoa/projects/3/views/1)

### Milestone 3: Final project

Our TODOs include: 
* Significantly improve the functionality of your system from Milestone M2.
* Incorporate a significant amount of “real” data into your system. 
* Find at least five UH community members (not from ICS 314) to try out your system and provide feedback.
* Implement acceptance testing

Milestone 3 was managed using [Clubs At Manoa GitHub Project Board M2](https://github.com/orgs/Clubs-At-Manoa/projects/4)

![](images/M1 project.png)

Team Contract: [Clubs At Manoa Team Contract](https://docs.google.com/document/d/12P4cILMMUF1ZTil_tapX8uh4npj-fnaBoBRHeb4GNOQ/edit#heading=h.ttlepxesoam)
