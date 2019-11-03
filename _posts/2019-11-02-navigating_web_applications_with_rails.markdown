---
layout: post
title:      "Sinatra Portfolio Project/Navigating Web Applications with Rails"
date:       2019-11-02 20:00:11 -0400
permalink:  navigating_web_applications_with_rails
---


Rails is a precious tool when it comes to building and navigating web applications. Not only does it provide the framework for easy implementation and continuity across Rails applications, but by way of its structure, gives the developer a virtual roadmap for building complex web applications.

Rails relies on a MVC (Model-View-Controller) framework. The different parts of the framework are in constant communication with each other and a database, which is also included in the framework. Models are the base objects that not only define how objects are saved to the database, but also how each object relates to each other. Views are the data rendered for the viewer in browser; views are usually rendered using a combination of HTML, CSS and ERB (embedded Ruby). With each model comes its associated views, and it is good practice to segregate accordingly. A controller is the conductor in that it defines the routes a web application will follow. Similar to views, it is good practice to build out separate controllers for each model, with each controller only defining the routes to its model's views. When dealing with multiple controllers, a parent "ApplicationController" class must be defined from which subsequent controller classes can inherit from.

Within the MVC framework is another key structure: CRUD. CRUD stands for "Create, Read, Update, Delete" and is an essential functionality that allows for continuity across Rails applications. More importantly, however, the CRUD functionality allows for an application to create and save data, read it, update it, and delete it from the database. The CRUD functionality is defined as routes in a model's respective controller. Using get and post requests, the controller is able to "get" the views, which, as mentioned above, often contain HTML, ERB and forms. The forms collect user data and "post" that data to the receiving "post" route, defined in the controller. The post route is responsible for creating objects from the received user data and saving to the database. Subsequent routes, which define the read, update, and destroy functionality, follow a similar pattern.

In summary, Rails is a powerful tool relying on an MVC framework and CRUD functionality, allowing for the creation and persistence of objects to a database. With it's easy implementation and default structures, it is a great resource when creating complex web applications.

Through the Sinatra Portfolio project, I was able to explore the power of the MVC framework and CRUD routes. I started with the idea of a simple activity tracker for "green" or sustainable activites, such as eating a vegetarian diet, or taking public transportation. Each recorded activity is assigned credits based on the activity type and the length (or units) of that activity. Additionally, an activity type is weighted. So "outreach" is weighted more than "food"; thus, an outreach activity would be worth more than a food activity, if length/units is equal.  It's not flawless by an standard. For example, I would like to weight each activity type realistically based on the relative carbon-offset of each. I would also like to add code that prohibits or assigns negative credits for adding non-sustainable activities.

The most difficult aspect of this project was the update function. To determine the total credits of an activity, based on length and activity type, I created a helper method. Though I tried my darnedest to mass assign updated attributes, I could not get an activity's total credits or the user's balance to update accordingly. I could not figure out how to update an object using the helper method. As a workaround, I had to assign each attribute individually, and then save to the database. Not very pretty, but definitely an opportunity to refactor in the future. 




