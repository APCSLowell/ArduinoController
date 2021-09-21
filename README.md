  
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
[Zoey](https://github.com/zoeyzhu/VirtualPet/blob/gh-pages/IMG_8459.GIF)   
[Jocelyn](https://github.com/jxcelynyu/VirtualPet/blob/gh-pages/IMG_0596.GIF)   
[Viva](https://github.com/vivavoong/VirtualPet/blob/gh-pages/processing_differentinputs.gif)   
[Kaitlin](https://github.com/kaiyenpepper/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20(2).gif)   
[Tiffany](https://github.com/tiffanyt11/VirtualPet/blob/gh-pages/845f586ee71d4459bf3b82f9efcedebb.gif)   
[Michelle](https://github.com/mitan4/VirtualPet/blob/gh-pages/bird.gif)   
[Jimmy](https://github.com/Jimmy1433223/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Alex](https://github.com/AlexHackathon/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20(1).gif)   
[Cameron](https://github.com/CaNguyen1/VirtualPet/blob/gh-pages/IMG_6116.GIF)   
[Mikey](https://github.com/miosullivan/ArduinoController/blob/main/ezgif.com-gif-maker%20(1).gif)   
[Nash](https://github.com/MoonNash/VirtualPet/blob/gh-pages/IMG_2876.GIF)   
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
[Karina](https://github.com/kaanders17/ArduinoController/blob/main/Arduino%20Controller%20GIF.GIF)   
[Bruno](https://github.com/bruno-415/VirtualPet/blob/gh-pages/ufo)   
[Damian](https://github.com/dabogdon/ArduinoController/blob/main/ezgif-4-0ce17385d59a.gif)   
[Paolo](https://github.com/paolo415/VirtualPet/blob/gh-pages/lightSensorShark.gif)   
[William](https://github.com/wicao1/VirtualPet/blob/gh-pages/other_arduino_buttons.gif)   
[Alvin](https://github.com/alchan6/VirtualPet/blob/gh-pages/Other%20Arduino%20Sensor.gif)   
[Christina](https://github.com/christina88chan/VirtualPet/blob/0c54b695443327fda79e071b026affb0292311e8/ezgif.com-gif-maker.gif)    
[Haden](https://github.com/hachan-beep/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%282%29.gif)   
[Joanne](https://github.com/joannechenn/ArduinoController/blob/main/ezgif.com-gif-maker%20%281%29.gif)   
[Irisa](https://github.com/irisac415/ArduinoController/blob/main/Fish%20Buttons.gif)   
[Christopher](https://github.com/ChGee/VirtualPet/blob/gh-pages/135C22BA-F855-477C-B751-C6C8E86F66B6.gif)   
[Wing](https://github.com/wilai3/ArduinoController/blob/main/ezgif.com-gif-maker%20%282%29.gif)   
[Caitlyn](https://github.com/calam1818/VirtualPet/blob/gh-pages/ezgif-2-ad9d63fa07a1.gif)   
[Breanna](https://github.com/brlau6/VirtualPet/blob/gh-pages/Abstract%20Rainbow%20Lines%20-%20Buttons%20and%20Light%20Sensor.gif)   
[Matthew](https://github.com/malee8/VirtualPet/blob/gh-pages/IMG_3427.GIF)   
[Ye](https://github.com/YejinL12/VirtualPet/blob/417992b7f3a6ce451937e2eb7658ad4ae9a4c743/colorfulOcto.gif)   
[Van](https://github.com/Vanthebot/VirtualPet/blob/gh-pages/otherArduinoSensor.gif)   
[Joshua](https://github.com/jopaza21/OtherArduinoSensors)   
[Edward](https://github.com/edpilotte/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Aiden](https://github.com/AidenShiu/VirtualPet/blob/gh-pages/ezgif-7-f278d7c40663.gif)   
[Andrew](https://github.com/antan2/VirtualPet/blob/gh-pages/buttons%20gif.gif)   
[Jeffrey](https://github.com/jethiDaCoder/VirtualPet/blob/gh-pages/Ping%20Pong.GIF)   
[Eric](https://github.com/desolaterakan/VirtualPet/blob/gh-pages/froog.gif)   
[Dylan](https://github.com/dy-alt/VirtualPet/blob/gh-pages/otherButtonsGif.gif)   
[Mira](https://github.com/mira16-v/VirtualPet/blob/gh-pages/other_sensor_GIF.gif)   
[Austin](https://drive.google.com/file/d/1D1Qi2s2Je5oXO8p3k0hUTvZQGbxz4wwr/view)   
[Jason](https://github.com/jawong32/Flappy)   
[Ivana](https://github.com/ivxu24/VirtualPet/blob/gh-pages/ezgif.com-video-to-gif.gif)   
[Gary](https://github.com/Gary055/anime/blob/main/ezgif.com-gif-maker%20%281%29.gif)   
[Emily](https://github.com/emyip/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Akemi](https://github.com/Akemi1222/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[William](https://github.com/WilliamsGitHubAccount/VirtualPet/blob/gh-pages/button_test.gif)   
[Stephen](https://github.com/stevenmeap/VirtualPet/blob/gh-pages/SnowManButton.gif)   
[Daniel](https://github.com/wood09/VirtualPet/blob/gh-pages/other_arduino_sensor-gif.gif)   
[Andrew](https://github.com/guppies23456/VirtualPet/blob/gh-pages/Other%20Sensor.gif)   
[Luke](https://github.com/LukeD808/VirtualPet/blob/gh-pages/LukeDonohueVirtualPetGif.gif)   
[Liam](https://github.com/ligiraldo/ArduinoController/blob/main/ezgif.com-gif-maker%20%281%29.gif)   
[Hayden](https://github.com/hakwok/VirtualPet/blob/gh-pages/gif-min.gif)   
[Jacob](https://github.com/jalambert/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Noella](https://github.com/noellalee1/VirtualPet/blob/gh-pages/D67067A3-0B42-4B34-8E5A-B5D9C5BB22CC.gif)   
[Caleb](https://github.com/caleung3/Snowman/blob/gh-pages/ezgif.com-gif-maker%20%284%29.gif)   
[Gabriel](https://github.com/galeung24/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Eric](https://github.com/ErLiao137/VirtualPet/blob/gh-pages/extra.arduino_gif.gif)   
[Joyce](https://drive.google.com/file/d/1B0qGeG1GO1Ip8Lg396Iwsc7S9PzcdVUQ/view)   
[Vivian](https://github.com/VivianMak/VirtualPet/blob/gh-pages/Other%20Arduino%20Sensors.gif)   
[Lexian](https://github.com/lexiannguyen/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Raina](https://drive.google.com/file/d/1xyOufV5JOFBs4oal3BEyj9Wa2SkbgPRc/view)   
[Rafael](https://github.com/IamRafaelllll/VirtualPet/blob/gh-pages/ezgif-3-8945803d9402.gif)   
[Nathaniel](https://github.com/NathanTjong/VirtualPet/blob/gh-pages/D29BD7F0-F638-4114-BDD5-F430A6F304E6.gif)   
[Nicolas](https://github.com/nireiss/VirtualPet/blob/gh-pages/sensorArduino.gif)   
[Brian](https://github.com/brsen/VirtualPet/blob/gh-pages/arduinoGameGIF.gif)   
[Justin](https://github.com/jushiu/Animation-2.0/blob/main/39F16F3D-26FB-45C0-B100-81D9FDC9A58F.gif)   
[Stella](https://github.com/StellaSit0/VirtualPet/blob/gh-pages/20210907_090630_1.gif)   
[Wendy](https://github.com/lafmj/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Joseph](https://github.com/JosephTeng/VirtualPet/blob/gh-pages/D0B5074F-26BA-4D05-BA87-E21E80FAE2A9.gif)   
[Joshua](https://github.com/jovegher/VirtualPet/blob/gh-pages/virtualcattemp.gif)   
[Brianna](https://github.com/brwong8/VirtualPet/blob/gh-pages/ezgif.com-video-to-gif%203.gif)   
[Justin](https://github.com/Justin-pyth/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Qiaoyan](https://github.com/QIAOYANX/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%282%29.gif)   
[Antonio](https://drive.google.com/file/d/11ZHX5IiykP8i5Yy4sSdWhpnMpqXj5duz/view)   
[Caden](https://github.com/cayeung1/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[TommyJun](https://github.com/toyu3/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[David](https://github.com/davidzhang3/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Darren](https://github.com/DarrenZhao1/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%202.gif)   
[Emily](https://github.com/huishancai/VirtualPet/blob/gh-pages/ezgif.com-video-to-gif%203.gif)   
[Brennan](https://github.com/Brennan-c/VirtualPet/blob/gh-pages/otherSensor.gif)   
[Jennifer](https://github.com/jennifer0525/VirtualPet/blob/gh-pages/Other%20Senors%20Virtual%20Pet.gif)   
[Deion](https://github.com/deionchaudhary/Panda/blob/gh-pages/otherArduinoSensors.gif)   
[Aaron](https://github.com/AaronnChen/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Jackie](https://github.com/jachen16/VirtualPet/blob/gh-pages/Other-Arduino-Sensors-Sep-3-2021.gif)   
[Christina](https://github.com/chchung1/VirtualPet/blob/gh-pages/other%20sensors.gif)   
[Joselino](https://github.com/joselinodt/VirtualPet/blob/gh-pages/IMG-9486.GIF)   
[Nathan](https://github.com/Naguan1/VirtualPet/blob/1741ad2cc41ccf1f048c3201c56ea2ba20c8e3ae/ezgif.com-gif-maker%20%283%29.gif)   
[Munkhtushie](https://github.com/tushigitgel/VirtualPet/blob/gh-pages/ezgifotherarduino.gif)   
[Kyle](https://github.com/kylam1/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[Noelle](https://github.com/noellelam/VirtualPet/blob/441fd125be9c1d5632d927bda3cb7f072426e491/ezgif.com-gif-maker.gif)   
[Andy](https://github.com/andeey3/VirtualPet/blob/gh-pages/ezgif-4-5a1c7e858863.gif)   
[Audrey](https://github.com/AudreyLau8/VirtualPet/blob/gh-pages/ezgif.com-gif-maker.gif)   
[William](https://github.com/Williamlaw2005/VirtualPet/blob/gh-pages/other%20sensor%20gif.gif)   
[Jenna](https://github.com/Jenna1910/VirtualPet/blob/gh-pages/ezgif.com-gif-maker%20%281%29.gif)   
[Ryan](https://github.com/chknwngs999/VirtualPet/blob/gh-pages/arduinoinput.gif)   

