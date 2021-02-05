---
layout: post
title:      "Seed Swap Rails Portfolio Project"
date:       2021-02-05 15:17:17 -0500
permalink:  seed_swap_rails_portfolio_project
---


At the beginning of the pandemic, I, as many others did as well, picked up a few new hobbies to help cope with our new and scary world. One of the hobbies I picked up was gardening. As an avid member of a neighborhood site called NextDoor, I thought, "How cool would it be to create an app that helps people exchange seeds with their neighbors?" Considering that travel to the local gardening store was not exactly essential, and interacting with a neighbor, albeit at a distance, might alleviate some quarantine fatigue, I thought a seed swap CMS (alliteration, anyone?) would be a fun project for my portfolio! And thus became Seed Swap!

Seed Swap is a Ruby on Rails application that has User, Seed, and Swap models, with Swap being the object that connects (belongs_to) User and Seed. A User signs up with standard credentials and their zip code, and after signing in, the main interface is populated with "swaps" in that immediate zip code. A User can view the swap, view all of their neighbors swaps, or create their own swaps. 

This project was a lot of fun, but I especially loved implementing my own scope methods for the first time. They sure make life a whole lot easier! In the near future, I hope to amend my application to allow for users to initiate swaps.

Thanks for reading!
