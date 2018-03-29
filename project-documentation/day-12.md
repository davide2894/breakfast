## Day 12 - Thursday 07/12/2017
6:03 AM - today I have the goal for the project is to finish the page. Let's go.

### Main section
Remember, we are one the third and last area of the page that is composed by the following parts:
1. So What is This About?
2. Participation
3. Benefits
4. Requirements
5. Footer (including the buiscuits splashing in the milk at the very bottom of the page) 

The fifth is the last to do, I began it yesterday so let's finish it today!

#### Footer 
Remember, the goal look is the following:
******************************
![day11_3](./images/day11_3.png?raw=true)

So far I'v set background color to pink, the text color to #333, the font to "Lobster", centerd it all and put some considerable padding-bottom to make the whole part longer. This way splashing cookies effect will become good.

Now I have to create the image that will be on the background, for this I will use Gimp. The overall process is easy and short, as you can see from the code.

    /*
        --------------------------
                Footer
        --------------------------
    */
    footer {
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -webkit-box-pack: center;
        -ms-flex-pack: center;
        justify-content: space-around;
        padding: 200% 20% 0 20%;
        border: 1px solid black;
    }
    footer a {
        text-decoration: none;
        color: #333;
        text-transform: lowercase;
        font-size: 6em;

    }
    footer {
        background: url(images/footer-cookies-in-milk.png) bottom no-repeat;
        background-color: #ffcdb2;
    }

### Details
Details make the difference between an averange and excellent product. It's the last but toughest work to do. The keys are the following:
* anchor styling
* make the site responsive

#### Anchor Styling
Well, the default style of anchor links is quite ugly. I thought it would be better to improve it a little bit. Only in this case I didn't use the mockup as a guide because, in the designing phase, I didn't make the links. That was on purpose as I was sure I would eventually come up with an idea :D.

So the general principle I followed for links was for them to be clean, not invasive. A color change and increase in font-weight, along with underline does the trick. 

Below you can check the code.

/*
    ----------------------------
    ----------------------------
            LINKS
    ----------------------------
    ----------------------------
*/
.summary a {
    color: #3a170d;
}
.summary a:hover {
    color: black;
}
.design-selection li {
    color: gray;
}
.design-selection a {
    text-decoration: underline;
}
.design-selection a:hover,
.design-archives a:hover,
.zen-resources a:hover {
    color: #FEBA55;
    font-weight: 600;
}
.design-selection a:hover {
    font-size: 1.05em;
}
.participation a {
    color: #333;
}
.participation a:hover,
.requirements a:hover,
footer a:hover {
    color: #000;
    font-weight: 500;
}
.requirements a {
    color: #333;   
}

.page-wrapper > a {
    -webkit-transition: 0.1s easy-in-out;
    transition: 0.1s easy-in-out;
}

As you can see, I set a minimal [transition](https://developer.mozilla.org/en-US/docs/Web/CSS/transition-property) rule. My goal in this case is simple: make the color and [[[[[[[font-weight]]]]]]]]]]]] change smoother.

##### Action
See [today's commits](https://github.com/davide2894/css-zen-garden/commits?author=davide2894&since=2017-12-05T23:00:00Z&until=2017-12-06T23:00:00Z) for a more detailed illustration.

Please check the website and give me your opinion on it 

Please give me your opinion on it, I would be immensely grateful for it.

# Announcement 
Responsiveness is the very last thing to do with this website. As we are now in December, I prefer to finish the course first. The reasons are the following:
* I want to complete one of the challenge requirements BUT I want to do it with excellence. This means that I may need additional time for fixing/editing of quizzes and, highly propable, for the last project
* Once I complete the course I can keep working on my personal projects and participate in the community (the latter won't be put on hold during course completion)

In other words, this project will be on hold for some time, probably a couple of weeks. I hope to come back at it as soon as I can. Still, quality of course completion has priority now. 

Thank you for the support given until now! :D 



