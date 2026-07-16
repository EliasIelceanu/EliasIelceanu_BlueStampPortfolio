# BlueStamp Self Driving Robotic Car
This project is a self driving car that works by using infared sensors and an ultrasonic sensor, that are all connected to an Arduino Uno r3, to make the car be able to detect obsticals infront of it. One issue that I faced while making this project was that the sensors weren't doing the best job at sensing objects and the car would sometimes get stuck. I fixed this by making a pseudo lidar out of ultrasonic senors that were doing a much better job at detecting objects.


| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Elias I | RJ Fisher Middle School | Electrical Engineering | Incoming Eighth Grader

**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**

![Headstone Image](logo.svg)
  
# Final Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE



# Second Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/Tyyodlb5-hw?si=uqHzkyr4-grcvucV" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

For your second milestone, explain what you've worked on since your previous milestone. You can highlight:
- Technical details of what you've accomplished and how they contribute to the final goal
- What has been surprising about the project so far
- Previous challenges you faced that you overcame
- What needs to be completed before your final milestone

    For my second milestone, I made a self driving car. The car works by using 2 IR sensors on the sides and an ultra sonic sensor at the very front of the car that are all connected to an Arduino Uno R3. This Arduino is connected to a L9110 module that is connected to 2 TT Motors.
  
   - An IR sensor is a sensor that dectects infared radiation, which is a type of invisible light emmited from objects based on their heat. The IR sensor has 2 main components, an IR LED and a IR photodiode. The IR LED emits the infared light and the IR photodiode dectects it. The IR photodiode is able to calculate the distance of an object based off of the light by generating an electrical signal that is proportional to the intensity of the light that it recived. The sensor then takes this information and uses it to calculate the distance of an object
     
   - An Ultra Sonic Sensor is a sensor that can meassure distance or dected objects by emmiting high frequency sound waves. The transmitter generates high frequency sound waves (Typically around 40 kHz) and radiets them into the envoirment that the sensor is in. The receiver dectects these sound waves and converts them the waves into an electrical signal. This electrical signal obtained by the receiver get calculated and turned into a distance by the signal processing electronics in the sensor.
 
     The IR sensors work in the car by dectecting wether there is an object infront of the sensors  

    


# First Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**
<iframe width="560" height="315" src="https://www.youtube.com/embed/SrDImx5UroA?si=3cv8lOjH-G7pOcDL" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

For your first milestone, describe what your project is and how you plan to build it. You can include:
- An explanation about the different components of your project and how they will all integrate together
- Technical progress you've made so far
- Challenges you're facing and solving in your future milestones
- What your plan is to complete your project

    For my first milestone, I made a car that is able to track black tape and be able to follow it. It works by using a line tracking module that can track the color black. This sensor was connected to an Arduino Uno R3 using cables. This arduino was connected to a L9110 module which was connected to 2 TT motors. The purpose of the Arduino Uno R3 was so I could power and code the line tracking module. I coded the line tracking module in the Arduino IDE software. The language of this sofware is a modifed version of C++. The 2 TT motors were the motors that powered the wheels which made the car able to drive around using code. The purpose L9110 module is to make the coding and math easier when connecting the motors to the arduino.
    All of this made it possible for when the car dectects the color black, then it would move left. But when it sees any other color, it would move right after some coding. The reason that I decided to use tape and not any other black object was because the sensor was connected to the frame of the car using some screws and small brakets. This made the sensor point toward the bottom so it didn't have a lot of options of what it could track and black tape was a reusable object near me that could produce strait lines when placed so I decided to use it.
    Some challenges that I faced during this project was assebling all the wiring and making sure that the wires don't fall out of where they are supposed to go. I plan to solve this issue by soldering the wires to my sensors so it is much more reliable and so it won't fall out.
# Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 

# Code For Self Driving Car
Here's where you'll put your code. The syntax below places it into a block of code. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize it to your project needs. 

