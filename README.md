# CS-350-10526-M01-Emerging-Sys-Arch-Tech-2026-
CS-350-10526-M01 Emerging Sys Arch &amp; Tech 2026 
Portfolio Piece – Module 8 

Items I chose to showcase: Morse Code State Machine and Temperature and Humidity Sensor System (utilizing QWIIC and 16x2 LCD). Both of these examples allowed me to highlight my technical skills in designing interface code that interacts directly with hardware components, while taking into consideration the limitations of the architecture and ensuring proper timing/measurement as needed for system reliability.

Project Goal Understanding 

In all of the projects throughout this course, we were tasked with building fully functioning systems on our Raspberry Pi’s that allowed us to see software interact with physical components. We used things like LED lights, buttons, and sensors to create reactions and measure inputs. In the Morse Code project, we were tasked with creating a state machine that could output timed signals to our LED light and read inputs from a button. The challenge was creating a timed series of signals (dots and dashes) that would spell out messages while mapping out our code to allow for effective button presses to move through each message. We had to account for timing, thread synchronization, and creating a functional mapping of our messages in the state machine to complete this task. In the Temperature sensor project, we read data from the onboard sensor and output those readings to a temperature display. We connected the sensor to our Raspberry Pi via the I2C interface and used a 1602 LCD screen to display our temperature and humidity readings. This required configuring the hardware components and ensuring we were able to detect the device on the bus, as well as converting and formatting the data to be human-readable on the 16×2 display. We also wanted to toggle between Fahrenheit and Celsius so we added this capability as well.

Problem-solving Focus 

In these projects I demonstrated good problem-solving practices by testing each piece individually before integrating. I tested each GPIO connection without the logic first to make sure our code would recognize each button and LED. I then tested if we were able to detect the I2C device before trying to integrate the display code. Whenever I was running into issues, I tried to look back through the notes and documentation before making any assumptions or guessing. I also took the time to draw out the state mapping for our Morse code example before jumping into writing the code. While this may not have seemed necessary at the time, I feel like this helped me to focus on designing the system before just jumping into implementation.

Things I wish I did 

I would spend more time creating a wiring and/or system diagram before jumping into writing code. While I was able to break down the systems sufficiently to test components one at a time before combining them, I still ran into some issues when merging my code that could have been alleviated or avoided by mapping out the system before starting. I would also make each example more modular in the future by moving reusable pieces of code to their own files and add comments to my code while I develop to help future me understand what I was doing.

Skill Development 

The primary area of skill that I feel was developed throughout this course was my technical support group. I now feel very comfortable navigating hardware documentation and data sheets, communicating over a protocol like I2C, and developing embedded code in Python. In order to complete these projects I learned how to interpret data sheets, use terminal commands to gather system information and troubleshoot problems, troubleshoot I2C communication failures, and utilize GPIO libraries. If something was mentioned that I hadn’t used before, I felt comfortable seeking out those resources on my own to learn how to use them. I also feel much more comfortable looking at architecture choices that were made and trying to understand how and why those decisions impacted the system as a whole.

Future applications 

Many of the skills that were touched on in this course are used every day in a corporate environment. State machines are utilized everywhere, from IoT devices to automation software. We are interfacing components and wiring them together, the same concept we used for our buttons and LEDs. We used timers for our Morse code project which are also common in many places. We troubleshooted communication on the I2C bus. All of these skills can be transferred to many future classes and job positions.

Code Maintainability 

To allow for future students to understand what is happening in my code, I made sure to name my variables appropriately and cleanly separated my hardware load up from the logic of my application. I broke up my code into functional pieces which should prove helpful when making changes or adding to this code. I also left comments to explain some of our timing decisions as well as the general behavior of the code. Separating out the hardware setup from the main runtime logic of our program also allows for users to change or add additional components to this project without needing to dig through the logic of our application to do so.

Overall Thoughts 

I think these projects were a great demonstration of my technical ability with new and emerging systems architectures and technologies. I feel like they also showcase my growth with thinking through how I design and troubleshoot hardware and software working together.
