## Day 6 - Friday 01/12/2017
5:50 AM - It's already Friday! When did this pass?? Time sure flies. Yesterday I finally started - though not without issues - to build the website from the mockup I created. The Udacity community gave me some useful feedback on it. Again, without them this project wouldn't be what it is, the design would have a different look.

### Pseudo elements
8:16 AM - I'm having some trouble with the cup image: the HTML can't be touched hence the only way to put the image as per the mockup is via pseudo elements. The downside of this trick is that is not possible to resize insisde CSS, it must done before anything else. 

With Gimp I can resize easily. Then there are two things to do:
* use the pseudo elements ::after to actually insert the image, specifically
    
    //code
    h2::after {
        content: url(images/coffee-hot-cup.jpg);
    }
    
    
* use relative positioning to put it at the wanted spot, on the right of "The Beauty of CSS Design"
    
    //code
    h2::after{
    content: url(images/coffee-hot-cup.jpg);
    margin-left: 3%;
    }
    
Here's the resul:

![Header](app/images/day6.png?raw=true)

### The Road to Enlightment
Time to style the biggest part of the first section.

This looks quite a tough one to do, I'm stuck at the CSS because I don't know how to render the mockup text alignment. Also, I'm still working on making that part of the mockup, the one with coffee beans going down the page, a background image. 

Here's the result for today.
//img

