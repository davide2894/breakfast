## Day 11 - Wednesday 06/12/2017

5:46 AM - we're almost at the middle of December, time sure flies!

Let's get some fun with the project.

### Main section
This is the third and last part of the mockup I designed though the longest. It is divided in 5 sub-parts that are the following:
1. [del]So What is This About?[del]
2. Participation
3. Benefits
4. Requirements
5. Footer (including the buiscuits splashing in the milk at the very bottom of the page) 

Yesterday I did the first one. Let's do the second.

#### Participation
The desired result is the following:
*****************************************************************************
![day11_0](./images/day11_0.png?raw=true)

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
*****************************************************************************************
![day11_1.png](./images/day11_1.png?raw=true)

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
![day11_2](./images/day11_2.png?raw=true)

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

#### Footer 
And here we are at the last area of the page. The result must look like the below
******************************
![day11_3](./images/day11_3.png?raw=true)

I couldn't finish all of the footer today, so the rest will come tomorrow!


##### Action
See [today's commits](https://github.com/davide2894/css-zen-garden/commits?author=davide2894&since=2017-12-05T23:00:00Z&until=2017-12-06T23:00:00Z) for a more detailed illustration.

Please check the website and give me your opinion on it 

Please give me your opinion on it, I would be immensely grateful for it.
