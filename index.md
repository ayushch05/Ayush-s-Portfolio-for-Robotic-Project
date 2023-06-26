# Ayush's Robotic Arm Smart Car
My project is a smart car with a fan and robotic arm. This project is a combination of the smart rover and the robotic arm. My robotic arm smart car also has a fan that turns on or off based on the temperature of a thermostate assembled on my smart car. My project also has infrared sensors and a thermostat, each for different functionalities. The infrared sensors are placed underneath the rover to detect ground surface within a 5-centimeter range by emitting light waves. The thermostat's function is to measure the room temperature, and based on a certain room temperature, the thermostat sends a signal to arduino controller board to either turn on or off the fan. This is what my rover consists of. 

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Aysuh C | Mountain House High School | Mechatronic Engineering | Incoming Senior

**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**

![Headstone Image](logo.svg)
  
# Final Milestone
For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

# Second Milestone
For your second milestone, explain what you've worked on since your previous milestone. You can highlight:
- Technical details of what you've accomplished and how they contribute to the final goal
- What has been surprising about the project so far
- Previous challenges you faced that you overcame
- What needs to be completed before your final milestone
My second milestone was completing my robotic arm and integrating it with my smart car.

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/y3VAmNlER5Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

# First Milestone
After assembling and setting up all the parts on my rover to create my base project, the first milestone I completed was getting my rover to follow the instructions of my arduino code in order to do basic actions like moving backward, moving forward, and turning towards one direction. I struggled to complete this milestone initially because my rover wouldn’t follow the instructions of my arduino code.
- My problem was that when my rover instructed to move forward, it would rotate very fast in the counterclockwise or clockwise direction. 
- The arduino code was right, so I knew there was nothing wrong with the software part of my rover.
- Each TT motor has a black and red wires attached as a terminal for battery voltage. The voltage flows from the positive terminal of the battery to the negative terminal
- I forgot that my motors are set in the opposite direction, so I also have to make the red and black wire terminals
- This is my arduino code:
```
  void loop() {
    moveForward();
    delay(2000);
    stopMove();
    delay(500);

    moveBackward();
    delay(2000);
    stopMove();
    delay(500);
}
void moveForward() {
    digitalWrite(in1, LOW);
    digitalWrite(in2, HIGH);
    digitalWrite(in3, HIGH);
    digitalWrite(in4, LOW);
}

void moveBackward() {
    digitalWrite(in1, HIGH);
    digitalWrite(in2, LOW);
    digitalWrite(in3, LOW);
    digitalWrite(in4, HIGH);
}
```

- 

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/CaCazFBhYKs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

# Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 

# Code
Here's where you'll put your code. The syntax below places it into a block of code. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize it to your project needs. 

```c++
void setup() {
  // put your setup code here, to run once:
  Serial.begin(9600);
  Serial.println("Hello World!");
}

void loop() {
  // put your main code here, to run repeatedly:

}
```

