## Day 7 - Saturday 01/12/2017

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
* after /*position: relative*/ **use padding instead of the left, right, bottom, top properties normally used in this case**
* use **% instead of pixels** because if you move an element of a specific /*px*/ amount it can't be responsve. But by using % is possible to achieve so as the page will keep its element-page aspect ratio. 

To apply this new learned concept on the website I code the following: 

    //code 
    position: relative;
    height: 0;
    width: 50%;
    padding-left: 20%;
    
********************************
![day7_0](app/images/day7_0.png?raw=true)
********************************

### The Coffee Road
I struggled but at the end I obtained a decented result. Gimp sure is a difficult program to get comfortable with. Among layers, masks and the miriads of tools, each with its own key shortcut I felt like the new student at school. If you'd like to learn more of Gimp check the [offical documentation](https://docs.gimp.org/docs/) (but I warn you, it's quite a long read).

First thing I did was trying to resize the coffee-bean.png file I download from [Flaticon](https://www.flaticon.com/free-icon/coffee-bean-for-a-coffee-break_31082#term=coffee bean&page=1&position=8) only to discover that .png files lose resolution when resized (say what?). So? Turns out that [SVG](https://en.wikipedia.org/wiki/Scalable_Vector_Graphics) files don't lose resolution as they are just XML documents BUT resizing them in any image editor program - such as my fellow Gimp or the likes - isn't so straight-foward. Scaling .png and .svg are two completely different processes. 
Then I find [this](https://www.hongkiat.com/blog/resize-export-svg-png-myscale/) simple yet so effective web application that handles the hard work for me and voilà, the trick is done. Now I have at my disposal a small-sized SVG file I can use repeatedly to create the background image I want.

...

And here it is

******************************
![day 7](app/images/day7_1.png?raw=true)
*******************************

...

While positioning the elements by using the above mentioned CSS trick somenthing bad was happening: the elements were behaving well but the image was not. In fact if I zoomed in or out the latter would stay the same while the former would change font-sizes accordingly, throwing out of the window the meaning of positioning itself. So I had to use the classic CSS alignment at the expense of responsiveness. I don't know how to achieve that but if you happen to know so **please** :( write it down.


And here we are, I'm not sure about the quality of today's output on the project but anyway 

    //codepen

Thanks to @vipper_maeglin for suggesting to use transparent background.




    



