## Day 5 - Thursday 30/11/2017

5:28 AM - today I can finally start to actually build the website. The goal for the week is to finish the project by Sunday night. Will I make it? We'll see. Let's do it!

### Recap
During the first four days of the project all I did was the following:
* setup the tools (Gulp, text editore etc)
* applied reset in CSS to avoid inconsistencies among diferent browsers
* give some initial, extremely basic style to the page - font-size for the headings, put some space among sections - just to make it more readable
* created the mockup of the website. I decided to separate the designing part from the building part: considering that the prime focus of CSS Zen Garden, as per the guidelines, is only CSS I found it proper for the occasion to do so. And I was pleased with the result.

### Let's do it
As of yestarday I gave different colors to the three main sections that divide the page which are:
1. intro: contains the header of the page 
    () and the **div** titled "Road to Enlightment"
2. main: it's the central part of the page, contains 5 **[div]**s: 
 * "So What is This About?"
 * "Participation"
 * "Requirements"
 * the footer 
 3. sidebar: this one contains "Select a Design", "Archives", "Resources". It's particular because even though the HTML tells us that it's semantic functin is to be a sidebar, with CSS you have the power of positioning it wherever you want in the page! 
 
 Here's again the visual representation posted yesterday
![divided page](app/images/day4_0?raw=true)

This is just to give me a reference point in order to not get confused. 



### Roadblock 
12:05 PM - I bumped into a roadblock this morning. After what I did above I realized that if I really wanted to put the sidebar content under the "So What is This About" div I would had to insert a section - sidebar - inside another div. Not having the possibility to change the HTML I had two options available:
1. use a combination of relative positioning z-index and pixels, sacrificing responsiveness and diving neck deep into a CSS nightmare 
2. or change the sections order using the **[order]** flexbox propery, which makes things way less complicated. 

You got my choice, right? :D 

Of course this meant that the actual design lost some of its aestethical meaning so a change in the design (again!) was needed. Well, adaptation is a fundamental skill to have in this profession, so I'm glad I had a problem of this kind today. 

Here's the new mockup: 

![new mockup](app/images/day5.png?raw=true)

It was time-consuming but I'm proud of this new design. 

And here's how the actual website looks now

https://codepen.io/davide2894/full/OOadxG/