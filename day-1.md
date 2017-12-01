# Goal
This project is my humble attempt at the omonym challenge. The interesting part is that the website has the same html, each version is made by customizing only the CSS file! 

[Official source: csszengarden.com](http://www.csszengarden.com)

## Tools used 
* [Brackets](http://brackets.io): text editor
* [Gulp](https://gulpjs.com): task-automation. 
* [official index.html](http://www.csszengarden.com), not to be edited
* [MockFlow](): useful website to build mockups without having to use more complex programs. It's intuitve, no instructions needed :)

## Day 1 - Sunday 26/11/2017
Today I start this new project after finishing [Magic: The Gathering card replica in HTML and CSS](https://github.com/davide2894/Magic-The-Gathering-card-in-HTML-and-CSS).

I downloaded the offical index.html. Then I setup [Gulp](https://gulpjs.com), since this is not the first time I am using it I didn't need to congifure every task from scratch, I just copy-pasted the folder structure and the gulpfile.js from the [portfolio project](https://github.com/davide2894/portfolio).
To learn more about Gulp and how to configure it follow [CSS-Tricks' own guide for beginners ](https://css-tricks.com/gulp-for-beginners/). It's what I used to learn how to make a basic configuration to reduce time-wasting and improve the workflow.

### Reset
The first thing to do is a [reset](https://meyerweb.com/eric/tools/css/reset/) because the optimal result is to have the website behave the same way accross browser. To achieve so I need to avoid inconsistencies by removing default settings inside browsers, such as headings, font-sizes etc.

Since I can't edit in any way the index.html provided I have to modify the gulpfile, so what I need to do is the following:
* delete "sass" task (that compiles any sass file into css)
* edit "watch" task to monitor any change in the "style.css" file
* delete app/js/ folder

Before reset    
[Before reset](app/images/before-reset.png?raw=true)

After reset
[After reset](app/images/after-reset.jpg?raw=true)

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
[Centered Page](app/images/initial-style.png )

Next point now is to come up with my own page design, the main thing to do actually. After researching for a while on [Dribble.com](https://dribbble.com) [this]() caught my eye (I'm particularly fond of split design), I'll be using it as inspiration for the project.
This means I won't use its asset.

As for the color combination, I found [this combo on Pinterest](https://www.pinterest.co.uk/pin/416864509237410284/). It's cool, so let's roll with it.

### Designing the mockup
So far this is going to be the most difficult part of the project. I'm using MockFlow, an intuitive website to build - as the name suggests - website mockups just discovered this morning.










