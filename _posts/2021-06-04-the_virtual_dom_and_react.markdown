---
layout: post
title:      "The Virtual DOM and React"
date:       2021-06-04 20:12:02 +0000
permalink:  the_virtual_dom_and_react
---


Frontend programming relys on manipulation of the DOM, or the "Document Object Model".  The DOM represents the HTML and XML of a page for the program to connect and make changes to. Though working with the DOM is integral to interactive sites, it can quickly become slow as most Javascript frameworks will re-render each time a change is made, however small. With large applications containing many pages or an extensive DOM tree, modifying the UI can be downright painful.

Welcome the Virtual DOM. The Virtual DOM represents a virtual, "ideal" copy of the UI, in-memory. It reflects React's declarative programming pattern in that one can declare what the UI should look like, and the changes will be made in the Virtual DOM. In fact, the entire new copy of the Virtual DOM made with each change in the React program. However, since it is a DOM copy stored in memory and not yet changing the actual DOM, these changes are much more lightweight than working with most Javascript frameworks.  With the Virtual DOM, changes in a React program's component rendering will trigger a new copy to store in memory. This copy is subsequently compared to the actual DOM, or rather, a snapshot the Virtual DOM took right before the  update. Through a process called "reconciliation" and the React DOM library, these changes are finally implemented. Rather than re-rendering more than necessary, this particular pattern is useful as React will only re-render those parts of the DOM that have changed, allowing for a much faster programming and user experience!

