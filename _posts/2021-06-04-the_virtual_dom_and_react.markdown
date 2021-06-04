---
layout: post
title:      "The Virtual DOM and React"
date:       2021-06-04 16:12:03 -0400
permalink:  the_virtual_dom_and_react
---


Frontend programming relys on manipulation of the DOM, or the "Document Object Model".  The DOM represents the HTML and XML of a page for the program to connect and make changes to. Though working with the DOM is integral to interactive sites, it can quickly become slow as most Javascript frameworks will re-render each time a change is made, however small. With large applications containing many pages or an extensive DOM tree, modifying the UI can be downright painful.

Welcome the "virtual DOM". The virtual DOM represents a virtual, "ideal" copy of the UI, in-memory. It reflects React's declarative programming pattern in that one can declare what the UI should look like, and the changes will be made in the Virtual DOM. In fact, an entire new copy of the virtual DOM is made with each change in the React program. However, since it is a DOM copy stored in memory and not yet changing the actual DOM, these changes are much more lightweight than changes made through most Javascript frameworks.  With the virtual DOM, changes in a React program's component rendering will trigger a new copy of the virtual DOM to store in memory. This copy is subsequently compared to the actual DOM, or rather, a snapshot the virtual DOM took right before the  update. Through a process called "reconciliation" and using the React DOM library, these changes are finally implemented. Rather than re-rendering more than necessary, the virtual DOM pattern is useful as React will only re-render those parts of the DOM that have changed. 

The traditional DOM can quickly become tedious and slow as applications grow and the DOM tree expands. By storing a copy of the DOM in memory and "reconciling" changes, the virtual DOM pattern provides a significantly faster programming and user experience. 



