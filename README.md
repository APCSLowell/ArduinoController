  
Use other features of an Adafruit Circuit Playground as an input device in a Processing program
===============================================================================================
![](CircuitPlaygroundLabeled.jpg)    
In this Arduino lab you will write a program that uses other features of the Adafruit Circuit Playground as an controller for a Processing program. The circuit playground has 16 inputs. Adafruit has a detailed description [here](https://learn.adafruit.com/introducing-circuit-playground/guided-tour). In addition to the light sensor that we used in the previous assignment, the circuit playground also has a:
* Temperature Sensor
* Microphone Audio Sensor
* Motion Sensor
* A 3-axis accelerometer
* Capacitive Touch sensor
* Two large left and right buttons
* Slide switch 

Here's a sample program that will print the values of 16 inputs. Run the program and then press, touch and manipulate the various sensors to see how they work.
```java {.line-numbers}
import processing.serial.*;
import cc.arduino.*;
Arduino arduino;

public void setup() {
  size(100, 100);
  arduino = new Arduino(this, Arduino.list()[0], 57600); //change the [0] to a [1] or [2] etc. if your program doesn't work
}

public void draw() {
  background(192);
  for(int i = 0; i < 16; i++)
    System.out.print(i+" "+arduino.analogRead(i) + "\t");
  System.out.println();
}
```
Write your own program
----------------------
Using the sample program as a guide, write your own program that uses one or more of the inputs. You may find slides 117 - 120 of the [apjavaProcessing slide presentation](https://docs.google.com/presentation/d/1sqbareaFmF9fMcp0XOl3hRO6hAlrU5WIaj4V-Kd3eDI/edit?usp=sharing) helpful. Your program doesn't have to work or look like any other, you can add more features to your previous virtual pet program or create a new one. Have fun and be creative! 

When you are happy with your program, have a friend make a short video of you using your program. The video need only show your hand, the arduino and your program's output, please don't include anyone's face in the video. Convert the video to an animated gif using a free converter like [ezgif.com](https://ezgif.com/). Use ezgif's *cut video* or a similar option to edit your video to under 10 seconds and less than 25MB. Upload your animated gif to your VirtualPet repository. Submit the link to your gif to Google Classroom. Don't forget to click the *Mark as done* button. 

Samples of Student Work
-----------------------
[Jimmy](https://github.com/Jimmy1433223/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Cameron](https://github.com/CaNguyen1/VirtualPet/blob/gh-pages/IMG_6116.GIF)   
[Mikey](https://github.com/miosullivan/ArduinoController/blob/main/ezgif.com-gif-maker%20(1).gif)   
[NaH](https://github.com/MoonNash/VirtualPet/blob/gh-pages/IMG_2876.GIF)   
[Federico](https://github.com/feaprile/ArduinoController/blob/main/ezgif.com-gif-maker%20(1).gif)   
[Koey](https://github.com/koeychan/VirtualPet/blob/gh-pages/ezgif.com-video-to-gif.gif)   
[Kenny](https://github.com/KennyCh13/VirtualPet/blob/gh-pages/Use%20other%20inputs%20of%20an%20Adafruit%20Circuit%20Playground%20in%20a%20Processing%20program.gif)   
[Leah](https://github.com/Lloyd2202/ArduinoController/blob/main/ezgif.com-gif-maker%20(1).gif)   
[Albert](https://github.com/alshi31/VirtualPet/blob/gh-pages/Albert%20Shi's%20Adafruit%20Circuit%20Playground%20GIF.gif)   
[Tiffany](https://github.com/TILOUIE2/VirtualPet/blob/gh-pages/season_gif.gif)   
[Keneth](https://github.com/KenethL/VirtualPet/blob/gh-pages/Arduino%20Game.gif)   
[Pansy](https://github.com/pakuang/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20(1).gif)   
[Johnny](https://github.com/Jlin202/VirtualPet/blob/gh-pages/ezgif-4%20final-b2ff005a7942.gif)   
[Chris](https://github.com/TophTheBro/ArduinoController/blob/main/ezgif.com-gif-maker.gif)   
[Sam](https://github.com/SamRosenblum415/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20(1).gif)   
[Tyler](https://github.com/ty237/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20(3).gif)   


