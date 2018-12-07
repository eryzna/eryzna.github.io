---
layout: post
title:      " Art_World CLI"
date:       2018-12-07 21:29:24 +0000
permalink:  art_world_cli
---


I have a hard time keeping up with all the cultural events here in Los Angeles, especially gallery openings and new art shows. Going into the CLI project, I wanted to create a program that allowed me to organize the slew of LA events, and parse for anything art-related. Using this concept as a starting point, I then decided I wanted to organize what art events were happening *around the world*. I envisioned my CLI as listing basic details of international art events, and allowing the user to select a single event for more information. Enter, Art World.

There are plenty of popular art websites that publish art news and events, so I started with one of my favorites: Artnet. I felt this was the perfect site for my CLI needs--it had a page that listed all upcoming events, and a detail page for each event, which included gallery information, artists in the show, a press release, and more. However, after successfully scraping the events page and creating objects, I went to the detail page only to discover a new animal: Javascript. As much as I wanted to learn to scrape Javascript, for the purposes of the project,  I decided to scrape another website. Frieze contains much of the same information as Artnet, without the Javascript.  

Using Frieze  as the data source, the Art World scrapes the upcoming events page and initializes objects, whereupon the CLI prints a list containing those object elements: gallery name, exhibition title, the dates of the exhibition, and location. The user can either select a number from the list, or exit. After choosing an exhibition, the CLI prints information scraped from individual gallery pages: address, telephone, email, and website. The user then has the option to choose another exhibition, or exit.

This project taught me a ton. I used pry an inumerable amount, but I gained a deeper insight into creating objects, scraping pages, and communication between classes. 
