---
layout: post
title:  "Pre-Compiling CSS"
date:   2019-11-9 10:47:25 -0600
categories: jekyll update
author: Maryna
---

CSS preprocessors are a great tool to add functionality and effectiveness to CSS management!

Although basic CSS is elegant, readable and easy to master, when you move on to working with large, complex sites, you might start stumble across its limitations. CSS main limitations are the lack of abstraction, like variables or functions, which means that you have to manually control all the branched out complexity of your style sheets and repeat one and the same code blocks again and again violating the programming principle DRY (Don’t Repeat Yourself) making your code verbose and WET (waste everyone’s time). 

With the power that comes from using variables and functions, CSS preprocessors offer extra functionality that can make website development faster, easier, more scalable and more maintainable: 

+ @import. By using @import you can modularize your code and abstract entire chunks of style snippets into separate files, which makes it easier to navigate through your “style system” and maintain it. 

This website “style system” relies on minima.scss file that imports from base.scss, layout.scss and syntax-highlighting.scss. 

+ $variable. Variables allow you to store a value or a set of values and reuse them throughout your SASS files, which means conforming to DRY, consistency, less reliance on your memory and less copy & pasting. 

This website “style system” includes many variables, such as $base-font-family, $text-color, $background-color, $spacing-unit and so on. 

+ @mixin. By its functionality, mixins can be compared to classes that can be freely reused by other classes (without the latter having to be the children of the former). Mixins can hold numerous CSS declarations and the entire block can be reused, which again means conforming to DRY, consistency, less reliance on your memory and less copy & pasting. 

This website “style system” includes a few mixins, for example, @mixin relative-font-size($ratio) that defines a relative-font-size which is reused multiply times throughout the code.  

+ Nested syntax. Nesting allows a cleaner way of targeting elements and keeps the stylesheet ordered and neat by grouping the corresponding CSS in a nice hierarchical block. With nested syntax, you no longer have to rewrite selectors multiple times, which again conforms to DRY and makes your code more readable and maintainable.

This website “style system” applies nested syntax in, for example, organizing style declarations for navigation and navigation child elements or list and list child elements.

But apart from above mentioned functionality boost, there are also certain disadvantages to CSS preprocessors.

Overusage of mixins and module dependencies might bring about the negative effects of the so-called “tight coupling”.
Tightly coupled systems tend to be fraught with following disadvantages: (<a href="http://blog.millermedeiros.com/the-problem-with-css-pre-processors/">source</a>)
-	A change in one module usually forces a ripple effect of changes in other modules.
-	Assembly of modules might require more effort and/or time due to the increased inter-module dependency.
-	A particular module might be harder to reuse and/or test because dependent modules must be included.

To sum up, CSS preprocessors are a great assistance to website development process, but as with any other assistance of this kind there are certain precautions to be kept in mind. 
