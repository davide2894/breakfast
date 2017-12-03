## Day 8 - Sunday 03/12/2017

8:09 AM - Oh well today I woke up later than my preferred time (5:00). When this happened to me in the past the perfectionist in me decided that "well, normally I start to code at 5:30, now it's 8, that's two hours and a half. And since it's so late I lost the momentum, the quiet in the early morning when the world is still sleeping. The entire day is wasted". 

Not this time. I still have the entire morning up until lunch time. Last night, before going to sleep, I also planned to dedicate the afternoon to the Udacity community (forum and Slack channels) and the evening to the blog. As a quote I heard recently said, the time is gonna pass anyway so it's up to me wheter I want to waste the entire day or work for my dream. And I don't even wanna rest "cuz is Sunday!". I don't feel tired, all the opposite. I feel pumped up so let's get going.

### More beans
Yesterday I created the image with the coffee beans going towards the coffee bag. I checked the page now and suddendly I didn't like how short the "coffee road" actually is compared to the one designed in the mockup. All I need to do is to modify the image by making the last part a little bit longer. 

Here it is:

****************************************
****************************************

![day8_0](app/images/day_0.png?raw=true)

****************************************
****************************************


I also increased the font-size of h3, p elements and fixed their position accordingly.

### Orders 
The second section allows the user three things:
* select and view a design among the ones featured in the home page, the best ones so to speak 
* select and vieww all the designes submitted
* consult the archives of the website or even view 

In the HTML file provided by the challenge this section is wrapped around `<aside></aside>` tags, has a class named `.sidebar` and his the last one in order. Since in my design this is the **second** section I need to change the order displayed. Thankfully [Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) provides an easy way to do so. 
First of all I need put `display: flex` and `flex-direction: column` inside the `.page-wrapper` so that each section is considered a flex item to be displayed vertically
Then I need to switch `.main` and `.sibear` orders by using the `order` property that comes with Flexbox. 

    .sidebar {
        oder: 3;
    }
    .main {
        order: 3;
    }
And that's it.

### Donuts
The focus now is this section's style. As a start, let's change the background color from yellow to `#3A170D` 

To understand better the specific HTML structure involved I want to use good ol' pen and paper, don't know about you but for me really heps to sink in new concepts. Just for a laugh take a look at my notes :)

*****************************************
*****************************************
![html structure 1](app/imagses/day8_2.png?raw=true)
*****************************************
*****************************************

*****************************************
*****************************************
![html structure 2](app/imagses/day8_3.png?raw=true)
*****************************************
*****************************************

And here's the work in progress
*****************************************
*****************************************
![html structure](app/imagses/day8_4.png?raw=true)
*****************************************
*****************************************