```c++
#include <Servo.h>

Servo myServo;

long duration;

int distance1;
int distance2;
int distance3;
int distance4;

const int trigPin1 = 12;
const int echoPin1 = 13;

const int trigPin2 = 8;
const int echoPin2 = 9;

const int trigPin3 = 10;
const int echoPin3 = 11;

const int trigPin4 = 44;
const int echoPin4 = 45;

void setup() {
  Serial.begin(9600);
  myServo.attach(7);    
  
  pinMode(trigPin1, OUTPUT);
  pinMode(echoPin1, INPUT);

  pinMode(trigPin2, OUTPUT);
  pinMode(echoPin2, INPUT);

  pinMode(trigPin3, OUTPUT);
  pinMode(echoPin3, INPUT);

  pinMode(trigPin4, OUTPUT);
  pinMode(echoPin4, INPUT);
}

void loop() {
  for (int i = 0; i<90; i+=5){
    myServo.write(i);
    delay(250);
    
    
    
    digitalWrite(trigPin1, LOW);
    delayMicroseconds(2);

    digitalWrite(trigPin1, HIGH);
    delayMicroseconds(10);
    digitalWrite(trigPin1, LOW);

    duration = pulseIn(echoPin1, HIGH);

    distance1 = duration * 0.034 / 2;
    
    
    
    digitalWrite(trigPin2, LOW);
    delayMicroseconds(2);

    digitalWrite(trigPin2, HIGH);
    delayMicroseconds(10);
    digitalWrite(trigPin2, LOW);

    duration = pulseIn(echoPin2, HIGH);

    distance2 = duration * 0.034 / 2;




    digitalWrite(trigPin3, LOW);
    delayMicroseconds(2);

    digitalWrite(trigPin3, HIGH);
    delayMicroseconds(10);
    digitalWrite(trigPin3, LOW);

    duration = pulseIn(echoPin3, HIGH);

    distance3 = duration * 0.034 / 2;




    digitalWrite(trigPin4, LOW);
   delayMicroseconds(2);

    digitalWrite(trigPin4, HIGH);
    delayMicroseconds(10);
   digitalWrite(trigPin4, LOW);

    duration = pulseIn(echoPin4, HIGH);

    distance4 = duration * 0.034 / 2;



   
    
    Serial.print(" Distance Of Sensor 1:  ");
    Serial.print(distance1);
    Serial.print(" Distance of Sensor 2:  ");
    Serial.print(distance2);
    Serial.print(" Distance Of Sensor 3:  ");
    Serial.print(distance3);
     Serial.print(" Distance of Sensor 4:  ");
    Serial.println(distance4);
    
  }
 
  
}


```

# Bill of Materials
TEST TEST TEST
Don't forget to place the link of where to buy each component inside the quotation marks in the corresponding row after href =. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize this to your project needs. 

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| SunFounder Ultimate Starter Kit Compatible with Arduino UNO IDE Scratch, 3 in 1| This is the cit to build the self driving car | $59.99 | <a href="[https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/](https://www.amazon.com/dp/B0B778L1DZ?lv=shuf&channelId=500&plpRedirect=mhFallback)"> Link </a> |
| Arduino Mega | This is one of the micro controllers for the project | $22.99 | <a href="https://www.amazon.com/ELEGOO-Compatible-Arduino-Projects-Compliant/dp/B01H4ZLZLQ/ref=sr_1_1?crid=2DMDC8DE4Q17O&dib=eyJ2IjoiMSJ9.7p3IEWq35-BhC7n2xPX9j_z4O4fOEa-f6EiV2WYTawSZ0qspE73EfIJD3EeU0BFKa5RIUUEOd8ZL_9-liu4TuGG4zGZaj-_iTLAsMBVXg5gAeEbCkla7aqVXZsWHSh8FI6Z8VUTzH6ZmJTbcRTk7OLEHUc3-k8DkjnY_t0CLul3vNutqy64RcqCdBhKflN3KB4uZPNvC5kXFQIhQM73rzyx7TRLmjdEKmaivCQrxT7E.FRkBUQzH1-ucwkDKRP2AznX1pAwwFonRQtns1BJ16pA&dib_tag=se&keywords=arduino%2Bmega%2Belegoo&qid=1783023442&sprefix=Arduino%2BMega%2Bel%2Caps%2C180&sr=8-1&th=1"> Link </a> |
| |   |  |  |

# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [Example 1](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/)

To watch the BSE tutorial on how to create a portfolio, click here.
