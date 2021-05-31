---
layout: post
title:      "React/Redux Final Project"
date:       2021-05-31 23:34:55 +0000
permalink:  react_redux_final_project
---


For my final project, I used a Rails API with a React/Redux frontend. The project lets a user explore various philosophical movements and quotes expressing each movement's respective philosophical doctrine. In addition, a user can add a movement and quote, as well as make edits. 

I used Redux to create a store, and after fetching /categories and /quotes, used it to hold these resources. Using this pattern, I was able to call these props from within my app. I encountered a problem, however, when rendering a component using a route defined by React router. Once rendered, my component did not have access to the store, and therefore the appropriate props were not passed down. I stuck with a local fetch request to gather the needed resources, but plan on returning to the problem to resolve it.

It was difficult for me to get accustomed to thinking in the React pattern, but I grasped it enough to complete the project (hopefully). I look forward to exploring it more and returning to refactor and expand upon my project. 
