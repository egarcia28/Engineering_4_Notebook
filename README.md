# Engineering_4_Notebook

&nbsp;

## Table of Contents
* [Launchpad 1](#Raspberry_Pi_Launchpad_1)
* [Launchpad 2](#Raspberry_Pi_Launchpad_2)
* [Launchpad 3](#Raspberry_Pi_Launchpad_3)
* [Launchpad 4](#Raspberry_Pi_Launchpad_4)
* [Crash Avoidance 1](#Raspberry_Pi_Crash_Avoidance_1)
* [Crash Avoidance 2](#Raspberry_Pi_Crash_Avoidance_2)
* [Crash Avoidance 3](#Raspberry_Pi_Crash_Avoidance_3)
* [Onshape_Beam_Part 1](#Onshape_Beam_Part1)
* [Onshape_Beam_Part 2](#Onshape_Beam_Part2)
* [Onshape_Beam_Part 3](#Onshape_Beam_Part3)
* [Landing Area 1](#Raspberry_Pi_Landing_Area_1)
* [Landing Area 2](#Raspberry_Pi_Landing_Area_2)
* [Morse Code 1](#Raspberry_Pi_Morse_Code_1)
* [Morse Code 2](#Raspberry_Pi_Morse_Code_2)
* [Data Storage](#Raspberry_Pi_Data_Storage_1)
* [Data Storage 2](#Raspberry_Pi_Data_Storage_2)

&nbsp;

## Raspberry_Pi_Launchpad_1

### Assignment Description

For this assignment we were tasked with creating a countdown from 10 that displayed on the serial moniter, at the end of the countdown, LIFTOFF should be printed.

### Evidence 

![Evidence_launchpad1](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/266376856-d6981811-ca07-442e-838a-f10ebdc2a6cd.gif)

### Code

[My code is here](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/launchpad_1.py)

### Reflection

This was my first time coding in circuit python in a while, and my first time using the pico, so I was bound to run into issues. Thankfully, they were all relatively minor and I was able to figure them out. I had some trouble with the new file organization of the picos, I was trying to run code from a new vs code file, but learned that in order to run code on the picos, you have to use the code.py file found on the actual pico drive. I also had some trouble remembering how to use "for" loops, but after reading over [this site](https://www.w3schools.com/python/gloss_python_for_range.asp) I was able to remember when, and how to use them to help me finish this assignment. 

&nbsp;

## Raspberry_Pi_Launchpad_2

### Assignment Description

For this assignment we built upon [launchpad_1](#Raspberry_Pi_Launchpad_1) where we coded a countdown for a lauchpad, and added 2 LEDs to it. One red LED to blink as it counted down, and one green LED to signify liftoff.

### Evidence 

![Evidence_launchpad2](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/266664910-ea34df20-a0a2-4264-a263-71d09dffac38.gif)

### Wiring

![Wiring_launchpad2](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/IMG-2678.jpg)

### Code

[My code is here](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/launchpad_2.py)

### Reflection
I ran into very few issues while coding this portion of the assignment, and the issues I did encounter were very minor. For example, I had trouble with how to wire the pico, I had the wiring diagram reversed in relation to my board. Another issue I had was forgetting to use ctrl + c to stop running the uploaded code, because I had a loop at the end of my code, it ran indefinitely and prevented me from uploading new code and making changes. All together, it was a relatively quick addition to the previous sections.


&nbsp;

## Raspberry_Pi_Launchpad_3

### Assignment Description

For this assignment we built upon [launchpad_1](#Raspberry_Pi_Launchpad_1) and [2](#Raspberry_Pi_Launchpad_2) where we coded a countdown and 2 LEDs for a launchpad. For this portion we added a button to signal the beginning of the countdown.

### Evidence 

![Evidence_launchpad3](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/266645327-fbb3ac5c-5c73-4c47-8530-02ba06b33c33.gif)

### Wiring

![Wiring_launchpad3](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/IMG-2679.jpg)

### Code

[My code is here](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/launchpad_3.py)

### Reflection
During this section, we modified our code in order to start the countdown when a button was pressed. Although I diddn't  run into any major issues during this portion, I did learn alot of useful information about the picos, their logic systems, and how to effectively wire them. For example, unlike boards we have used in the past, they have an internal pull down resistors, this means that the board is able to do much of the wiring for us. Rather than use an external resistor to wire a button, we can use simply one wire to ground and one to 3v. Although this assignment went pretty quickly, I still feel like I learned alot that will be very useful later in the year.


&nbsp;

## Raspberry_Pi_Launchpad_4

### Assignment Description

For this assignment we built upon [launchpad_1](#Raspberry_Pi_Launchpad_1), [2](#Raspberry_Pi_Launchpad_2), and [3](#Raspberry_Pi_Launchpad_3)where we coded a a button and LEDs to signal a countdown for a launchpad. For this section, we added a servo that would rotate 180&deg; when the countdown reached 0, or liftoff began.
### Evidence 

![Evidence_launchpad4](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/ezgif-3-d803740028.gif)

### Wiring

![Wiring_launchpad4](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/IMG-2680.jpg)

### Code

[My code is here](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/launchpad_4.py)

### Reflection
In this section of the launchpad assignment, we added a servo to the existing code and wiring. Although it was really only  a few lines of code, it was a really good refresher as to how to code servos, and their interactions with other physical and code components. The process of wiring the servo was also relatively straightforward, although I did learn that you need to be very careful when working with 5v on the picos, they have no short-protection, so if you mistake ground and 5v you can easily fry the board.

&nbsp;

## Raspberry_Pi_Crash_Avoidance_1

### Assignment Description

For this assignment we were tasked with linking an accelerometer with the pico using i2c, we were then able to take values for x, y, and z acceleration and print them on the serial moniter.

### Evidence 

![Evidence Accelerometer1](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/ezgif-1-9ddb8fe37b.gif)

### Wiring

![Wiring_Accelerometer1](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/Accelerometer1%20wiring.jpg)

### Code

[My code is here](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/accelerometer.py)

### Reflection
For this assignment I learned quite a lot about I2C devices, and how to use "F strings". Despite the fact that I have used I2C devices before, I have never used them on the pico's so, the setup was quite different, especially since we were initializing it to be compatible with 2 I2C devices on the same pins, namely the OLED screens which we will be adding in the future. Another useful python feature I learned while working through this assignment was how to use "F strings", F strings are a way of printing formated variables in python. [This](https://www.freecodecamp.org/news/python-f-strings-tutorial-how-to-use-f-strings-for-string-formatting/) website was incredibly useful in learning how to effectively use F strings.

&nbsp;

## Raspberry_Pi_Crash_Avoidance_2

### Assignment Description

On this assignment we built upon the previous crash avoidance system by adding a light which indicates when the accelerometer has been rotated 90&deg;, we also added a external LIPO battery.

### Evidence 

![Evidence Accelerometer2](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/accelerometer2.gif)

### Wiring

![Wiring_Accelerometer2](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/Accelerometer2%20wiring.jpg)

### Code

[My code is here](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/accelerometer2.py)

### Reflection

During this assignment I mostly dealt with concepts I was very familliar with, such as LEDs and wiring external power, but I was able to expand upon my knowledge with these in a way that logically added the next step to the current crash detection. Another new python feature I learned how to use was ``` :.3f``` in order to limit the number of decimals printed. Although this wasnt strictly part of this assignment, it made my output alot neater, and I knew it was a required aspect of the next assignment.  Lots of thanks to [Pinocchio](https://en.wikipedia.org/wiki/Pinocchio?scrlybrkr=973947e4) for help with the wiring on this assignment, at first I found it quite complicated, but he clearly explained it to me.

&nbsp;

## Raspberry_Pi_Crash_Avoidance_3

### Assignment Description

For this assignment we expanded both our crash avoidance systems as well as our knowledge of I2C devices by adding a OLED screen to our system that would display values of angular velocity for x,y, and z.

### Evidence 

![Evidence Accelerometer3](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/accelerometer3.gif)

### Wiring

![Wiring_Accelerometer3](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/Accelerometer3.jpg)

### Code

[My code is here](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/accelerometer3.py)

### Reflection

This assignment was the first time I had used an OLED screen, so it brought with it it's own set of challenges, at first I was unable to locate the I2C address of the OLED, this was because I was using 3V3 EN to power my OLED and accelerometer. This was a problem because 3V3 EN is a pin to help debug the pico, and while it does ouput power for some uses ( which is why my accelerometer worked fine ) it does not work to power multiple devices. Another problem I ran into was setting up and printing the angular velocity on the OLED, because it was a new format, I was not used to printing on the OLED and had to re-read the assignment several times.

&nbsp;

## Onshape_Beam_Part1

### Assignment Description

This was the first section of our beam assignment, the goal being to design and mock up a beam that could hold as much weight ( 180mm from the lever point ) as possible without snapping or excessive deflecting, while maintaining a weight below 13g.

### Part Link 

[Link to our Onshape document](https://cvilleschools.onshape.com/documents/bbb8fb04f2c7e9a26ef00d6f/w/8353d61f44a10197441fa346/e/12a872e8fa7823561546f9c6)

### Part Image

![Beam Image](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/beam.PNG)

### Reflection
Like many other groups, we began by reasearching [beam theory](https://en.wikipedia.org/wiki/Euler%E2%80%93Bernoulli_beam_theory#:~:text=Euler%E2%80%93Bernoulli%20beam%20theory%20), a study of how load bearing beams behave elastically and deflect. We then looked into succesful cantilever beam designs, as well as commonplace beam designs that are very prevalent, such as I-Beams ( simillar to the design we ended up going with ). We then began to design our beam using ideas we had gathered, an I-Beam adjacent design with a strong load bearing top section with 45&deg; chamfers to increase strength and printability constraints of the assignment. Other strategic design choices we made include, a thin middle section, as well as holes along the middle and bottom, to reduce mass on a relatively low load bearing components. We also had to make sure that there were no vertical angles above 45&deg; as that was one of our design constraints due to the printer only being able to print up to 45&deg;. Lots of thanks to [Komaram Bheem](https://en.wikipedia.org/wiki/Komaram_Bheem?scrlybrkr=973947e4) for help with the pronunciation and etymology of his name, as well as help with certain aspects of our design.

&nbsp;

## Onshape_Beam_Part2

### Assignment Description
For this assignment we built upon our first beam design using Onshape's built in FEA analysis software to determine areas of high stress and displacement in order to edit our design to account for these flaws in our first design.

### Part Link 

[Link to our Onshape document](https://cvilleschools.onshape.com/documents/bbb8fb04f2c7e9a26ef00d6f/w/8353d61f44a10197441fa346/e/12a872e8fa7823561546f9c6)

### Part Image
_All simulations tested with 30N of force_
![Beam Stress](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/stress.PNG)
_FEA sim of stress -- Max stress around 80MPa_

![Beam Safety](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/saftey.PNG)
_FEA sim of safety factor -- Min around .4_

![Beam Displacement](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/displace.PNG)
_FEA sim of displacement -- Max around 50mm_

### Reflection
After running the FEA simulation for our initial beam design, we were able to visualise the areas of our beam under the most stress as well as areas most likely to break. As shown in the above images, the part of the top rail nearest the base, as well as the area nearest the weight seem to be the areas under the most stress. In order to strengthen these parts and better distribute the stress, we will be removing material from areas with the littlest stress and adding it to these areas. For example, we could remove material from the center of the upper rail as well as the area closest to the weight under the least stress and add it to the areas described above. The FEA simulation tools in onshape are relatively complete and fairly simple to use, so after running through the short training activities I felt like I had a good grasp on the simulation tools, although, when first testing our beam, we diddn't add a bearing face, so we got unrealistic results (we were able hold >20 lbs of force), but once we fixed that we were able to easily analyze the forces acting on our beam.

&nbsp;

## Onshape_Beam_Part3

### Assignment Description
For this section of the beam assignment we first improved our design based on the Onshape FEA simulation, and then tested the improved design in the real world giving us much more accurate results allowing us to iterate on our design once again with accurate, real world data.

### Part Link 

[Link to our Onshape document](https://cvilleschools.onshape.com/documents/bbb8fb04f2c7e9a26ef00d6f/w/8353d61f44a10197441fa346/e/12a872e8fa7823561546f9c6)

### Part Image

![Beam2 Stress](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/stress%202.png)
_FEA sim of stress 2nd iteration (MPa)_

![Beam3 Stress](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/stress%203.png)
_FEA sim of stress 3rd iteration (MPa)_

![Beam2 Displacement](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/displacement%202.png)
_FEA sim of displacement 2nd iteration_

![Beam3 Displacement](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/displacement%203.png)
_FEA sim of displacement 3rd iteration_


### Reflection
When it came to improving our design based on our first FEA simulation, we just added some simple changes to better distribute the stress. These changes include, removing material from the sides by connecting the holes together, and adding that material to the top rail near the base and weight through some simple chamfers and extrusions. When we tested this in the real world we did pretty well and held a decent ammount of weight, but our beam ultimately broke due to the lack of support on the sides created by the singular long hole, causing it to bend sideways and break much quicker. When we went back to Onshape to improve our design from the real world results, we re-connected all of the holes to add support and prevent the beam from twisting, we also added a secondary rail on the top in order to better distribute the stress. When testing our 3rd iteration in the real world it held much more weight and diddn't twist, when it finally broke it shattered showing that we had done a pretty good job of distributing the stress.  

&nbsp;

## Raspberry_Pi_Landing_Area_1
### Assignment Description
For this assignment we were tasked with writing a program that would take user input for 3 ordered pairs, and then calculate and display the area of the triangle they created using functions.
### Evidence 
![Evidence Landing Area 1](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/landingarea1.gif)
### Code
[My code is here](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/raspberry-pi/landing_area_1.py)
### Reflection
This was  helpful learning experience as I had never used the REPL to input values for a program, as well as functions to formulate an output based on the inputs given. I did run into some trouble at first because I mixed up the naming conventions I had set for each set of ordered pairs but after careful exxamination I figured it out relatively quickly. Due to this being an entirely PICO contained assignment, there wasn't any wiring to throw me off, and any errors I encountered stemmed from my own incompetence, but I eventually got my program up and running.
&nbsp;

## Raspberry_Pi_Landing_Area_2
### Assignment Description
For this assignment, we built upon the program we coded for [Landing Area 1](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/README.md#raspberry_pi_landing_area_1) by adding an OLED screen and displaying the triangle input, plotted onto the OLED.
### Evidence 
![Evidence lLanding Area 2](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/landingarea2.gif)
### Wiring
![Wiring_Landing Area 2](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/landingareawiring.jpg)
### Code
[My code is here](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/raspberry-pi/landing_area_2.py)

### Reflection
Because we had used the OLED screens in a [prevoius assignment](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/README.md#raspberry_pi_landing_area_1), I already felt somewhat confident in their use, one difference from the prevous assignment was that we only had to accoount for one I2C device in our code which pared down alot of the confusion I had surrounding the OLED before. Another thing I had trouble with was figuring out how to display the axes and triangle on the OLED, but after some troubleshooting and re-reading the instructions I was able to better understand the shape libraries.

&nbsp;
## Raspberry_Pi_Morse_Code_1
### Assignment Description
For this assignment we created a relatively simple program where a message of the users choice was input, and in return, the program translated it into morse code.
### Evidence 
![Evidence Morse Code 1](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/morsecode1.gif)

### Code
[My code is here](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/raspberry-pi/morse_code_1.py)

### Reflection
Although this was a technically easy assignment, I had some trouble with creating the logic portions of the program. For example, this for loop '''for x in range(len(string))'''  caused some confusion as I had never worked this in depth with strings in python before, but once I learned some new syntax (to me) for string functions (like "len()") the logic portion of this assignment went pretty fast. One really "cool trick" I used for this assignment was editing the morse code dictionary in order to add a "/" at every instance of a space. 

&nbsp;

## Raspberry_Pi_Morse_Code_2
### Assignment Description
In this asssignment we built upon [morse code 1](https://github.com/egarcia28/Engineering_4_Notebook#Raspberry_Pi_Morse_Code_1) by bringing our previously, exclusively digital program into the real world, and wiring a LED to display the morse code messages input by the user.
### Evidence 
![Evidence Morse Code 2](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/morsecode2.gif)
### Wiring
![Wiring Morse Code 2](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/morsecode2wiring.jpg)
### Code
[My code is here](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/raspberry-pi/morse_code_2.py)
### Reflection
This was a relatively easy transition from the purely digital program to a physical morse code translator, but it was still really fun nonetheless. I had some minor trouble with the new timings and their names for the LED, but it was pretty self explanitory and I was quickly able to correctly assign each timing to its appropriate delay. 

&nbsp;

## Raspberry_Pi_Data_Storage_1
### Assignment Description
In this assignment, we were tasked with taking the basis from [a previous assignment](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/Accelerometer2%20wiring.jpg) and adding several things to it in order to record the data captured by the accelepometer.
### Evidence 
![Evidence Data_Storage_CSV_File](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/raspberry-pi/data.csv)
### Wiring
![Wiring Data Storage](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/Accelerometer2%20wiring.jpg)
### Code
[My code is here](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/raspberry-pi/data_storage.py)

### Reflection
This was a very confusing assignment, and I had a lot of trouble with the really finicky aspects of the data modes and features. One such issue was keeping track of the data.csv file as well as recognizing which mode I was in while recording data or uploading code. On the code front, one issue I encountered was was the odering of statements within the '''while''' loop.

&nbsp;
## Raspberry_Pi_Data_Storage_2
### Assignment Description
In this assignment, we were tasked with taking the data we recorded in the prrevoius assignment, and using google sheets to plot and analyze it.
### Evidence 
![Evidence Data_Storage accel graph](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/data%20storage%20graph.PNG)
Graph of accelerometers acceleration_
![Evidence Data_Storage tilt graph](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/images/tilt%20data%20storage%20graph.PNG)
_Graph of the accelerometers tilt_
### Code
[My code is here](https://github.com/egarcia28/Engineering_4_Notebook/blob/main/raspberry-pi/data_storage.py)

### Reflection
Although this was more of a tutorial than an actual assignment, I did feel like it not only was a very interesting way of looking at data, but also I feel like this knowledge will become very useful when we eventually need to recoord and analyze data collected by our pi in the sky project.

&nbsp;
