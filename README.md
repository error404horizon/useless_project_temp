<img width="1280" height="640" alt="git (1)" src="https://github.com/user-attachments/assets/8920b256-2ba8-4988-b824-5351134eb4bd" />



# Alarming Alarm ⏰


## Basic Details
### Team Name: Never Call Saul


### Team Members
- Member 1: Akash Krishnan U - Model Engineering College 
- Member 2: Aldrin Baiju - Model Engineering College 

### Project Description
 The project is about an alarm that turns off in a funny manner

### The Problem (that doesn't exist)
In our life we've always abused the use of the "snooze" button of alarms, extending the waking time and ending up sleeping more time than usual.

### The Solution (that nobody asked for)
This project aims to completely eliminate the snooze button by introducing a dismissing button that turns it off by pure luck

## Technical Details

The Alarming Alarm is an ESP32-based embedded system that combines real-time clock functionality, random number generation, an LCD display, and an annoying buzzer mechanism to create a deliberately useless alarm system.

### Working Principle

- The ESP32 acts as the main microcontroller and controls all peripherals.
- The DS3231 RTC module provides accurate timekeeping and is used to trigger the alarm at the configured time.
- A 16×2 I2C LCD displays the current time, alarm status, generated random number, and system messages.
- A push button is used by the user to attempt to dismiss the alarm.
- Every button press generates a random number from 1 to 50.
- The numbers are divided into **five ranges of 10 numbers each**, with each range assigned a different buzzer frequency.
- Five numbers out of 50 act as lucky dismissal numbers.
- If a lucky number is generated, the alarm is turned off.
- Otherwise, the alarm continues and the buzzer frequency changes according to the generated number.

### Technologies/Components Used
For Software:
- Languages used: C++, JS, HTML,CSS
- Applications used: Arduino IDE, VS code, Firebase 
- Simulation: https://wokwi.com/

For Hardware:
Resistors - 1k,10k ohm, Jumper wires, Push button, Buzzer, LCD, RTC module, ESP32, connecting USBs

### Implementation
A random number generator is set up which chooses a number between 1 and 50 every time you push the button. Each 10 number intervals is mapped to a certain annoying buzzer frequency, and so are each "dismissing" numbers. So in short, you have a 5 in 50 chance to turn off the alarm, or a grand possibility of 1/10

# Screenshots (Add at least 3)
![Screenshot1](assets/screenshots/Screenshot%202026-09-04%20055047.png)


![Screenshot2](assets/screenshots/Screenshot%202026-09-04%20055219.png)


![Screenshot3](assets/screenshots/WhatsApp%20Image%202026-09-04%20at%206.39.16%20AM.jpeg)

# Schematic & Circuit
![Circuit](assets/screenshots/WhatsApp%20Image%202026-09-04%20at%205.59.52%20AM.jpeg)
*The circuit shows the complete hardware architecture of the Alarming Alarm. The ESP32 serves as the main controller, interfacing with the DS3231 RTC and 16×2 I2C LCD through the I2C bus. The RTC provides accurate timekeeping, while the LCD displays the alarm status and generated numbers. A push button connected to a digital GPIO is used to generate a new random number, and the passive buzzer produces different frequencies based on the generated number. Together, these components implement the random-number-based alarm dismissal mechanism.*

![Schematic](assets/screenshots/Screenshot%202026-09-04%20055131.png)

# Build Photos

## Final Product

![Final Product](assets/screenshots/WhatsApp%20Image%202026-09-04%20at%206.45.58%20AM.jpeg)
*The final Alarming Alarm prototype.*

# Project Demo
## Video

[🎥 Watch the Alarming Alarm Demo](https://drive.google.com/file/d/10BJ9cb-xXH3knYk9JTLaL4JBsSJlJ3Ed/view?usp=drive_link)

*The video demonstrates the working of the Alarming Alarm.*


---
Made with ❤️ at TinkerHub Useless Projects 

![Static Badge](https://img.shields.io/badge/TinkerHub-24?color=%23000000&link=https%3A%2F%2Fwww.tinkerhub.org%2F)
![Static Badge](https://img.shields.io/badge/UselessProjects--26-26?link=https%3A%2F%2Ftinkerhub.org%2Fevents%2F1M8ORET9A1%2Fuseless-projects-3.0)
