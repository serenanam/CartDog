# CartDog
## Summary
I collaborated with two other students to design and prototype the CartDog, a motorized cart that follows the user via Bluetooth and avoids obstacles to help people with disabilities or the elderly easily transport their groceries.

## Project Overview
The CartDog is a motorized cart that follows the user with a control pad via Bluetooth to help people with disabilities or the elderly easily transport their groceries with the touch of a finger.

I was the Head of Programming, in charge of all the programming of the CartDog, and worked with Ayaka Fujita and Ricardo Cortes to build a motorized cart prototype called the CartDog in 10 weeks as part of the NYU EG-UY 1004 Semester Long Design Project. 

## Brainstorm
The idea of the motorized cart was brainstormed to help the elderly to replace carrying or pushing heavy objects for daily activities such as grocery shopping. The responsibilities were broadly split into three parts: Programming, Design, and Circuitry. 

To build the prototype of the CartDog, four VEX wheels, six VEX axles, four large gears, two medium gears, two continuous servo motors, four steel rails, two c-channels, seven wide c-channels, six bearings, 24 spacers, 16 keps nuts, 16 medium screws, 16 shaft collars, two 3D printed connector parts, two 9V batteries, an Arduino Mega 2650, an Adafruit Bluefruit LE Shield, and a breadboard were used.

## Initial Design
A CAD model of a circular three-tier cart with four 360 degree wheels and a Bluetooth bracelet was designed. 

![image](https://github.com/user-attachments/assets/78019fb7-ea0e-427a-8785-f75a1d3b8ccd)
![image](https://github.com/user-attachments/assets/3dec4053-9a8b-4d68-b149-b506ebfbb964)

A circuit diagram of a Raspberry Pi being used to control an Ultrasonic sensor and Bluetooth to connect to DC motors was designed. 

![image](https://github.com/user-attachments/assets/b7d8cdf5-7ed4-4678-bc99-59e302b3cfe2)

A code flow diagram of the Ultrasonic sensor, Bluetooth, and 360 degree wheels was outlined. 

![image](https://github.com/user-attachments/assets/55cfaa59-bb2c-4ee6-82f7-65ba7c8405e2)

## Updated Design
After numerous discussions, we decided to change multiple components of our project. For the motors, we decided to use servo motors instead of DC motors in order to effectively move our cart at a reasonable speed with added weight. We also decided to use VEX wheels instead of 360 turning wheels. We decided to use an Arduino instead of Raspberry Pi because the functions we needed could be done with just an Arduino. Lastly, we ordered a three-tiered rectangular cart instead of a circular cart. 

Therefore, we updated our CAD model to reflect these design changes. 

![image](https://github.com/user-attachments/assets/7a64887e-3f88-4b7b-9d51-7f633f26b628)
![image](https://github.com/user-attachments/assets/75fb977b-44b1-4f44-9ba1-ad5b27ff417f)
![image](https://github.com/user-attachments/assets/6b993ee3-367d-48ae-abf2-ba391450833c)
![image](https://github.com/user-attachments/assets/3264fe27-2368-48e0-8e54-683d3097ac80)

We updated our circuit diagram to show the wiring with two servo motors. 
![image](https://github.com/user-attachments/assets/ea3cb22f-45b5-49ac-ac45-32d7f6d10e36)

We updated our code flow diagram to outline the wheel movement with two motors. 
![image](https://github.com/user-attachments/assets/47794fb8-0111-4525-8b87-a1b362e3e0f8)

## Motors
We used servo motors to power our wheels for the cart. 
![image](https://github.com/user-attachments/assets/ab29f065-eb06-469c-9b83-27b1dc679d88)

Since the axels of the wheels did not fit the servo motors, we designed a 3D printed part to connect the servo motors to the gears. 
![image](https://github.com/user-attachments/assets/6e747743-c153-4304-9123-34d35562c4c4)
![image](https://github.com/user-attachments/assets/3f2140f0-2c2b-4462-9892-1dd92a4a3692)
![image](https://github.com/user-attachments/assets/00dcd926-02af-43bc-b422-3c6b756bb130)

After attaching the servo motors to the cart base and connecting them to the wheels, I coded the servo motors to move forward, backward, right, and left using the Servo library on Arduino IDE.
![image](https://github.com/user-attachments/assets/3ad52d15-7b21-4784-9d40-41ce5c7ad1a9)

## Bluetooth
An Adafruit Bluefruit LE Shield was used to connect the CartDog to a user’s mobile device using the Adafruit_BluefruitLE_nRF51 library.
![image](https://github.com/user-attachments/assets/d304b35e-d1ce-4e1c-9a43-2617b3f697ef)

The Control Pad was programmed to move forward or backward, or turn left or right, depending on the button pressed.
![image](https://github.com/user-attachments/assets/a4aaee81-21a5-4706-9daa-24a41e29cdba)

## Final Design
Due to time limitations, ultrasonic sensors were not used for obstacle avoidance. Additionally, due to shipment delays, trouble with ordering a magnetometer, and difficulties with using GPS sensors indoors, the CartDog was engineered to move based on a control pad instead of automatically following a user’s device. 
 
However, the CartDog features a modular motor base that can be attached to any basket or cart.
![image](https://github.com/user-attachments/assets/168bb7df-1802-415f-aa1a-50e70777214e)
![image](https://github.com/user-attachments/assets/8d0e27ab-2105-4b54-9041-feed115a7a7a)

The CartDog’s final CAD model includes the base of the cart connected to its wheels, axles, and servo motors, and the attachment part between the cart base and the cart or basket. The modifiable cart or basket is depicted with a three-tier cart.
![image](https://github.com/user-attachments/assets/ebfbedae-8c56-4f32-bf26-79052ef8bb00)

The final circuitry components include the Bluefruit Adafruit LE Shield which was soldered onto the Arduino Mega, a breadboard connected to the Arduino mega, two servo motors connected to the breadboard, and two 9V batteries powering the breadboard and Arduino Mega separately.
![image](https://github.com/user-attachments/assets/26568475-617c-4eb9-8b56-02abfab716db)

The final CartDog code programmed the CartDog to move continuously according to the button that is pressed until the button is released using the Servo library and the Adafruit_BluefruitLE_nRF51 library.
![image](https://github.com/user-attachments/assets/f21d2bff-fa7e-4c85-81ce-bbb8befffc8a)


