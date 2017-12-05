## Day 9 - Monday 04/12/2017

5:34 AM - It's a new day, yes it is! *music starts playing* (any WWE fan here?)

Let's continue the work started yesterday with the `.sidebar` section.

### Select a Design
This section is the the second the three. As of yesterday this area of the website was fairly similar to a construction site, after today I hope that it looks better :D

So the first thing to do is the section's layout. Thanks to Flexbox this is achievable without too many headaches. To recap, the desired result is the following: 


![target layout](app/images/day8_1.png);


I can achive doing the following:
1 - set Flexbox direction to row and enable wrapping

    `.wrapper {
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;  
        -webkit-box-orient: horizontal;  
        -webkit-box-direction: normal;  
        -ms-flex-flow: row wrap;  
        flex-flow: row wrap;
        background: url(./images/donut.png) center/contain no-repeat;
        margin-bottom: 10%;
    }`
    
    
2 - set the "Select a Design" part to occupy the entire width available on the screen, so that "Archives and "Resources" slip to the second row and both occupy half of the space available.

    `.design-selection {
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
    }`

And that's it! Isn't it amazing? :D

#### Header 
This is easy as I only need to
* fix the `font-size` to make it bigger
* set `font-family` to Lobster as the first font and "cursive" as the fallback, just in case the browser doesn't read the first one
* set the color to `#FDBA55` (a yellow variation)

`
    font-size: 6em;
    font-family: "Lobster", cursive;
    color: #FDBA55;
`
#### Design list box
Besides colors it needs size adjustments:
    `
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
    
    `
    .design-selection li {
        font-size: 1.3em;
        color: #fff;
        font-weight: 600;
        margin-left: 10%;
    }
    `

I also need to put some space between the name of design and designer. I chose to do so by putting some horizontal margin there:

    `
    .design-name{
    margin-right: 1%;
    }
    .designer-name {
        margin-left: 1%;
    }
    `  
    
Here's the result so far: 
![day9-0](app/images/day9_0)

Now let's focus on the other two sub-parts of this sections.
 
#### Archives and Resources
The HTML code of these two `div`s are basically the same, meaning they have the same structure, hence they can be customized at the same time by using two selectors together.

For a start let's center them:

    `
    .design-archives > *, 
    .zen-resources > * {
        margin: 0 auto;
    }
    `
    
What's that? It's a shortcut to select all the elements contained in a class, so simple yet so useful. When I write `.class-name > *` I'm telling CSS "hey, see this class? Do me a favor: go look every single element that you contain and style them as I tell you ". Read more about the [CSS * selector](https://www.w3schools.com/cssref/sel_all.asp).

Then I can give some simple style to the respective titles:

    `
    .archives,
    .resources {
        font-size: 3em;
        padding: 0 0 5% 0;
    }
    `
    
Increase the size of the characters written in the list items::

    `
    .design-archives ul,
    .zen-resources ul {
        font-size: 1.5em;
    }
    `
Le's make these two menus look better :) 

Now I want to select each list item - except the last one - in order to do three things:
* put some padding all around it
* put some margin at the bottom so that there is some distance between the end of this section and the next one coming
* put some shadow around the now visible boxes at every list item so that they do not look flat
    
    
    `
    .design-archives li:not(last-of-type),
    .zen-resources li:not(last-of-type) {
        margin-bottom: 5%;
        padding: 22px;
        text-align: center;
        -webkit-box-shadow: -2px 5px 2px #333;
        box-shadow: 2px 5px 2px #;
    }
    `
    
But it's not enough because there is still a final touch of color to give:

    `
    .design-archives li,
    .zen-resources li {
        background: #333333;
        border: 5px solid #FDBA55;
        border-radius: 6px;
    }
    .design-archives {
        border-right: 2px solid #FDBA55;
    }
    `
    
    
Here's the result:
![archives and resources](app/images/day9_1.png)


#### Donut background
Last part for today. A donut background with a good amount of opacity (i.e. transparency). But how can I edit a background image's opacity inside CSS?? I researched on the internet and found the following possible solutions: 

*[this](https://scotch.io/tutorials/how-to-change-a-css-background-images-opacity)
*[and this](https://stackoverflow.com/questions/4183948/css-set-background-image-with-opacity)

Unfortunately I couldn't make it work in either of these way. I wanted to persist though so after a few headaches I came to the most simple solution: edit the opacity in Gimp. Why do I overcomplicate things so much sometimes? :(

#### Website 
The website is now published on GitHub Pages, feel free to check it out :D
https://davide2894.github.io/css-zen-garden/

#### Commit
Lastly, be sure to check out [today's commit](https://github.com/davide2894/css-zen-garden/commit/6f10f6e462ee359e42f005d0f71e850b622af231) as well :D
