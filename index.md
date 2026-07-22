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

  For my final milestone, I decided to add a LiDAR inspired system to make the self driving a lot more reliable and accurate. I also added an Arduino Mega 2560 to replace the old Arduino Uno R3.

  - A LiDAR is a light detection and ranging system that uses rapid laser pulses to measure distaces. By calculating how long it takes for the light to hit the surface and bounce back, it creates a highly accurate 3d map.
 
  - An Arduino Mega is a high capacity micro controller that is a more powerful sibling of the stadard Arduino Uno
  


# Second Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/Tyyodlb5-hw?si=uqHzkyr4-grcvucV" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

For your second milestone, explain what you've worked on since your previous milestone. You can highlight:
- Technical details of what you've accomplished and how they contribute to the final goal
- What has been surprising about the project so far
- Previous challenges you faced that you overcame
- What needs to be completed before your final milestone

    For my second milestone, I made a self driving car. The car works by using 2 IR sensors on the sides and an ultra sonic sensor at the very front of the car that are all connected to an Arduino Uno R3. This Arduino is connected to a L9110 module that is connected to 2 TT Motors.
  
   - An IR sensor is a sensor that dectects infared radiation, which is a type of invisible light emmited from objects based on their heat. The IR sensor has 2 main components, an IR LED and a IR photodiode. The IR LED emits the infared light and the IR photodiode dectects it. The IR photodiode is able to calculate the distance of an object based off of the light by generating an electrical signal that is proportional to the intensity of the light that it recived. The sensor then takes this information and uses it to calculate the distance of an object.
     
   - An Ultra Sonic Sensor is a sensor that can meassure distance or dected objects by emmiting high frequency sound waves. The transmitter generates high frequency sound waves (Typically around 40 kHz) and radiets them into the envoirment that the sensor is in. The receiver dectects these sound waves and converts them the waves into an electrical signal. This electrical signal obtained by the receiver get calculated and turned into a distance by the signal processing electronics in the sensor.
 
     The IR sensors work in the car by dectecting wether there is an object infront of the sensors. If there is an object, the sensor emits a 1 in the code. If there isn't an object, the sensor emits a 0 in the code. At the very front of the is the ultra sonic sensors. The sensors are there so that it can make the car stop and turn around when there is an object 0-20 cm away. All of these sensors make the car be able to drive by itself.

    


# First Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**
<iframe width="560" height="315" src="https://www.youtube.com/embed/SrDImx5UroA?si=3cv8lOjH-G7pOcDL" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

For your first milestone, describe what your project is and how you plan to build it. You can include:
- An explanation about the different components of your project and how they will all integrate together
- Technical progress you've made so far
- Challenges you're facing and solving in your future milestones
- What your plan is to complete your project

    For my first milestone, I made a car that is able to track black tape and be able to follow it. It works by using a line tracking module that can track the color black. This sensor was connected to an Arduino Uno R3 using cables. This arduino was connected to a L9110 module which was connected to 2 TT motors.
    
    - An L9100 module is a small circuit board that helps small computers like an Arduino control the speed and direction of motors.
 
    - A TT motor is a DC gear motor that operates on 3V to 6V DC.
 
    - An Arduino Uno R3 is a small micro controller used to build electronics projects.
 
    - A line tracking module is a small sensor used by robots to follow a specific path. 


  The purpose of the Arduino Uno R3 was so I could power and code the line tracking module. I coded the line tracking module in the Arduino IDE software. The language of this sofware is a modifed version of C++. The 2 TT motors were the motors that powered the wheels which made the car able to drive around using code. The purpose L9110 module is to make the coding and math easier when connecting the motors to the arduino.

    All of these components made it possible for when the car dectects the color black, then it would move left. But when it sees any other color, it would move right after some coding. The reason that I decided to use tape and not any other black object was because the sensor was connected to the frame of the car using some screws and small brakets. This made the sensor point toward the bottom so it didn't have a lot of options of what it could track and black tape was a reusable object near me that could produce strait lines when placed so I decided to use it.

    Some challenges that I faced during this project was assebling all the wiring and making sure that the wires don't fall out of where they are supposed to go. I plan to solve this issue by soldering the wires to my sensors so it is much more reliable and so it won't fall out.


# Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 

# Code For Self Driving Car
Here's where you'll put your code. The syntax below places it into a block of code. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize it to your project needs. 

```c++
#include <Servo.h>
#include <Wire.h>
#include <Adafruit_MPU6050.h>
#include <Adafruit_Sensor.h>
#include <avr/wdt.h>

// ============================================================
// HARDWARE OBJECTS
// ============================================================

Servo scanningServo;
Adafruit_MPU6050 mpu;

// ============================================================
// PIN CONFIGURATION
// ============================================================

// Ultrasonic Sensor 1
const int TRIG_PIN_1 = 12;
const int ECHO_PIN_1 = 13;

// Ultrasonic Sensor 2
const int TRIG_PIN_2 = 8;
const int ECHO_PIN_2 = 9;

// Ultrasonic Sensor 3
const int TRIG_PIN_3 = 10;
const int ECHO_PIN_3 = 11;

// Ultrasonic Sensor 4
const int TRIG_PIN_4 = 27;
const int ECHO_PIN_4 = 26;

// Servo
const int SERVO_PIN = 7;

// Motor A: right wheel
const int A_1B = 51;
const int A_1A = 50;

// Motor B: left wheel
const int B_1B = 53;
const int B_1A = 52;

// ============================================================
// SCANNING CONFIGURATION
// ============================================================

const int SCAN_START_ANGLE = 0;
const int SCAN_END_ANGLE = 85;
const int SCAN_ANGLE_STEP = 5;

const int NUM_SCAN_STEPS =
  ((SCAN_END_ANGLE - SCAN_START_ANGLE) / SCAN_ANGLE_STEP) + 1;

const int GROUP_SIZE = 3;
const int NUM_GROUPS = NUM_SCAN_STEPS / GROUP_SIZE;

// Time given to the servo after each movement.
const unsigned long SERVO_STEP_DELAY_MS = 20;

// Time given to the servo for a large reset movement.
const unsigned long SERVO_RESET_DELAY_MS = 250;

// Maximum ultrasonic echo wait time.
//
// 25,000 microseconds corresponds to roughly 425 cm.
// A timeout prevents one missing echo from freezing the scan.
const unsigned long ULTRASONIC_TIMEOUT_US = 25000;

// Reading used when the sensor receives no echo.
const float MAX_DISTANCE_CM = 400.0;

// Small pause between ultrasonic sensors to reduce interference.
const unsigned int SENSOR_GAP_US = 800;

// ============================================================
// MOVEMENT CONFIGURATION
// ============================================================

// Servo angle representing straight ahead.
// Recalibrate this value if necessary.
const int CENTER_ANGLE = 42;

// Stop turning when this close to the desired angle.
const float ANGLE_MARGIN_DEGREES = 5.0;

// Maximum time allowed for one turn.
const unsigned long ROTATE_TIMEOUT_MS = 2500;

// How long the car moves after choosing a direction.
const unsigned long DRIVE_DURATION_MS = 2000;

// Obstacle behavior.
const float BOXED_IN_DISTANCE_CM = 10.0;
const float CLOSE_PROXIMITY_DISTANCE_CM = 10.0;
const int CLOSE_SENSOR_THRESHOLD = 3;

const unsigned long BACKUP_TIME_MS = 800;
const unsigned long ESCAPE_ROTATE_TIME_MS = 600;

// Brief motor pause before starting a turn.
const unsigned long MOTOR_DIRECTION_DELAY_MS = 30;

// Ignore extremely small gyro readings while integrating.
const float GYRO_DEAD_ZONE_DPS = 1.5;

// ============================================================
// TURNING DIRECTION CONFIGURATION
// ============================================================

// Set either of these to true if that movement is physically reversed.
//
// For example, if turnLeft() makes the car rotate right, change
// REVERSE_TURN_DIRECTIONS to true.
const bool REVERSE_TURN_DIRECTIONS = false;

// If the measured gyro angle does not increase while the car turns,
// change this to true.
const bool REVERSE_GYRO_SIGN = false;

// Your original code treated target angles greater than CENTER_ANGLE
// as left turns because the turret was mounted in reverse.
const bool HIGHER_SERVO_ANGLE_MEANS_LEFT = true;

// ============================================================
// DATA STRUCTURES
// ============================================================

struct UltrasonicSensor {
  int trigPin;
  int echoPin;
  float distance;

  void begin() {
    pinMode(trigPin, OUTPUT);
    pinMode(echoPin, INPUT);

    digitalWrite(trigPin, LOW);
  }

  void update() {
    digitalWrite(trigPin, LOW);
    delayMicroseconds(2);

    digitalWrite(trigPin, HIGH);
    delayMicroseconds(10);

    digitalWrite(trigPin, LOW);

    unsigned long duration =
      pulseIn(echoPin, HIGH, ULTRASONIC_TIMEOUT_US);

    if (duration == 0) {
      // No echo arrived before the timeout.
      distance = MAX_DISTANCE_CM;
    } else {
      distance = duration * 0.0343 / 2.0;

      if (distance > MAX_DISTANCE_CM) {
        distance = MAX_DISTANCE_CM;
      }
    }
  }

  float getDistance() const {
    return distance;
  }
};

struct Packet {
  float sensor1;
  float sensor2;
  float sensor3;
  float sensor4;
};

struct Reading {
  int angle;
  float distance;
};

struct Group {
  int angle;
  float average;
};

// ============================================================
// SENSOR OBJECTS
// ============================================================

UltrasonicSensor sensor1 = {
  TRIG_PIN_1,
  ECHO_PIN_1,
  MAX_DISTANCE_CM
};

UltrasonicSensor sensor2 = {
  TRIG_PIN_2,
  ECHO_PIN_2,
  MAX_DISTANCE_CM
};

UltrasonicSensor sensor3 = {
  TRIG_PIN_3,
  ECHO_PIN_3,
  MAX_DISTANCE_CM
};

UltrasonicSensor sensor4 = {
  TRIG_PIN_4,
  ECHO_PIN_4,
  MAX_DISTANCE_CM
};

// ============================================================
// GLOBAL STATE
// ============================================================

float bestDistanceFound = 0.0;
float gyroZBiasDps = 0.0;

// ============================================================
// MOTOR CONTROL
// ============================================================

void beginMotors() {
  pinMode(A_1B, OUTPUT);
  pinMode(A_1A, OUTPUT);
  pinMode(B_1B, OUTPUT);
  pinMode(B_1A, OUTPUT);

  digitalWrite(A_1B, LOW);
  digitalWrite(A_1A, LOW);
  digitalWrite(B_1B, LOW);
  digitalWrite(B_1A, LOW);
}

void stopCar() {
  digitalWrite(A_1B, LOW);
  digitalWrite(A_1A, LOW);
  digitalWrite(B_1B, LOW);
  digitalWrite(B_1A, LOW);
}

void moveForward() {
  // Right motor forward
  digitalWrite(A_1B, LOW);
  digitalWrite(A_1A, HIGH);

  // Left motor forward
  digitalWrite(B_1B, HIGH);
  digitalWrite(B_1A, LOW);
}

void moveBackward() {
  // Right motor backward
  digitalWrite(A_1B, HIGH);
  digitalWrite(A_1A, LOW);

  // Left motor backward
  digitalWrite(B_1B, LOW);
  digitalWrite(B_1A, HIGH);
}

void rawTurnRight() {
  // Right wheel backward
  digitalWrite(A_1B, HIGH);
  digitalWrite(A_1A, LOW);

  // Left wheel forward
  digitalWrite(B_1B, HIGH);
  digitalWrite(B_1A, LOW);
}

void rawTurnLeft() {
  // Right wheel forward
  digitalWrite(A_1B, LOW);
  digitalWrite(A_1A, HIGH);

  // Left wheel backward
  digitalWrite(B_1B, LOW);
  digitalWrite(B_1A, HIGH);
}

void turnRight() {
  if (REVERSE_TURN_DIRECTIONS) {
    rawTurnLeft();
  } else {
    rawTurnRight();
  }
}

void turnLeft() {
  if (REVERSE_TURN_DIRECTIONS) {
    rawTurnRight();
  } else {
    rawTurnLeft();
  }
}

// ============================================================
// IMU AND GYROSCOPE
// ============================================================

float readRawYawRateDps() {
  sensors_event_t acceleration;
  sensors_event_t gyro;
  sensors_event_t temperature;

  mpu.getEvent(&acceleration, &gyro, &temperature);

  return gyro.gyro.z * 180.0 / PI;
}

float getYawRateDps() {
  float yawRate = readRawYawRateDps() - gyroZBiasDps;

  if (REVERSE_GYRO_SIGN) {
    yawRate = -yawRate;
  }

  if (abs(yawRate) < GYRO_DEAD_ZONE_DPS) {
    yawRate = 0.0;
  }

  return yawRate;
}

void calibrateGyroscope() {
  Serial.println("Calibrating gyroscope...");
  Serial.println("Keep the car completely still.");

  stopCar();

  const int calibrationSamples = 300;
  float total = 0.0;

  for (int i = 0; i < calibrationSamples; i++) {
    total += readRawYawRateDps();

    if (i % 50 == 0) {
      wdt_reset();
    }

    delay(5);
  }

  gyroZBiasDps = total / calibrationSamples;

  Serial.print("Gyroscope Z bias: ");
  Serial.print(gyroZBiasDps, 4);
  Serial.println(" degrees/second");
}

// ============================================================
// ULTRASONIC SENSOR READING
// ============================================================

Packet readAllSensors() {
  Packet packet;

  sensor1.update();
  packet.sensor1 = sensor1.getDistance();

  delayMicroseconds(SENSOR_GAP_US);

  sensor2.update();
  packet.sensor2 = sensor2.getDistance();

  delayMicroseconds(SENSOR_GAP_US);

  sensor3.update();
  packet.sensor3 = sensor3.getDistance();

  delayMicroseconds(SENSOR_GAP_US);

  sensor4.update();
  packet.sensor4 = sensor4.getDistance();

  return packet;
}

int countCloseSensors(const Packet &packet) {
  int count = 0;

  if (
    packet.sensor1 > 0 &&
    packet.sensor1 <= CLOSE_PROXIMITY_DISTANCE_CM
  ) {
    count++;
  }

  if (
    packet.sensor2 > 0 &&
    packet.sensor2 <= CLOSE_PROXIMITY_DISTANCE_CM
  ) {
    count++;
  }

  if (
    packet.sensor3 > 0 &&
    packet.sensor3 <= CLOSE_PROXIMITY_DISTANCE_CM
  ) {
    count++;
  }

  if (
    packet.sensor4 > 0 &&
    packet.sensor4 <= CLOSE_PROXIMITY_DISTANCE_CM
  ) {
    count++;
  }

  return count;
}

// ============================================================
// SCAN PROCESSING
// ============================================================

void groupSensorReadings(
  Reading readings[],
  int readingCount,
  Group groups[]
) {
  int groupIndex = 0;

  for (
    int startIndex = 0;
    startIndex + GROUP_SIZE - 1 < readingCount;
    startIndex += GROUP_SIZE
  ) {
    float total = 0.0;

    for (int offset = 0; offset < GROUP_SIZE; offset++) {
      total += readings[startIndex + offset].distance;
    }

    int middleIndex = startIndex + GROUP_SIZE / 2;

    groups[groupIndex].angle =
      readings[middleIndex].angle;

    groups[groupIndex].average =
      total / GROUP_SIZE;

    groupIndex++;
  }
}

void printLargestGroup(
  const char *sensorName,
  Group groups[]
) {
  float largestDistance = groups[0].average;
  int largestAngle = groups[0].angle;

  for (int groupIndex = 1; groupIndex < NUM_GROUPS; groupIndex++) {
    if (groups[groupIndex].average > largestDistance) {
      largestDistance = groups[groupIndex].average;
      largestAngle = groups[groupIndex].angle;
    }
  }

  Serial.print(sensorName);
  Serial.print(" largest group: ");
  Serial.print(largestDistance, 1);
  Serial.print(" cm at angle ");
  Serial.println(largestAngle);
}

void considerGroup(
  const Group &group,
  float &bestDistance,
  int &bestAngle
) {
  if (group.average > bestDistance) {
    bestDistance = group.average;
    bestAngle = group.angle;
  }
}

int findOverallBestAngle(
  Group sensor1Groups[],
  Group sensor2Groups[],
  Group sensor3Groups[],
  Group sensor4Groups[]
) {
  float bestDistance = -1.0;
  int bestAngle = CENTER_ANGLE;

  for (int groupIndex = 0; groupIndex < NUM_GROUPS; groupIndex++) {
    considerGroup(
      sensor1Groups[groupIndex],
      bestDistance,
      bestAngle
    );

    considerGroup(
      sensor4Groups[groupIndex],
      bestDistance,
      bestAngle
    );

    // Preserve your original behavior:
    // ignore the first group for Sensors 2 and 3 because those
    // sensors face backward at the beginning of the sweep.
    if (groupIndex != 0) {
      considerGroup(
        sensor2Groups[groupIndex],
        bestDistance,
        bestAngle
      );

      considerGroup(
        sensor3Groups[groupIndex],
        bestDistance,
        bestAngle
      );
    }
  }

  bestDistanceFound = bestDistance;

  return bestAngle;
}

int processScan(
  Packet scanData[],
  int scanCount
) {
  Reading readings1[NUM_SCAN_STEPS];
  Reading readings2[NUM_SCAN_STEPS];
  Reading readings3[NUM_SCAN_STEPS];
  Reading readings4[NUM_SCAN_STEPS];

  for (int index = 0; index < scanCount; index++) {
    int angle =
      SCAN_START_ANGLE + index * SCAN_ANGLE_STEP;

    readings1[index] = {
      angle,
      scanData[index].sensor1
    };

    readings2[index] = {
      angle,
      scanData[index].sensor2
    };

    readings3[index] = {
      angle,
      scanData[index].sensor3
    };

    readings4[index] = {
      angle,
      scanData[index].sensor4
    };
  }

  Group groups1[NUM_GROUPS];
  Group groups2[NUM_GROUPS];
  Group groups3[NUM_GROUPS];
  Group groups4[NUM_GROUPS];

  groupSensorReadings(
    readings1,
    scanCount,
    groups1
  );

  groupSensorReadings(
    readings2,
    scanCount,
    groups2
  );

  groupSensorReadings(
    readings3,
    scanCount,
    groups3
  );

  groupSensorReadings(
    readings4,
    scanCount,
    groups4
  );

  printLargestGroup("SENSOR 1", groups1);
  printLargestGroup("SENSOR 2", groups2);
  printLargestGroup("SENSOR 3", groups3);
  printLargestGroup("SENSOR 4", groups4);

  int bestAngle = findOverallBestAngle(
    groups1,
    groups2,
    groups3,
    groups4
  );

  Serial.print("Best angle: ");
  Serial.print(bestAngle);

  Serial.print(" | Best distance: ");
  Serial.print(bestDistanceFound, 1);

  Serial.println(" cm");

  return bestAngle;
}

// ============================================================
// TURNING
// ============================================================

void rotateToAngle(int targetAngle) {
  int servoDifference = targetAngle - CENTER_ANGLE;
  float requestedTurnDegrees = abs(servoDifference);

  Serial.println();
  Serial.println("Beginning rotation");

  Serial.print("Target servo angle: ");
  Serial.println(targetAngle);

  Serial.print("Center servo angle: ");
  Serial.println(CENTER_ANGLE);

  Serial.print("Requested physical turn: ");
  Serial.print(requestedTurnDegrees, 1);
  Serial.println(" degrees");

  if (requestedTurnDegrees <= ANGLE_MARGIN_DEGREES) {
    Serial.println("Direction is already approximately forward.");
    stopCar();
    return;
  }

  bool shouldTurnLeft;

  if (HIGHER_SERVO_ANGLE_MEANS_LEFT) {
    shouldTurnLeft = servoDifference > 0;
  } else {
    shouldTurnLeft = servoDifference < 0;
  }

  stopCar();
  delay(MOTOR_DIRECTION_DELAY_MS);

  if (shouldTurnLeft) {
    Serial.println("Turning left");
    turnLeft();
  } else {
    Serial.println("Turning right");
    turnRight();
  }

  float accumulatedDegrees = 0.0;

  unsigned long rotationStart = micros();
  unsigned long previousReadingTime = rotationStart;
  unsigned long previousPrintTime = millis();

  while (accumulatedDegrees <
         requestedTurnDegrees - ANGLE_MARGIN_DEGREES) {
    wdt_reset();

    unsigned long nowMicros = micros();
    unsigned long elapsedMicros =
      nowMicros - previousReadingTime;

    previousReadingTime = nowMicros;

    float deltaTimeSeconds =
      elapsedMicros / 1000000.0;

    float yawRateDps = getYawRateDps();

    // We already selected the direction using the target angle.
    // Accumulating the magnitude prevents a gyro sign mismatch from
    // causing the turn loop to run forever.
    accumulatedDegrees +=
      abs(yawRateDps) * deltaTimeSeconds;

    unsigned long elapsedRotationMs =
      (nowMicros - rotationStart) / 1000UL;

    if (millis() - previousPrintTime >= 100) {
      Serial.print("Yaw rate: ");
      Serial.print(yawRateDps, 1);

      Serial.print(" dps | Turned: ");
      Serial.print(accumulatedDegrees, 1);

      Serial.print(" / ");
      Serial.println(requestedTurnDegrees, 1);

      previousPrintTime = millis();
    }

    if (elapsedRotationMs >= ROTATE_TIMEOUT_MS) {
      Serial.println("Rotation timeout reached.");
      break;
    }

    delay(2);
  }

  stopCar();

  Serial.print("Rotation finished after approximately ");
  Serial.print(accumulatedDegrees, 1);
  Serial.println(" degrees");

  delay(100);
}

// ============================================================
// OBSTACLE RESPONSE
// ============================================================

void handleImmediateProximity() {
  Serial.println();
  Serial.println("Three or more sensors detected a close obstacle.");

  stopCar();

  scanningServo.write(CENTER_ANGLE);
  wdt_reset();
  delay(SERVO_RESET_DELAY_MS);

  Serial.println("Backing away.");

  moveBackward();

  unsigned long backupStart = millis();

  while (millis() - backupStart < BACKUP_TIME_MS) {
    wdt_reset();
    delay(5);
  }

  stopCar();
}

void handleBoxedIn() {
  Serial.println();
  Serial.println("Best direction is blocked.");
  Serial.println("Checking the rear before backing up.");

  sensor2.update();
  delayMicroseconds(SENSOR_GAP_US);
  sensor3.update();

  float rearDistance = min(
    sensor2.getDistance(),
    sensor3.getDistance()
  );

  Serial.print("Rear distance: ");
  Serial.print(rearDistance, 1);
  Serial.println(" cm");

  if (rearDistance > BOXED_IN_DISTANCE_CM) {
    Serial.println("Rear is clear. Backing up.");

    moveBackward();

    unsigned long backupStart = millis();

    while (millis() - backupStart < BACKUP_TIME_MS) {
      wdt_reset();
      delay(5);
    }

    stopCar();
  } else {
    // Do not permanently freeze here. The original boxed-in
    // condition could enter a permanent stop whenever the rear
    // was also blocked.
    Serial.println("Rear is blocked. Performing escape rotation.");

    turnRight();

    unsigned long escapeStart = millis();

    while (
      millis() - escapeStart < ESCAPE_ROTATE_TIME_MS
    ) {
      wdt_reset();
      delay(5);
    }

    stopCar();
  }

  scanningServo.write(SCAN_START_ANGLE);
  wdt_reset();
  delay(SERVO_RESET_DELAY_MS);
}

// ============================================================
// DRIVING
// ============================================================

void driveForwardForConfiguredTime() {
  Serial.println();
  Serial.print("Driving forward for ");
  Serial.print(DRIVE_DURATION_MS);
  Serial.println(" ms");

  moveForward();

  unsigned long driveStart = millis();

  while (millis() - driveStart < DRIVE_DURATION_MS) {
    wdt_reset();
    delay(5);
  }

  stopCar();

  Serial.println("Forward movement finished.");
}

// ============================================================
// SETUP
// ============================================================

void setup() {
  Serial.begin(115200);

  scanningServo.attach(SERVO_PIN);

  sensor1.begin();
  sensor2.begin();
  sensor3.begin();
  sensor4.begin();

  beginMotors();
  stopCar();

  scanningServo.write(SCAN_START_ANGLE);
  delay(SERVO_RESET_DELAY_MS);

  if (!mpu.begin()) {
    Serial.println("Failed to find MPU6050.");

    while (true) {
      delay(100);
    }
  }

  mpu.setGyroRange(MPU6050_RANGE_500_DEG);
  mpu.setAccelerometerRange(MPU6050_RANGE_8_G);
  mpu.setFilterBandwidth(MPU6050_BAND_21_HZ);

  Serial.println("MPU6050 found.");

  // Enable after sensor initialization so setup does not reset
  // during the initial connection process.
  wdt_enable(WDTO_2S);

  calibrateGyroscope();

  Serial.println();
  Serial.println("Robot ready.");
}

// ============================================================
// MAIN LOOP
// ============================================================

void loop() {
  wdt_reset();

  Serial.println();
  Serial.println("========================================");
  Serial.println("Starting new scan cycle");
  Serial.println("========================================");

  stopCar();

  Packet scanData[NUM_SCAN_STEPS];

  int scanIndex = 0;
  bool scanInterrupted = false;

  unsigned long scanStartTime = millis();

  for (
    int servoAngle = SCAN_START_ANGLE;
    servoAngle <= SCAN_END_ANGLE;
    servoAngle += SCAN_ANGLE_STEP
  ) {
    wdt_reset();

    scanningServo.write(servoAngle);
    delay(SERVO_STEP_DELAY_MS);

    Packet packet = readAllSensors();

    scanData[scanIndex] = packet;
    scanIndex++;

    Serial.print("Angle ");
    Serial.print(servoAngle);

    Serial.print(" | S1: ");
    Serial.print(packet.sensor1, 1);

    Serial.print(" | S2: ");
    Serial.print(packet.sensor2, 1);

    Serial.print(" | S3: ");
    Serial.print(packet.sensor3, 1);

    Serial.print(" | S4: ");
    Serial.println(packet.sensor4, 1);

    if (
      countCloseSensors(packet) >=
      CLOSE_SENSOR_THRESHOLD
    ) {
      handleImmediateProximity();
      scanInterrupted = true;
      break;
    }
  }

  unsigned long scanDuration =
    millis() - scanStartTime;

  Serial.print("Scan duration: ");
  Serial.print(scanDuration);
  Serial.println(" ms");

  if (scanInterrupted) {
    scanningServo.write(SCAN_START_ANGLE);
    wdt_reset();
    delay(SERVO_RESET_DELAY_MS);
    return;
  }

  int bestAngle =
    processScan(scanData, scanIndex);

  if (
    bestDistanceFound <
    BOXED_IN_DISTANCE_CM
  ) {
    handleBoxedIn();
    return;
  }

  rotateToAngle(bestAngle);

  // Return the sensor assembly to the beginning of its sweep
  // while the car is about to drive.
  scanningServo.write(SCAN_START_ANGLE);

  driveForwardForConfiguredTime();
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