# Bill of Materials
Here's where you'll list the parts in your project. To add more rows, just copy and paste the example rows below.
Don't forget to place the link of where to buy each component inside the quotation marks in the corresponding row after href =. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize this to your project needs. 

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| Arduino UNO REV3 Microcontroller Board | Used as a motherboard to connect input devices with a power supply and source code to make output devices carry the correct functionality. | $ 28.50 | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
|:--:|:--:|:--:|:--:|
| Motor Drive Controller H Bridge | Used to pick up source code and power supply to move the motors accordingly to the arduino code using jumper cables | $ 6.49 | <a href="https://www.amazon.com/Diymall-Module-Stepper-Modules-Arduino/dp/B00NJOTBOK/ref=sr_1_8crid=3MNMJIM3088O2&keywords=arduino+h+bridge&qid=1687547055&s=electronics&sprefix=arduino+h+bridge%2Celectronics%2C129&sr=1-8"> Link </a> |
|:--:|:--:|:--:|:--:|
| Chassis, and TT Motors, TT Wheels Kit | Contains two motors for each one to be connected to each wheel and a chassis (acrylic plate)  | $9.09 | <a href="https://www.amazon.com/Ardokit-Chassis-Encoder-Battery-Arduino/dp/B00K5OWHXO/ref=sr_1_32?crid=1XXQOORADTDRZ&keywords=acrylic+plate+arduino+car&qid=1687549054&sprefix=acrylic+plate+arduino+car%2Caps%2C130&sr=8-32"> Link </a> |
|:--:|:--:|:--:|:--:|
| PKCELL 9V Battery 1 pc| A power supply with a voltage of 9 volts to power my smart car | $ 7.55 | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6](https://www.amazon.com/PKCELL-Batteries-Alkaline-Detectors-Detector/dp/B0855T49B4/ref=sr_1_23?crid=21BYBZNF2XAL4&keywords=pkcell+battery+9+volt+1pc&qid=1687547725&sprefix=pkcell+battery+9+volt1pc%2Caps%2C137&sr=8-23/"> Link </a> |
|:--:|:--:|:--:|:--:|
| USB Cable| Connects my computer to the Arduino UNO board to trasmit Arduino source code| $ 6.99 | <a href="https://www.amazon.com/DIYmall-Cable-Arduino-2560-Pack/dp/B09JRXT1TY/ref=sr_1_3?crid=1P9JLY2QO6HQJ&keywords=arduino+usb+cable&qid=1687547998&sprefix=arduino+usb+ca%2Caps%2C142&sr=8-3"> Link </a> |
|:--:|:--:|:--:|:--:|
|1'' Universal Wheel 1 pc| Used as additional wheel that can rotate 360 degrees clockwise or counterclockwise, provides support for the two TT wheels, and it set under and behind the two TT wheels  | $1.92 | <a href="https://www.amazon.com/Universal-Casters-Furniture-Trolley-Suitcase/dp/B07HMJ464V/ref=sr_1_5 crid=1HAR0JUZ1O3M6&keywords=1%27%27+universal+wheel&qid=1687548176&sprefix=1%27%27+universal +wheel%2Caps%2C150&sr=8-5"> Link </a> |
|:--:|:--:|:--:|:--:|
| Arduino Jumper Cables | Cables and wires to connect the mini breadboard, Arduino microcontroller board, H bridge, and input devices like IR sensors.  | $ 6.98 | <a href="https://www.amazon.com/Elegoo-EL-CP-004-Multicolored-Breadboard-arduino/dp/B01EV70C78/ref=sr_1_1_sspa?crid=2RWU8S1SQUB7J&keywords=jumper%2Bcables%2Barduino&qid=1687548607&sprefix=jumper%2Bcables%2Barduino%2Caps%2C138&sr=8-1-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&th=1"> Link </a> |
|:--:|:--:|:--:|:--:|
| Hot-glue Gun| Used to glue any parts together using glue sticks | $ 14.99 | <a href="https://www.amazon.com/Gorilla-100426-Full-Size-Glue-Orange/dp/B087418ZDN/ref=sr_1_3?crid=3QJY6NH6HHKIU&keywords=gorilla%2Bglue%2Bgun&qid=1687549371&sprefix=gorilla%2Bglue%2Bgun%2Caps%2C145&sr=8-3&th=1"> Link </a> |
|:--:|:--:|:--:|:--:|
| Gorilla Hot Glue Sticks | Used and inserted into hot glue guns | $9.07 | <a href="https://www.amazon.com/Gorilla-Sticks-Diameter-Count-Clear/dp/B071HH42WW/ref=sr_1_1_sspa?crid=30VY1B5ZI2KQP&keywords=hot%2Bglue%2Bsticks&qid=1687549546&sprefix=hot%2Bglue%2Bsticks%2Caps%2C150&sr=8-1-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&th=1"> Link </a> |
|:--:|:--:|:--:|:--:|
| 200 Popsicle Sticks| Cables and wires to connect the mini breadboard, Arduino microcontroller board, H bridge, and input devices like IR sensors.  | $ 6.98 | <a href="https://www.amazon.com/Sticks-Natural-Popsicle-Length-Crafts/dp/B07F367TCK/ref=sr_1_3?crid=27RXCEJUZ96XU&keywords=200+pc+popsicle+sticks+KTOJOY&qid=1687549910&sprefix=200+pc+popsicle+sticks+ktojoy%2Caps%2C130&sr=8-3"> Link </a> |
|:--:|:--:|:--:|:--:|



# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [Example 1](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/)

To watch the BSE tutorial on how to create a portfolio, click here.
