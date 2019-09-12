# IDD-Fa19-Lab1: Blink!

**A lab report by Benjamin Yellin**

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

[Blink Your Way Code](https://github.com/byellin/IDD-Fa18-Lab1/blob/master/BlinkYourWayCode.ino) 

### 2. Blink your LED

**Make a video of your LED blinking, and add it to your lab submission.**

[Blink Your Own Way](https://github.com/byellin/IDD-Fa18-Lab1/blob/master/1e.ino)


## Part D. Manually fade an LED

**a. Are you able to get the LED to glow the whole turning range of the potentiometer? Why or why not?**
[Potentiometer Video](https://github.com/byellin/IDD-Fa18-Lab1/blob/master/Potentiometer.MOV)

## Part E. Fade an LED using Arduino

**a. What do you have to modify to make the code control the circuit you've built on your breadboard?**

To make the LED fade, we had to adjust its brightness over time. When the LED is getting brighter, we increase the brightness. Once the LED reaches its maximum brightness, fadeAmount is negated so that when it is added to brightness, the LED gets less bright. 

**b. What is analogWrite()? How is that different than digitalWrite()?**

digitalWrite has only two states: high and low, while analogWrite can be called on a continuous range of states. 

## Part F. FRANKENLIGHT!!!

### 1. Take apart your electronic device, and draw a schematic of what is inside. 

[Schematic of inside of device](https://github.com/byellin/IDD-Fa18-Lab1/blob/master/1f%20Drawing.JPG)

**a. Is there computation in your device? Where is it? What do you think is happening inside the "computer?"**

There is computation going on inside of this device (a calculator). The computer is storing the inputs from the buttons as binary numbers, and together with the operation specified, triggering signals in particular wires to be fired. The wires that fire correspond to the numbers involved in a computation. 

**b. Are there sensors on your device? How do they work? How is the sensed information conveyed to other portions of the device?**

The sensors in the calculator transmit input from the button into electrical signals. These electrical signals are combined according to the operation specified on the calculator.

**c. How is the device powered? Is there any transformation or regulation of the power? How is that done? What voltages are used throughout the system?**

The device is powered by a battery, and the power from the battery is not regulated by a resistor. The voltage used throughout the system is 1.5V.

**d. Is information stored in your device? Where? How?**

Information is stored in the device by either sending or not sending current through wires. These correspond to the binary representations of digits, where a 1 in a particular place value would correspond to current flowing through a certain wire, and a 0 in a particular place value would correspond to current not flowing through a certain wire. The wires are the light green lines overlaid on the dark green component. 


### 2. Using your schematic, figure out where a good point would be to hijack your device and implant an LED.

Electricity flows from the laptop into the Arduino. Then it flows down the rail on the right and through the resistor. Electricity then passes through the calculator and back into the breadboard. 

### 3. Build your light!

**Make a video showing off your Frankenlight.**

[Frankenlight] (https://github.com/byellin/IDD-Fa18-Lab1/blob/master/Franklight.JPG)

**Include any schematics or photos in your lab write-up.**
