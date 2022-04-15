# Microwavin Manoa
## Table of contents

* [Overview](#overview)
* [Deployment](#deployment)
* [User Guide](#user-guide)
* [Community Feedback](#community-feedback)
* [Developer Guide](#developer-guide)
* [Development History](#development-history)
* [Team](#team)

## Overview

Many college students have limited kitchen resources, limited cooking skills, limited time, limited access to grocery stores, and no access to creative recipes that respect these constraints. As a result, college students spend money to eat out, or eat non-healthy foods at fast food places or through vending machines.

Microwavin Manoa creates a way for students (on-campus or off) to learn and share recipes that:
* Can be made using minimal kitchen facilities (at a minimum, a toaster oven, or a microwave!).
* Can be made out of ingredients that are available within walking distance of UH.
* Suit local taste sensibilities.
* Can be filtered via dietary restrictions (gluten-free, vegan, etc).
* Have an estimated cost per serving.
* Has an estimated number of servings per recipe.
* Has an estimate of how long it takes to make.

Technologies we plan on using for "Microwavin Manoa":

* [Meteor](https://www.meteor.com/) for Javascript-based implementation of client and server code.
* [React](https://reactjs.org/) for component-based UI implementation and routing.
* [Semantic UI React](https://react.semantic-ui.com/) CSS Framework for UI design.
* [Uniforms](https://uniforms.tools/) for React and Semantic UI-based form design and display.

## Deployment
[Microwavin' Manoa](http://159.223.149.189/#/) website, deployed from Digital Ocean.

## User Guide
A walkthrough for the Microwavin Manoa user interface.

### Landing page

The landing page is the first page presented when users visit the URL.
![landing](images/MMlanding.png)

### Sign In and Sign Up page
If you were previously registered, you are able to "Login" by clicking the button on the upper right button on the navbar.
If not, you are able to make an account by clicking "Sign up".

![singin](images/Screen Shot 2022-04-14 at 8.51.42 PM.png)

### User home page
After successfully logging in, the system takes you to user home page. It is like the landing page, but the NavBar contains links to search recipe and add recipe. You can also view your profile by clicking the option 'view profile' after clicking the user's name:

![userlanding](images/MMlandinguser.png)

### Admin home page
When a user has the admin role, they have an 'Admin' link in the NavBar that lets them view and edit all recipes for all users. 

![adminLanding](images/MMlandingadmin.png)

### Vendor home page
When the user is a vendor, they have a 'Stock' link in their NavBar that let's them edit their stock

![vendor](images/vendorLanding.png)

### User profile page
After logging in, you are able to view your profile, where you have your added recipes.

![userprofile](images/userProfile.png)

### Admin profile page
After logging in, admin can view and edit any recipe from any user.

![admin](images/admin.png)

### Vendor profile page
Vendor's can edit thier profile page which show all the information regarding their store. This includes the store's name, location, hours, stock of items, and the price for each item. There is also a picture of the store so people know what it looks like

![vendorProfile](images/vendorProfile.png)

### Add recipe page
After logging in, Users are able to add recipes

![addrecipe](images/MMaddrecipe.png)

### Search recipe page
On this page you can search for recipes by name or filter search by tags. 

![searchrecipe](images/MMsearchrecipe.png)

### Edit recipe page
After clicking an edit button associated with a recipe, you can edit the parts of that recipe on this page.

![editrecipe](images/editRecipe.png)

### Individual recipe page
Lists all the information for a recipe. It shows the name of the recipe, the different tags it has, a picture of the food the recipe is for, a list of ingredients and their price depending on the store, availability at each store, and the steps for the recipe. 

![indivrecipe](images/MMrecipepage.png)

### Admin edit page
Users defined as admin are able to see all vendor profiles and recipes. They are able to edit this information.

![adminedit](images/MMadminedit.png)

## Community Feedback
Coming soon!

## Developer Guide

### Installation

First, [install Meteor](https://www.meteor.com/install).

Second, [download a copy of Microwavin Manoa](https://github.com/microwavin-manoa/microwavin-manoa).

Third, cd into the app directory and install the required libraries with:

```
$ meteor npm install
```

### Running the system

Once the libraries are installed, you can run the application by invoking:

```
$ meteor npm run start
```

#### Note regarding "bcrypt warning":

You might also get the following message when you run this application:

```
Note: you are using a pure-JavaScript implementation of bcrypt.
While this implementation will work correctly, it is known to be
approximately three times slower than the native implementation.
In order to use the native implementation instead, run

  meteor npm install --save bcrypt

in the root directory of your application.
```

On some operating systems (particularly Windows), installing bcrypt is much more difficult than implied by the above message. Bcrypt is only used in Meteor for password checking, so the performance implications are negligible until your site has very high traffic. You can safely ignore this warning without any problems during initial stages of development.

### Viewing the running app

If all goes well, the template application will appear at [http://localhost:3000](http://localhost:3000).  You can login using the credentials in [settings.development.json](https://github.com/microwavin-manoa/microwavin-manoa/blob/master/config/settings.development.json), or else register a new account.

### ESLint

Lastly, you can run ESLint over the code in the imports/ directory with:

```
meteor npm run lint
```

## Development History

[GitHub Organization](https://github.com/microwavin-manoa) of Microwavin-Manoa containing all its repositories.

The development process for Microwavin Manoa conformed to [Issue Driven Project Management](http://courses.ics.hawaii.edu/ics314f19/modules/project-management/) practices. In a nutshell:

* Development consists of a sequence of Milestones.
* Each Milestone is specified as a set of tasks.
* Each task is described using a GitHub Issue, and is assigned to a single developer to complete.
* Tasks should typically consist of work that can be completed in 2-4 days.
* The work for each task is accomplished with a git branch named "issue-XX", where XX is replaced by the issue number.
* When a task is complete, its corresponding issue is closed and its corresponding git branch is merged into master.
* The state (todo, in progress, complete) of each task for a milestone is managed using a GitHub Project Board.

The following sections document the development history of Microwavin Manoa.

### Milestone 1

The goal of Milestone 1 to form an idea how the site would be set up along with developing very basic mockups for the pages and starting work on the different Mongo collections

Milestone 1 was managed using [Microwavin Manoa GitHub Project Board M1](https://github.com/microwavin-manoa/microwavin-manoa/projects/1):
![](images/M1.png)

### Milestone 2

Milestone 2 is currently being managed using [Microwavin Manoa GitHub Project Board M2](https://github.com/microwavin-manoa/microwavin-manoa/projects/2):

### Milestone 3

Coming soon!

## Team
* [Kailee Hung](https://kaileehung.github.io/), [Carol Wong](https://carolwong492.github.io/), [Jiahui Liao](https://jiahuiliao.github.io/), [Kristyn Mimura](https://kristyn-mimura.github.io/)
* [Team Contract](https://docs.google.com/document/d/1M3Itsauhm6VcdMkSpO9jBSF_vA0zvCPWDgKkCVhjftk/edit?usp=sharing)
