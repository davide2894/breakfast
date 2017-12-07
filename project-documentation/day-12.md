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