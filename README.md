# IDD-Fa19-Lab1: Blink!

**A lab report by John Q. Student**

**Fork** this repository to get a template for Lab 1 for *Developing and Designing Interactive Devices* at Cornell Tech, Fall 2019. You should modify this `README.md` file to delete this paragraph and update below. As the lab asks:

> Include your responses to the bold questions on your own fork of the lab activities. Include snippets of code that explain what you did. Deliverables are due next Tuesday. Post your lab reports as `README.md` pages on your GitHub, and post a link to that on your main class hub page.

We've copied the questions from the lab here. Answer them below!

## Part A. Set Up a Breadboard

![image](https://github.com/byellin/IDD-Fa18-Lab1/blob/master/Breadboard%20Image.JPG)

## Part B. Manually Blink a LED

**a. What color stripes are on a 100 Ohm resistor?**
 
A 100 ohm resistor has blue and red stripes on it. 
 
**b. What do you have to do to light your LED?**

b.	The LED went on by itself when I plugged in the breadboard.

## Part C. Blink a LED using Arduino

### 1. Blink the on-board LED

**a. What line(s) of code do you need to change to make the LED blink (like, at all)?**

To make the LED blink, we did not have to change the original version of the code. 

**b. What line(s) of code do you need to change to change the rate of blinking?**

To change the rate of blinking, we had to change the parameters of the delay() function. By making the parameter lower, we increase the rate of the blinking.

**c. What circuit element would you want to add to protect the board and external LED?**
 
A resistor would control the flow of electricity and the circuit and prevent it from getting overloaded.
 
**d. At what delay can you no longer *perceive* the LED blinking? How can you prove to yourself that it is, in fact, still blinking?**

Once the delay parameter is below or equal to 15, I can no longer perceive that the LED is flashing. 

**e. Modify the code to make your LED blink your way. Save your new blink code to your lab 1 repository, with a link on the README.md.**

[Blink Your Own Way](https://github.com/byellin/IDD-Fa18-Lab1/blob/master/1e.ino).

### 2. Blink your LED

**Make a video of your LED blinking, and add it to your lab submission.**

[link to your video here; feel free to upload to youtube and just paste in a link here]


## Part D. Manually fade an LED

**a. Are you able to get the LED to glow the whole turning range of the potentiometer? Why or why not?**


## Part E. Fade an LED using Arduino

**a. What do you have to modify to make the code control the circuit you've built on your breadboard?**

**b. What is analogWrite()? How is that different than digitalWrite()?**


## Part F. FRANKENLIGHT!!!

### 1. Take apart your electronic device, and draw a schematic of what is inside. 

**a. Is there computation in your device? Where is it? What do you think is happening inside the "computer?"**

**b. Are there sensors on your device? How do they work? How is the sensed information conveyed to other portions of the device?**

**c. How is the device powered? Is there any transformation or regulation of the power? How is that done? What voltages are used throughout the system?**

**d. Is information stored in your device? Where? How?**

### 2. Using your schematic, figure out where a good point would be to hijack your device and implant an LED.

**Describe what you did here.**

### 3. Build your light!

**Make a video showing off your Frankenlight.**

**Include any schematics or photos in your lab write-up.**
