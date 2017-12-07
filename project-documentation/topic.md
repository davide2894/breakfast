# Goal
This project is my humble attempt at the omonym challenge. The interesting part is that the website has the same html, each version is made by customizing only the CSS file! 

[Official source: csszengarden.com](http://www.csszengarden.com)

This is the first time I share a project while I am working at it. I guess it's a good learning opportunity for everyone. #
Expect daily updates with progress report.

## Tools used 
* [Brackets](http://brackets.io): text editor
* [Gulp](https://gulpjs.com): task-automation. 
* [official index.html](http://www.csszengarden.com), not to be edited
* [MockFlow](): useful website to build mockups without having to use more complex programs. It's intuitve, no instructions needed :)

# Website 
Check the progresses directly on the website hosted on **Github Pages**. https://davide2894.github.io/css-zen-garden/

## Day 1 - Sunday 26/11/2017

[details="Read"]
Today I start this new project after finishing [Magic: The Gathering card replica in HTML and CSS](https://github.com/davide2894/Magic-The-Gathering-card-in-HTML-and-CSS).

I downloaded the offical index.html. Then I setup [Gulp](https://gulpjs.com), since this is not the first time I am using it I didn't need to congifure every task from scratch, I just copy-pasted the folder structure and the gulpfile.js from the [portfolio project](https://github.com/davide2894/portfolio).
To learn more about Gulp and how to configure it follow [CSS-Tricks' own guide for beginners ](https://css-tricks.com/gulp-for-beginners/). It's what I used to learn how to make a basic configuration to reduce time-wasting and improve the workflow.

### Reset
The first thing to do is a [reset](https://meyerweb.com/eric/tools/css/reset/) because the optimal result is to have the website behave the same way accross browser. To achieve so I need to avoid inconsistencies by removing default settings inside browsers, such as headings, font-sizes etc.

Since I can't edit in any way the index.html provided I have to modify the gulpfile, so what I need to do is the following:
* delete "sass" task (that compiles any sass file into css)
* edit "watch" task to monitor any change in the "style.css" file
* delete app/js/ folder

![before-resert|690x387](upload://5VY8J19rWKiQVukJVrEm7AqoFbf.png)

![after-reset|690x387](upload://ibDlWOdRwDj0JSXPb85PX9GnEH1.png)

### Initial style
Added basic font-sizes:

    h1 {
    font-size: 44px;
    font-weight: 800;
    }
    h2 {
        font-size: 36px;
    }
    h3 {
        font-size: 28px;
    }

Then some centering and margin:

    .page-wrapper {
        max-width: 1280px;
        margin: 0 auto; /*centers the page*/
    }
    div {
        margin-bottom: 22px;
    }
    
Centered page
![initial-style|690x387](upload://hLppsMRjdZnPdo9FVcV3phCCb0S.png)

Next point now is to come up with my own page design, the main thing to do actually. After researching for a while on [Dribble.com](https://dribbble.com) [this]() caught my eye (I'm particularly fond of split design), I'll be using it as inspiration for the project.
This means I won't use its asset.

As for the color combination, I found [this combo on Pinterest](https://www.pinterest.co.uk/pin/416864509237410284/). It's cool, so let's roll with it.

### Designing the mockup
So far this is going to be the most difficult part of the project. I'm using MockFlow, an intuitive website to build - as the name suggests - website mockups just discovered this morning.
 
![26-11-17|690x387](upload://84sG3mvofilQqWXSQ5EueCgTsvv.png)

### Recap
This was what I did today for this project.:
* setup the project folder
* setup Gulp
* reset CSS
* an initial styling
* started designing the website mockup

### Conclusion
Thank you so much for reading this topic, I hope it heps everyone, myself included, in improving my understanding of web development.
Please let me know what you think, also if you have any question just write it down!




[/details]

## Day 2   - Monday 27/11/2017
[details="Read"]
Today is the second day I dedicate to this project. The goal I have is to at least finish the mockup. Let's start.

...

I'm going with the flow though slowly. I wonder if it's the same for professional designers. I lost count of how many times I deleted and created an element of the page. Again and again and again because I was either not satisfied of the outcome or something better came up in my mind. 

Anyway, this is today's work
![day2|134x500](upload://rm2Y8gn7ztgqrf5d3oiLFdwMTUZ.png)

### Conclusion
I didn't hit my project goal for today i.e. I didn't finish to design the mockup. It took more than expected to be honest. One thing I noticed while working on it was that designing is kinda like programming in terms of energy demands. Creativity works in the same way as stamina, at least for me.
[/details]

## Day 3 - Tuesday 28/11/2017

[details="Read"]
Third day of the project. On the first day I basically set up everything I needed, then I started to design the website mockup. The following day I continued this very task knowing that the overall look is getting better. I did half of the page. The goal is the same as yesterday: finish to design the page. Let's go!

The "Participation" and "Benefits" sections can go together as the latter has a particularly short text. Not sure a split screen visualization can be achieved. 

By the way, I found this cool color matcher online named [Coolors.co](https://coolors.co/421e15-8fd694-4fb286-b5d6b2-f3f7f0). The color palettes are showed in full screen with the relative hex!

Oh my...things got out hands. The mockup became kawaii //insert shocked face. I started to search for a simple donut icon to insert as background then for a cute cupcake and last thing I know I typed "unicor vomiting rainbow" on Google. Ok. Don't worry: you won't see it on the page.

I just finished the footer. Not satisfied. The general result is ok but this last piece of the puzzle is meh. Need to change that.

Here's the result
![day3|61x500](upload://1QVy9bEF3HtssqIQbEn9MScqCaY.png)
[/details]

## Day 4 -  Wednesday 29/11/2017
[details="Read"]
Another day has come, it's 5:19 AM. Clean face: check. Brush teeth: check. Coffee: check. Time to continue this project. 
The first three days went well, except for the footer of the page whom I want to improve. Remember, I can't modify the index.html file of the project, not even in the slightest. 
In the mentioned document I noticed that the "Resources" and "Archives" divs are both part of the same block like the following simple representation: 

```html
<aside class="sidebar>
    
    <!-- "Select a Design" -->
    <div class="design-selection></div> 
    
    <!-- "Archives" -->
    <div class="design-archives></div> 
    
    <!-- "Resources" -->
    <div class="zen-resources></div> 
    
</aside>
```

Here's how the page looks at the moment, ugly :face_vomiting:
![day4_2|565x500](upload://qQAdzKpWeeezdd999hRKrm5ORsg.png)

Now I am going to put things into order and edit the design as needed. 

Project goal for today:
* fix html order
* modify current design as needed 
* finish the page's design
* ask for feedback

Let's do it!

...

I asked for feedback on Slack and I was pleased to receive good critic despite the early hour. 

So it seems the bottom of the website, from "Benefits" till the end is not - as I suspected - designed well as it doesn't match the upper-half theme. Let's make it more delicious then! 


Here it is
![day4_1|55x500](upload://4XzwiMvoRTeh2SbmjLOpw3T3Ow3.png)
I think the design is finished, so now I can start building! Thank you for the kind feedback, it's helping me alot. For instance, if I wouldn't ask this morning on Slack for feedback I wouldn't have the chance to make the design as it is right now. 

As always please let me know what you think. Every single reply is important :D
[/details]

## Day 5 - Thursday 30/11/2017


[details="Read"]
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
![day4_2|565x500](upload://qQAdzKpWeeezdd999hRKrm5ORsg.png)

This is just to give me a reference point in order to not get confused. 

### Roadblock 
12:05 PM - I bumped into a roadblock this morning. After what I did above I realized that if I really wanted to put the sidebar content under the "So What is This About" div I would had to insert a section - sidebar - inside another div. Not having the possibility to change the HTML I had two options available:
1. use a combination of relative positioning z-index and pixels, sacrificing responsiveness and diving neck deep into a CSS nightmare 
2. or change the sections order using the **[order]** flexbox propery, which makes things way less complicated. 

You got my choice, right? :D 

Of course this meant that the actual design lost some of its aestethical meaning so a change in the design (again!) was needed. Well, adaptation is a fundamental skill to have in this profession, so I'm glad I had a problem of this kind today. 

Here's the new mockup: 


[details="For a better view: opein it in a new tab then zoom in"]
![day5|55x500](upload://iJ1Kbv572kOqWsyEVhqujOKolw3.png)
[/details]


It was time-consuming but I'm proud of this new design. 

And here's how the actual website looks now (view it full-screen on Codepen)

https://codepen.io/davide2894/pen/OOadxG

### Questions:
1. What do you think?
2. What would you change?
3. Are you interested in taking this challenge yourself?

Let me know!
[/details]

## Day 6 - Friday 01/12/2017

[details="Read"]
5:50 AM - It's already Friday! When did week this pass?? Time sure flies. Yesterday I finally started - though not without issues - to build the website from the mockup I created. The Udacity community gave me some useful feedback on it. Again, without them this project wouldn't be what it is, the design would have a different look.

### Pseudo elements
8:16 AM - I'm having some trouble with the cup image: the HTML can't be touched hence the only way to put the image as per the mockup is via [pseudo elements](https://css-tricks.com/almanac/selectors/a/after-and-before/). The downside of this trick is that is not possible to resize insisde CSS, it must done before anything else. 

With Gimp I can resize easily. Then there are two things to do:
* use the pseudo elements ::after to actually insert the image, specifically
    
    
    h2::after {
        content: url(images/coffee-hot-cup.jpg);
    }
    
    
* use relative positioning to put it at the wanted spot, on the right of "The Beauty of CSS Design"
    
    
    h2::after{
    content: url(images/coffee-hot-cup.jpg);
    margin-left: 3%;
    }
    
Here's the resul:

![Header](app/images/day6.png?raw=true)

### The Road to Enlightment
Time to style the biggest part of the first section.

This looks quite a tough one to do, I'm stuck at the CSS because I don't know how to render the mockup text alignment. Also, I'm still working on making that part of the mockup, the one with coffee beans going down the page, a background image. 
![day6_1|458x500](upload://zMvw3ZMYSAX1Zd7FlLgpdiNiflD.png)

Do you have suggestions on how can I translate the above image into CSS?

Here's the result for today.
https://codepen.io/davide2894/pen/yPGxZr
[/details]


## Day 7 - Saturday 02/12/2017


[details="Read"]
5:37 AM - seventh day for the project. I started yesterday to build the page. 

### Udacity community to the rescue
I asked for feedback to the Udacity community since I was desperate for help and damn if I didn't received it. Both from mentors and fellow students. You are awesome :D .It helped to feel less frustrated over it, to see the problem from another perspective, not as big as I thought it was. All this new info from the community was heading torward the simplest solution: build the background image directly, by using an image editor (and yes, place the little coffee beans one by one). The simplest solution is not always the easiest, right? But I must be careful: I don't want to lose any resolution in this process. The background image is going to be full-screen. Blurred brown dots would not be any good to look at :D

Well, let's see what I can do.

### Paragraphs
To put heading and paragraphs in their exact positions I need to use CSS alignment i.e. the [position property](https://www.w3schools.com/cssref/pr_class_position.asp). More specifically the 
/*position: relative*/ property that allows me to do two important things:
1. move the element arbitrarly but
2. keep it in the document flow ergo the element stays inside its own div and respects the hierachic order.

But there is a problem: it sacrifices responsiveness. I am worried  so I ask my dear friend Google. I find [this hack on God-bless-you Stack Overflow](https://stackoverflow.com/questions/44217169/css-position-relative-with-responsive-height). 
Basically the concept is this: 
* after `position: relative` **use padding instead of the left, right, bottom, top properties normally used in this case**
* use **% instead of pixels** because if you move an element of a specific `px` amount it can't be responsive. But by using % is possible to achieve so as the page will keep its element-page aspect ratio. 

To apply this new learned concept on the website I code the following: 

    
    position: relative;
    height: 0;
    width: 50%;
    padding-left: 20%;
    
![day7_0|690x375](upload://mFK0q3CzKjXofHAnMScW7q7Q4GZ.png)

### The Coffee Road
I struggled but at the end I obtained a decent result. Gimp sure is a difficult program to get comfortable with. Among layers, masks and the myriads of tools, each with its own key shortcut I felt like the new student at school. If you'd like to learn more of Gimp check the [official documentation](https://docs.gimp.org/docs/) (but I warn you, it's quite a long read).

First thing I did was trying to resize the coffee-bean.png file I download from 
[Flaticon](https://www.flaticon.com) only to discover that .png files lose resolution when resized (say what?). So? Turns out that [SVG](https://en.wikipedia.org/wiki/Scalable_Vector_Graphics) files don't lose resolution as they are just XML documents BUT resizing them in any image editor program - such as my fellow Gimp or the likes - isn't so straightforward. Scaling .png and .svg are two completely different processes. 
Then I find [this](https://www.hongkiat.com/blog/resize-export-svg-png-myscale/) simple yet so effective web application that handles the hard work for me and voilà, the trick is done. Now I have at my disposal a small-sized SVG file I can use repeatedly to create the background image I want.

...

And here it is

![day7_1|467x500](upload://gDaCv2e2KqUtG78GcahGsUO7Nga.jpg)

...

While positioning the elements by using the above mentioned CSS trick somenthing bad was happening: the elements were behaving well but the image was not. In fact if I zoomed in or out the latter would stay the same while the former would change font-sizes accordingly, throwing out of the window the meaning of positioning itself. So I had to use the classic CSS alignment at the expense of responsiveness. I don't know how to achieve that but if you happen to know so **please** write it down :disappointed_relieved:

And here we are, I'm not sure about the quality of today's output on the project but anyway 

https://codepen.io/davide2894/pen/JOxEWZ?editors=1100    

For more detailed information, check the [commit I pushed on GitHub](https://github.com/davide2894/css-zen-garden/commit/30113cf8879bbd51a39d7b8521003a2acacddaf6).

Thanks to @vipper_maeglin for suggesting to use transparent background.
[/details]

## Day 8 - Sunday 03/12/2017


[details="Read"]
8:09 AM - Oh well today I woke up later than my preferred time (5:00). When this happened to me in the past the perfectionist in me decided that "well, normally I start to code at 5:30, now it's 8, that's two hours and a half. And since it's so late I lost the momentum, the quiet in the early morning when the world is still sleeping. The entire day is wasted". 

Not this time. I still have the entire morning up until lunch time. Last night, before going to sleep, I also planned to dedicate the afternoon to the Udacity community (forum and Slack channels) and the evening to the blog. As a quote I heard recently said, the time is gonna pass anyway so it's up to me wheter I want to waste the entire day or work for my dream. And I don't even wanna rest "cuz is Sunday!". I don't feel tired, all the opposite. I feel pumped up so let's get going.

### More beans
Yesterday I created the image with the coffee beans going towards the coffee bag. I checked the page now and suddendly I didn't like how short the "coffee road" actually is compared to the one designed in the mockup. All I need to do is to modify the image by making the last part a little bit longer. 

Here it is:
![day8_0|161x500](upload://5LiOPfKje3fvhUEl4aL2yY3GSiR.png)

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

![day8_2|375x500](upload://vzUbHoxoXSkvXaNtDY2MJd6hoOo.JPG)

![day8_3|375x500](upload://9FZdZUX3qDmoJvFvceWlH9S7tiI.JPG)


Here's the work in progress
![day8_4|690x387](upload://fILebc0gmBU6ElPnJUedsl0JBOV.png)

For a more details check my the [commit to GitHub](https://github.com/davide2894/css-zen-garden/commit/feefd4c3ee005c021339b47b9967c14250494e9c)
[/details]

## Day 9 - Monday 04/12/2017


[details="Read"]
5:34 AM - It's a new day, yes it is! *music starts playing* (any WWE fan here?)

Let's continue the work started yesterday with the `.sidebar` section.

### Select a Design
This section is the the second the three. As of yesterday this area of the website was fairly similar to a construction site, after today I hope that it looks better :D

So the first thing to do is the section's layout. Thanks to Flexbox this is achievable without too many headaches. To recap, the desired result is the following: 

![day8_1|335x500](upload://n8cyOyww5dBAfz1mLkhqigPUlqy.png)

**How ?** 

1 - set Flexbox direction to row and enable wrapping

    .wrapper {
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;  
        -webkit-box-orient: horizontal;  
        -webkit-box-direction: normal;  
        -ms-flex-flow: row wrap;  
        flex-flow: row wrap;
        background: url(./images/donut.png) center/contain no-repeat;
        margin-bottom: 10%;
    }
    
    
2 - set the "Select a Design" part to occupy the entire width available on the screen, so that "Archives and "Resources" slip to the second row and both occupy half of the space available.

    .design-selection {
        -webkit-box-flex: 2;
        -ms-flex: 2;
        flex: 2 100%;
        margin-bottom: 5%;
    }
    
    .design-archives,
    .zen-resources {
        -webkit-box-flex: 1;
        -ms-flex: 1;
        flex: 1;
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -webkit-box-orient: vertical;
        -webkit-box-direction: normal;
        -ms-flex-direction: column;
        flex-direction: column;
    }

And that's it! Isn't it amazing? :D

#### Header 
This is easy as I only need to
* fix the `font-size` to make it bigger
* set `font-family` to Lobster as the first font and "cursive" as the fallback, just in case the browser doesn't read the first one
* set the color to `#FDBA55` (a yellow variation)

        select{
        font-size: 6em;
        font-family: "Lobster", cursive;
        color: #FDBA55;
        }

#### Design list box
Besides colors it needs size adjustments:
    
    .design-selection ul {
        width: 28vw;
        height: 48vh;
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -webkit-box-orient: vertical;
        -webkit-box-direction: normal;
        -ms-flex-direction: column;
        flex-direction: column;
        -ms-flex-pack: distribute;
        justify-content: space-around;
        padding: 2%;
        background-color: #333;
        border: 10px solid #fdba55;
        border-radius: 6px;
        margin-bottom: 5%;
    }
    `
    
Now I focus on the single list items, they need some color, a bit of centering and more [font-weight](https://developer.mozilla.org/en-US/docs/Web/CSS/font-weight):
    
    
    .design-selection li {
        font-size: 1.3em;
        color: #fff;
        font-weight: 600;
        margin-left: 10%;
    }
   

I also need to put some space between the name of design and designer. I chose to do so by putting some horizontal margin there:

    
    .design-name{
       margin-right: 1%;
    }
    .designer-name {
       margin-left: 1%;
    }
    
    
Here's the result so far: 
![day9_0|527x500](upload://e1GWzQvbz1x94wASbp6PETLjWWs.png)
Now let's focus on the other two sub-parts of this sections.
 
#### Archives and Resources
The HTML code of these two `div`s are basically the same, meaning they have the same structure, hence they can be customized at the same time by using two selectors together.

For a start let's center them:

    
    .design-archives > *, 
    .zen-resources > * {
        margin: 0 auto;
    }
    
    
What's that? It's a shortcut to select all the elements contained in a class, so simple yet so useful. When I write `.class-name > *` I'm telling CSS "hey, see this class? Do me a favor: go look every single element that you contain and style them as I tell you ". Read more about the [CSS * selector](https://www.w3schools.com/cssref/sel_all.asp).

Then I can give some simple style to the respective titles:

    
    .archives,
    .resources {
        font-size: 3em;
        padding: 0 0 5% 0;
    }
    
    
Increase the size of the characters written in the list items::

    
    .design-archives ul,
    .zen-resources ul {
        font-size: 1.5em;
    }
    
Le's make these two menus look better :) 

Now I want to select each list item - except the last one - in order to do three things:
* put some padding all around it
* put some margin at the bottom so that there is some distance between the end of this section and the next one coming
* put some shadow around the now visible boxes at every list item so that they do not look flat
    
    
    
    .design-archives li:not(last-of-type),
    .zen-resources li:not(last-of-type) {
        margin-bottom: 5%;
        padding: 22px;
        text-align: center;
        -webkit-box-shadow: -2px 5px 2px #333;
        box-shadow: 2px 5px 2px #;
    }
    
    
But it's not enough because there is still a final touch of color to give:

    
    .design-archives li,
    .zen-resources li {
        background: #333333;
        border: 5px solid #FDBA55;
        border-radius: 6px;
    }
    .design-archives {
        border-right: 2px solid #FDBA55;
    }
    
    
    
Here's the result:
![day9_1|690x325](upload://3GLGVLZ8kRRmE52GwywBslHrX5n.png)

#### Donut background
Last part for today. A donut background with a good amount of opacity (i.e. transparency). But how can I edit a background image's opacity inside CSS?? I researched on the internet and found the following possible solutions: 

* [this](https://scotch.io/tutorials/how-to-change-a-css-background-images-opacity)
* [and this](https://stackoverflow.com/questions/4183948/css-set-background-image-with-opacity)

Unfortunately I couldn't make it work in either of these way. I wanted to persist though so after a few headaches I came to the most simple solution: edit the opacity in Gimp. Why do I overcomplicate things so much sometimes? :(

# Website 
The website is now published on GitHub Pages, feel free to check it out :D
https://davide2894.github.io/css-zen-garden/

#### Commit
Lastly, be sure to check out [today's commit](https://github.com/davide2894/css-zen-garden/commit/6f10f6e462ee359e42f005d0f71e850b622af231) as well :D
[/details]

## Day 10 - Tuesday 05/12/2017 

[details="Read"]
5:33 AM - it's a new day, yes it is! It's early morning, the world is still sleeping. There is total quiet now. 

### Main section
This is the third and last part of the mockup I designed though the longest. It is divided in 5 sub-parts that are the following:
1. So What is This About?
2. Participation
3. Benefits
4. Requirements
5. Footer (including the buiscuits splashing in the milk at the very bottom of the page) 

One by one, let's do this.

### So What is This About? 
The goal is to achieve the following look, as per the mockup:

![day10_0|382x500](upload://hKjMHpO1YskIIiy1SnewEaxCOvA.png)

Only thing to change is the border as I think it would be better if it would look like a chocolate square.

The work divided in different areas:
* layout
* font
* colors

Check out the [website](https://davide2894.github.io/css-zen-garden/) to see the result.

For a full-detailed version of changes, check [today's commit](https://github.com/davide2894/css-zen-garden/commit/741655f1c267aaca6fc86ab4cf274e5506d14468)

P.S. Sorry for the short post today, I couldn't stay at the computer all day for personal reasons.
[/details]

## Day 11 - Wednesday 06/12/2017

5:46 AM - we're almost at the middle of December, time sure flies!

Let's get some fun with the project.

### Main section
This is the third and last part of the mockup I designed though the longest. It is divided in 5 sub-parts that are the following:
1. So What is This About?
2. Participation
3. Benefits
4. Requirements
5. Footer (including the buiscuits splashing in the milk at the very bottom of the page) 

Yesterday I did the first one. Let's do the second.

#### Participation
The desired result is the following:
![day11_0|530x500](upload://oTiwAb3oKSNMYHkDRDtKQivm1yE.png)

The first thing I did was to setup Flexbox to handle the layout. Then I worked on the yellow area of this part, specifically I set the dimensions, relative position, text font, color and size. Background color and image, and lastly the padding. 

Below you can see the code

    /*
        --------------------------
            Participation
        --------------------------

    */
    .participation {
        height: 100vh;
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -webkit-box-orient: vertical;
        -webkit-box-direction: normal;
        -ms-flex-direction: column;
        flex-direction: column;
        background: url(images/cupcake.png) no-repeat 88% 80%;
        background-color: #B6D5B3;
    }

    .participation>* {
        max-width: 50%;
        position: relative;
        top: 5vh;
        left: 15vh;
        background: #FEBA55;
        padding: 0 4%;
        z-index: 1;
        -webkit-box-shadow: 0 2px 2px 0px #333;
        box-shadow: 0 2px 2px 0px #333; 
    }
    .participation h3 {
        font-size: 8em;
        padding-top: 4%;
        padding-bottom: 4%;
    }
    .participation p {
        font-size: 1.5em;
        line-height: 1.38;
        letter-spacing: 2px;
        padding-bottom: .5%;
    }
    .participation p:last-of-type {
        padding-bottom: 8%;
    }


#### Benefits

The goal look is the following:
![day11_1|690x467](upload://a8wpUF5bX1rvDCc5qA9VLjCSmXU.jpg)

The work to be done was not so much to be honest. In fact the tasks to do were the following:
* setup Flexbox
* set padding and margins
* decide the font color, size, line height and letter spacing
* position the coffee stain image as per the design mockup
* set background color


    /*
        -----------------------
            Benefits
        -----------------------
    */
    .benefits {
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -webkit-box-orient: vertical;
        -webkit-box-direction: normal;
        -ms-flex-direction: column;
        flex-direction: column;
        padding: 50% 20%;
        background: url(./images/coffe-circle-stain.png) no-repeat 73% 63.4%; 
        background-color: #FFEAC1;
    }
    .benefits>* {
        -ms-flex-item-align: center;
        align-self: center;
    }
    .benefits h3 {
        font-size: 10em;
        letter-spacing: 10px;
        margin-bottom: 10%;
    }
    .benefits p {
        width: 75%;
        font-size: 1.5em;
        letter-spacing: 0.6px;
        line-height: 1.5
    }


#### Requirements
![day11_2|444x500](upload://lSF64sTvURUP6ayL0HitWoMtPQW.png)

The work to do here is for most part the same as above.
One exeption is the line above the last paragraph. I realized by using the [[border-top]] property that can be set as a normal border. 

    /*
    -------------------------
        Requirements
    -------------------------
    */
    .requirements,
    footer {
        background-color: #ffcdb2;
    }
    .requirements {
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -webkit-box-orient: vertical;
        -webkit-box-direction: normal;
        -ms-flex-direction: column;
        flex-direction: column;
        padding: 20% 25%;
    }
    .requirements>* {
        -webkit-box-flex: 1;
        -ms-flex: 1 100%;
        flex: 1 100%;
    }
    .requirements h3 {
        font-size: 12em;
        -ms-flex-item-align: center;
        align-self: center;
        margin-bottom: 16%
    }
    .requirements p {
        width: 146%;
        -ms-flex-item-align: center;
        align-self: center;
        text-align: justify;
        font-size: 2em;
        line-height: 1.5;
        letter-spacing: 2px;
    }
    .requirements p:nth-child(5) {
        margin-bottom: 25%;
    }
    .requirements p:last-of-type {
        border-top: 6px solid #333;
        padding-top: 6%;
    }

I couldn't finish all of the footer today, so the rest will come tomorrow!

***
# Action
See [today's commits](https://github.com/davide2894/css-zen-garden/commits?author=davide2894&since=2017-12-05T23:00:00Z&until=2017-12-06T23:00:00Z) for a more detailed illustration.

Please check the [website](https://davide2894.github.io/css-zen-garden/) and give me your opinion on it 

Please give me your opinion on it, I would be immensely grateful for it.
# Goal
This project is my humble attempt at the omonym challenge. The interesting part is that the website has the same html, each version is made by customizing only the CSS file! 

[Official source: csszengarden.com](http://www.csszengarden.com)

This is the first time I share a project while I am working at it. I guess it's a good learning opportunity for everyone. #
Expect daily updates with progress report.

## Tools used 
* [Brackets](http://brackets.io): text editor
* [Gulp](https://gulpjs.com): task-automation. 
* [official index.html](http://www.csszengarden.com), not to be edited
* [MockFlow](): useful website to build mockups without having to use more complex programs. It's intuitve, no instructions needed :)

# Website 
Check the progresses directly on the website hosted on **Github Pages**. https://davide2894.github.io/css-zen-garden/

## Day 1 - Sunday 26/11/2017

[details="Read"]
Today I start this new project after finishing [Magic: The Gathering card replica in HTML and CSS](https://github.com/davide2894/Magic-The-Gathering-card-in-HTML-and-CSS).

I downloaded the offical index.html. Then I setup [Gulp](https://gulpjs.com), since this is not the first time I am using it I didn't need to congifure every task from scratch, I just copy-pasted the folder structure and the gulpfile.js from the [portfolio project](https://github.com/davide2894/portfolio).
To learn more about Gulp and how to configure it follow [CSS-Tricks' own guide for beginners ](https://css-tricks.com/gulp-for-beginners/). It's what I used to learn how to make a basic configuration to reduce time-wasting and improve the workflow.

### Reset
The first thing to do is a [reset](https://meyerweb.com/eric/tools/css/reset/) because the optimal result is to have the website behave the same way accross browser. To achieve so I need to avoid inconsistencies by removing default settings inside browsers, such as headings, font-sizes etc.

Since I can't edit in any way the index.html provided I have to modify the gulpfile, so what I need to do is the following:
* delete "sass" task (that compiles any sass file into css)
* edit "watch" task to monitor any change in the "style.css" file
* delete app/js/ folder

![before-resert|690x387](upload://5VY8J19rWKiQVukJVrEm7AqoFbf.png)

![after-reset|690x387](upload://ibDlWOdRwDj0JSXPb85PX9GnEH1.png)

### Initial style
Added basic font-sizes:

    h1 {
    font-size: 44px;
    font-weight: 800;
    }
    h2 {
        font-size: 36px;
    }
    h3 {
        font-size: 28px;
    }

Then some centering and margin:

    .page-wrapper {
        max-width: 1280px;
        margin: 0 auto; /*centers the page*/
    }
    div {
        margin-bottom: 22px;
    }
    
Centered page
![initial-style|690x387](upload://hLppsMRjdZnPdo9FVcV3phCCb0S.png)

Next point now is to come up with my own page design, the main thing to do actually. After researching for a while on [Dribble.com](https://dribbble.com) [this]() caught my eye (I'm particularly fond of split design), I'll be using it as inspiration for the project.
This means I won't use its asset.

As for the color combination, I found [this combo on Pinterest](https://www.pinterest.co.uk/pin/416864509237410284/). It's cool, so let's roll with it.

### Designing the mockup
So far this is going to be the most difficult part of the project. I'm using MockFlow, an intuitive website to build - as the name suggests - website mockups just discovered this morning.
 
![26-11-17|690x387](upload://84sG3mvofilQqWXSQ5EueCgTsvv.png)

### Recap
This was what I did today for this project.:
* setup the project folder
* setup Gulp
* reset CSS
* an initial styling
* started designing the website mockup

### Conclusion
Thank you so much for reading this topic, I hope it heps everyone, myself included, in improving my understanding of web development.
Please let me know what you think, also if you have any question just write it down!




[/details]

## Day 2   - Monday 27/11/2017
[details="Read"]
Today is the second day I dedicate to this project. The goal I have is to at least finish the mockup. Let's start.

...

I'm going with the flow though slowly. I wonder if it's the same for professional designers. I lost count of how many times I deleted and created an element of the page. Again and again and again because I was either not satisfied of the outcome or something better came up in my mind. 

Anyway, this is today's work
![day2|134x500](upload://rm2Y8gn7ztgqrf5d3oiLFdwMTUZ.png)

### Conclusion
I didn't hit my project goal for today i.e. I didn't finish to design the mockup. It took more than expected to be honest. One thing I noticed while working on it was that designing is kinda like programming in terms of energy demands. Creativity works in the same way as stamina, at least for me.
[/details]

## Day 3 - Tuesday 28/11/2017

[details="Read"]
Third day of the project. On the first day I basically set up everything I needed, then I started to design the website mockup. The following day I continued this very task knowing that the overall look is getting better. I did half of the page. The goal is the same as yesterday: finish to design the page. Let's go!

The "Participation" and "Benefits" sections can go together as the latter has a particularly short text. Not sure a split screen visualization can be achieved. 

By the way, I found this cool color matcher online named [Coolors.co](https://coolors.co/421e15-8fd694-4fb286-b5d6b2-f3f7f0). The color palettes are showed in full screen with the relative hex!

Oh my...things got out hands. The mockup became kawaii //insert shocked face. I started to search for a simple donut icon to insert as background then for a cute cupcake and last thing I know I typed "unicor vomiting rainbow" on Google. Ok. Don't worry: you won't see it on the page.

I just finished the footer. Not satisfied. The general result is ok but this last piece of the puzzle is meh. Need to change that.

Here's the result
![day3|61x500](upload://1QVy9bEF3HtssqIQbEn9MScqCaY.png)
[/details]

## Day 4 -  Wednesday 29/11/2017
[details="Read"]
Another day has come, it's 5:19 AM. Clean face: check. Brush teeth: check. Coffee: check. Time to continue this project. 
The first three days went well, except for the footer of the page whom I want to improve. Remember, I can't modify the index.html file of the project, not even in the slightest. 
In the mentioned document I noticed that the "Resources" and "Archives" divs are both part of the same block like the following simple representation: 

```html
<aside class="sidebar>
    
    <!-- "Select a Design" -->
    <div class="design-selection></div> 
    
    <!-- "Archives" -->
    <div class="design-archives></div> 
    
    <!-- "Resources" -->
    <div class="zen-resources></div> 
    
</aside>
```

Here's how the page looks at the moment, ugly :face_vomiting:
![day4_2|565x500](upload://qQAdzKpWeeezdd999hRKrm5ORsg.png)

Now I am going to put things into order and edit the design as needed. 

Project goal for today:
* fix html order
* modify current design as needed 
* finish the page's design
* ask for feedback

Let's do it!

...

I asked for feedback on Slack and I was pleased to receive good critic despite the early hour. 

So it seems the bottom of the website, from "Benefits" till the end is not - as I suspected - designed well as it doesn't match the upper-half theme. Let's make it more delicious then! 


Here it is
![day4_1|55x500](upload://4XzwiMvoRTeh2SbmjLOpw3T3Ow3.png)
I think the design is finished, so now I can start building! Thank you for the kind feedback, it's helping me alot. For instance, if I wouldn't ask this morning on Slack for feedback I wouldn't have the chance to make the design as it is right now. 

As always please let me know what you think. Every single reply is important :D
[/details]

## Day 5 - Thursday 30/11/2017


[details="Read"]
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
![day4_2|565x500](upload://qQAdzKpWeeezdd999hRKrm5ORsg.png)

This is just to give me a reference point in order to not get confused. 

### Roadblock 
12:05 PM - I bumped into a roadblock this morning. After what I did above I realized that if I really wanted to put the sidebar content under the "So What is This About" div I would had to insert a section - sidebar - inside another div. Not having the possibility to change the HTML I had two options available:
1. use a combination of relative positioning z-index and pixels, sacrificing responsiveness and diving neck deep into a CSS nightmare 
2. or change the sections order using the **[order]** flexbox propery, which makes things way less complicated. 

You got my choice, right? :D 

Of course this meant that the actual design lost some of its aestethical meaning so a change in the design (again!) was needed. Well, adaptation is a fundamental skill to have in this profession, so I'm glad I had a problem of this kind today. 

Here's the new mockup: 


[details="For a better view: opein it in a new tab then zoom in"]
![day5|55x500](upload://iJ1Kbv572kOqWsyEVhqujOKolw3.png)
[/details]


It was time-consuming but I'm proud of this new design. 

And here's how the actual website looks now (view it full-screen on Codepen)

https://codepen.io/davide2894/pen/OOadxG

### Questions:
1. What do you think?
2. What would you change?
3. Are you interested in taking this challenge yourself?

Let me know!
[/details]

## Day 6 - Friday 01/12/2017

[details="Read"]
5:50 AM - It's already Friday! When did week this pass?? Time sure flies. Yesterday I finally started - though not without issues - to build the website from the mockup I created. The Udacity community gave me some useful feedback on it. Again, without them this project wouldn't be what it is, the design would have a different look.

### Pseudo elements
8:16 AM - I'm having some trouble with the cup image: the HTML can't be touched hence the only way to put the image as per the mockup is via [pseudo elements](https://css-tricks.com/almanac/selectors/a/after-and-before/). The downside of this trick is that is not possible to resize insisde CSS, it must done before anything else. 

With Gimp I can resize easily. Then there are two things to do:
* use the pseudo elements ::after to actually insert the image, specifically
    
    
    h2::after {
        content: url(images/coffee-hot-cup.jpg);
    }
    
    
* use relative positioning to put it at the wanted spot, on the right of "The Beauty of CSS Design"
    
    
    h2::after{
    content: url(images/coffee-hot-cup.jpg);
    margin-left: 3%;
    }
    
Here's the resul:

![Header](app/images/day6.png?raw=true)

### The Road to Enlightment
Time to style the biggest part of the first section.

This looks quite a tough one to do, I'm stuck at the CSS because I don't know how to render the mockup text alignment. Also, I'm still working on making that part of the mockup, the one with coffee beans going down the page, a background image. 
![day6_1|458x500](upload://zMvw3ZMYSAX1Zd7FlLgpdiNiflD.png)

Do you have suggestions on how can I translate the above image into CSS?

Here's the result for today.
https://codepen.io/davide2894/pen/yPGxZr
[/details]


## Day 7 - Saturday 02/12/2017


[details="Read"]
5:37 AM - seventh day for the project. I started yesterday to build the page. 

### Udacity community to the rescue
I asked for feedback to the Udacity community since I was desperate for help and damn if I didn't received it. Both from mentors and fellow students. You are awesome :D .It helped to feel less frustrated over it, to see the problem from another perspective, not as big as I thought it was. All this new info from the community was heading torward the simplest solution: build the background image directly, by using an image editor (and yes, place the little coffee beans one by one). The simplest solution is not always the easiest, right? But I must be careful: I don't want to lose any resolution in this process. The background image is going to be full-screen. Blurred brown dots would not be any good to look at :D

Well, let's see what I can do.

### Paragraphs
To put heading and paragraphs in their exact positions I need to use CSS alignment i.e. the [position property](https://www.w3schools.com/cssref/pr_class_position.asp). More specifically the 
/*position: relative*/ property that allows me to do two important things:
1. move the element arbitrarly but
2. keep it in the document flow ergo the element stays inside its own div and respects the hierachic order.

But there is a problem: it sacrifices responsiveness. I am worried  so I ask my dear friend Google. I find [this hack on God-bless-you Stack Overflow](https://stackoverflow.com/questions/44217169/css-position-relative-with-responsive-height). 
Basically the concept is this: 
* after `position: relative` **use padding instead of the left, right, bottom, top properties normally used in this case**
* use **% instead of pixels** because if you move an element of a specific `px` amount it can't be responsive. But by using % is possible to achieve so as the page will keep its element-page aspect ratio. 

To apply this new learned concept on the website I code the following: 

    
    position: relative;
    height: 0;
    width: 50%;
    padding-left: 20%;
    
![day7_0|690x375](upload://mFK0q3CzKjXofHAnMScW7q7Q4GZ.png)

### The Coffee Road
I struggled but at the end I obtained a decent result. Gimp sure is a difficult program to get comfortable with. Among layers, masks and the myriads of tools, each with its own key shortcut I felt like the new student at school. If you'd like to learn more of Gimp check the [official documentation](https://docs.gimp.org/docs/) (but I warn you, it's quite a long read).

First thing I did was trying to resize the coffee-bean.png file I download from 
[Flaticon](https://www.flaticon.com) only to discover that .png files lose resolution when resized (say what?). So? Turns out that [SVG](https://en.wikipedia.org/wiki/Scalable_Vector_Graphics) files don't lose resolution as they are just XML documents BUT resizing them in any image editor program - such as my fellow Gimp or the likes - isn't so straightforward. Scaling .png and .svg are two completely different processes. 
Then I find [this](https://www.hongkiat.com/blog/resize-export-svg-png-myscale/) simple yet so effective web application that handles the hard work for me and voilà, the trick is done. Now I have at my disposal a small-sized SVG file I can use repeatedly to create the background image I want.

...

And here it is

![day7_1|467x500](upload://gDaCv2e2KqUtG78GcahGsUO7Nga.jpg)

...

While positioning the elements by using the above mentioned CSS trick somenthing bad was happening: the elements were behaving well but the image was not. In fact if I zoomed in or out the latter would stay the same while the former would change font-sizes accordingly, throwing out of the window the meaning of positioning itself. So I had to use the classic CSS alignment at the expense of responsiveness. I don't know how to achieve that but if you happen to know so **please** write it down :disappointed_relieved:

And here we are, I'm not sure about the quality of today's output on the project but anyway 

https://codepen.io/davide2894/pen/JOxEWZ?editors=1100    

For more detailed information, check the [commit I pushed on GitHub](https://github.com/davide2894/css-zen-garden/commit/30113cf8879bbd51a39d7b8521003a2acacddaf6).

Thanks to @vipper_maeglin for suggesting to use transparent background.
[/details]

## Day 8 - Sunday 03/12/2017


[details="Read"]
8:09 AM - Oh well today I woke up later than my preferred time (5:00). When this happened to me in the past the perfectionist in me decided that "well, normally I start to code at 5:30, now it's 8, that's two hours and a half. And since it's so late I lost the momentum, the quiet in the early morning when the world is still sleeping. The entire day is wasted". 

Not this time. I still have the entire morning up until lunch time. Last night, before going to sleep, I also planned to dedicate the afternoon to the Udacity community (forum and Slack channels) and the evening to the blog. As a quote I heard recently said, the time is gonna pass anyway so it's up to me wheter I want to waste the entire day or work for my dream. And I don't even wanna rest "cuz is Sunday!". I don't feel tired, all the opposite. I feel pumped up so let's get going.

### More beans
Yesterday I created the image with the coffee beans going towards the coffee bag. I checked the page now and suddendly I didn't like how short the "coffee road" actually is compared to the one designed in the mockup. All I need to do is to modify the image by making the last part a little bit longer. 

Here it is:
![day8_0|161x500](upload://5LiOPfKje3fvhUEl4aL2yY3GSiR.png)

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

![day8_2|375x500](upload://vzUbHoxoXSkvXaNtDY2MJd6hoOo.JPG)

![day8_3|375x500](upload://9FZdZUX3qDmoJvFvceWlH9S7tiI.JPG)


Here's the work in progress
![day8_4|690x387](upload://fILebc0gmBU6ElPnJUedsl0JBOV.png)

For a more details check my the [commit to GitHub](https://github.com/davide2894/css-zen-garden/commit/feefd4c3ee005c021339b47b9967c14250494e9c)
[/details]

## Day 9 - Monday 04/12/2017


[details="Read"]
5:34 AM - It's a new day, yes it is! *music starts playing* (any WWE fan here?)

Let's continue the work started yesterday with the `.sidebar` section.

### Select a Design
This section is the the second the three. As of yesterday this area of the website was fairly similar to a construction site, after today I hope that it looks better :D

So the first thing to do is the section's layout. Thanks to Flexbox this is achievable without too many headaches. To recap, the desired result is the following: 

![day8_1|335x500](upload://n8cyOyww5dBAfz1mLkhqigPUlqy.png)

**How ?** 

1 - set Flexbox direction to row and enable wrapping

    .wrapper {
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;  
        -webkit-box-orient: horizontal;  
        -webkit-box-direction: normal;  
        -ms-flex-flow: row wrap;  
        flex-flow: row wrap;
        background: url(./images/donut.png) center/contain no-repeat;
        margin-bottom: 10%;
    }
    
    
2 - set the "Select a Design" part to occupy the entire width available on the screen, so that "Archives and "Resources" slip to the second row and both occupy half of the space available.

    .design-selection {
        -webkit-box-flex: 2;
        -ms-flex: 2;
        flex: 2 100%;
        margin-bottom: 5%;
    }
    
    .design-archives,
    .zen-resources {
        -webkit-box-flex: 1;
        -ms-flex: 1;
        flex: 1;
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -webkit-box-orient: vertical;
        -webkit-box-direction: normal;
        -ms-flex-direction: column;
        flex-direction: column;
    }

And that's it! Isn't it amazing? :D

#### Header 
This is easy as I only need to
* fix the `font-size` to make it bigger
* set `font-family` to Lobster as the first font and "cursive" as the fallback, just in case the browser doesn't read the first one
* set the color to `#FDBA55` (a yellow variation)

        select{
        font-size: 6em;
        font-family: "Lobster", cursive;
        color: #FDBA55;
        }

#### Design list box
Besides colors it needs size adjustments:
    
    .design-selection ul {
        width: 28vw;
        height: 48vh;
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -webkit-box-orient: vertical;
        -webkit-box-direction: normal;
        -ms-flex-direction: column;
        flex-direction: column;
        -ms-flex-pack: distribute;
        justify-content: space-around;
        padding: 2%;
        background-color: #333;
        border: 10px solid #fdba55;
        border-radius: 6px;
        margin-bottom: 5%;
    }
    `
    
Now I focus on the single list items, they need some color, a bit of centering and more [font-weight](https://developer.mozilla.org/en-US/docs/Web/CSS/font-weight):
    
    
    .design-selection li {
        font-size: 1.3em;
        color: #fff;
        font-weight: 600;
        margin-left: 10%;
    }
   

I also need to put some space between the name of design and designer. I chose to do so by putting some horizontal margin there:

    
    .design-name{
       margin-right: 1%;
    }
    .designer-name {
       margin-left: 1%;
    }
    
    
Here's the result so far: 
![day9_0|527x500](upload://e1GWzQvbz1x94wASbp6PETLjWWs.png)
Now let's focus on the other two sub-parts of this sections.
 
#### Archives and Resources
The HTML code of these two `div`s are basically the same, meaning they have the same structure, hence they can be customized at the same time by using two selectors together.

For a start let's center them:

    
    .design-archives > *, 
    .zen-resources > * {
        margin: 0 auto;
    }
    
    
What's that? It's a shortcut to select all the elements contained in a class, so simple yet so useful. When I write `.class-name > *` I'm telling CSS "hey, see this class? Do me a favor: go look every single element that you contain and style them as I tell you ". Read more about the [CSS * selector](https://www.w3schools.com/cssref/sel_all.asp).

Then I can give some simple style to the respective titles:

    
    .archives,
    .resources {
        font-size: 3em;
        padding: 0 0 5% 0;
    }
    
    
Increase the size of the characters written in the list items::

    
    .design-archives ul,
    .zen-resources ul {
        font-size: 1.5em;
    }
    
Le's make these two menus look better :) 

Now I want to select each list item - except the last one - in order to do three things:
* put some padding all around it
* put some margin at the bottom so that there is some distance between the end of this section and the next one coming
* put some shadow around the now visible boxes at every list item so that they do not look flat
    
    
    
    .design-archives li:not(last-of-type),
    .zen-resources li:not(last-of-type) {
        margin-bottom: 5%;
        padding: 22px;
        text-align: center;
        -webkit-box-shadow: -2px 5px 2px #333;
        box-shadow: 2px 5px 2px #;
    }
    
    
But it's not enough because there is still a final touch of color to give:

    
    .design-archives li,
    .zen-resources li {
        background: #333333;
        border: 5px solid #FDBA55;
        border-radius: 6px;
    }
    .design-archives {
        border-right: 2px solid #FDBA55;
    }
    
    
    
Here's the result:
![day9_1|690x325](upload://3GLGVLZ8kRRmE52GwywBslHrX5n.png)

#### Donut background
Last part for today. A donut background with a good amount of opacity (i.e. transparency). But how can I edit a background image's opacity inside CSS?? I researched on the internet and found the following possible solutions: 

* [this](https://scotch.io/tutorials/how-to-change-a-css-background-images-opacity)
* [and this](https://stackoverflow.com/questions/4183948/css-set-background-image-with-opacity)

Unfortunately I couldn't make it work in either of these way. I wanted to persist though so after a few headaches I came to the most simple solution: edit the opacity in Gimp. Why do I overcomplicate things so much sometimes? :(

# Website 
The website is now published on GitHub Pages, feel free to check it out :D
https://davide2894.github.io/css-zen-garden/

#### Commit
Lastly, be sure to check out [today's commit](https://github.com/davide2894/css-zen-garden/commit/6f10f6e462ee359e42f005d0f71e850b622af231) as well :D
[/details]

## Day 10 - Tuesday 05/12/2017 

[details="Read"]
5:33 AM - it's a new day, yes it is! It's early morning, the world is still sleeping. There is total quiet now. 

### Main section
This is the third and last part of the mockup I designed though the longest. It is divided in 5 sub-parts that are the following:
1. So What is This About?
2. Participation
3. Benefits
4. Requirements
5. Footer (including the buiscuits splashing in the milk at the very bottom of the page) 

One by one, let's do this.

### So What is This About? 
The goal is to achieve the following look, as per the mockup:

![day10_0|382x500](upload://hKjMHpO1YskIIiy1SnewEaxCOvA.png)

Only thing to change is the border as I think it would be better if it would look like a chocolate square.

The work divided in different areas:
* layout
* font
* colors

Check out the [website](https://davide2894.github.io/css-zen-garden/) to see the result.

For a full-detailed version of changes, check [today's commit](https://github.com/davide2894/css-zen-garden/commit/741655f1c267aaca6fc86ab4cf274e5506d14468)

P.S. Sorry for the short post today, I couldn't stay at the computer all day for personal reasons.
[/details]

## Day 11 - Wednesday 06/12/2017

5:46 AM - we're almost at the middle of December, time sure flies!

Let's get some fun with the project.

### Main section
This is the third and last part of the mockup I designed though the longest. It is divided in 5 sub-parts that are the following:
1. So What is This About?
2. Participation
3. Benefits
4. Requirements
5. Footer (including the buiscuits splashing in the milk at the very bottom of the page) 

Yesterday I did the first one. Let's do the second.

#### Participation
The desired result is the following:
![day11_0|530x500](upload://oTiwAb3oKSNMYHkDRDtKQivm1yE.png)

The first thing I did was to setup Flexbox to handle the layout. Then I worked on the yellow area of this part, specifically I set the dimensions, relative position, text font, color and size. Background color and image, and lastly the padding. 

Below you can see the code

    /*
        --------------------------
            Participation
        --------------------------

    */
    .participation {
        height: 100vh;
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -webkit-box-orient: vertical;
        -webkit-box-direction: normal;
        -ms-flex-direction: column;
        flex-direction: column;
        background: url(images/cupcake.png) no-repeat 88% 80%;
        background-color: #B6D5B3;
    }

    .participation>* {
        max-width: 50%;
        position: relative;
        top: 5vh;
        left: 15vh;
        background: #FEBA55;
        padding: 0 4%;
        z-index: 1;
        -webkit-box-shadow: 0 2px 2px 0px #333;
        box-shadow: 0 2px 2px 0px #333; 
    }
    .participation h3 {
        font-size: 8em;
        padding-top: 4%;
        padding-bottom: 4%;
    }
    .participation p {
        font-size: 1.5em;
        line-height: 1.38;
        letter-spacing: 2px;
        padding-bottom: .5%;
    }
    .participation p:last-of-type {
        padding-bottom: 8%;
    }


#### Benefits

The goal look is the following:
![day11_1|690x467](upload://a8wpUF5bX1rvDCc5qA9VLjCSmXU.jpg)

The work to be done was not so much to be honest. In fact the tasks to do were the following:
* setup Flexbox
* set padding and margins
* decide the font color, size, line height and letter spacing
* position the coffee stain image as per the design mockup
* set background color


    /*
        -----------------------
            Benefits
        -----------------------
    */
    .benefits {
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -webkit-box-orient: vertical;
        -webkit-box-direction: normal;
        -ms-flex-direction: column;
        flex-direction: column;
        padding: 50% 20%;
        background: url(./images/coffe-circle-stain.png) no-repeat 73% 63.4%; 
        background-color: #FFEAC1;
    }
    .benefits>* {
        -ms-flex-item-align: center;
        align-self: center;
    }
    .benefits h3 {
        font-size: 10em;
        letter-spacing: 10px;
        margin-bottom: 10%;
    }
    .benefits p {
        width: 75%;
        font-size: 1.5em;
        letter-spacing: 0.6px;
        line-height: 1.5
    }


#### Requirements
![day11_2|444x500](upload://lSF64sTvURUP6ayL0HitWoMtPQW.png)

The work to do here is for most part the same as above.
One exeption is the line above the last paragraph. I realized by using the [[border-top]] property that can be set as a normal border. 

    /*
    -------------------------
        Requirements
    -------------------------
    */
    .requirements,
    footer {
        background-color: #ffcdb2;
    }
    .requirements {
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -webkit-box-orient: vertical;
        -webkit-box-direction: normal;
        -ms-flex-direction: column;
        flex-direction: column;
        padding: 20% 25%;
    }
    .requirements>* {
        -webkit-box-flex: 1;
        -ms-flex: 1 100%;
        flex: 1 100%;
    }
    .requirements h3 {
        font-size: 12em;
        -ms-flex-item-align: center;
        align-self: center;
        margin-bottom: 16%
    }
    .requirements p {
        width: 146%;
        -ms-flex-item-align: center;
        align-self: center;
        text-align: justify;
        font-size: 2em;
        line-height: 1.5;
        letter-spacing: 2px;
    }
    .requirements p:nth-child(5) {
        margin-bottom: 25%;
    }
    .requirements p:last-of-type {
        border-top: 6px solid #333;
        padding-top: 6%;
    }

I couldn't finish all of the footer today, so the rest will come tomorrow!

***
# Action
See [today's commits](https://github.com/davide2894/css-zen-garden/commits?author=davide2894&since=2017-12-05T23:00:00Z&until=2017-12-06T23:00:00Z) for a more detailed illustration.

Please check the [website](https://davide2894.github.io/css-zen-garden/) and give me your opinion on it 

Please give me your opinion on it, I would be immensely grateful for it.
