    LEVEL 1         

KERALA IOT CHALLENGE( 2021 - 22 )
---------------------------------

LEVEL 1 - EXPERIMENTS
---------------------

### *   [EXP1-- Hello World LED Blinking](#exp01)
*   [EXP2-- Traffic Light](#exp02)
*   [EXP3-- LED Chasing Effect](#exp03)
*   [EXP4-- Button Controlled LED](#exp04)
*   [EXP5-- Buzzer](#exp05)
*   [EXP6-- RGB LED](#exp06)
*   [EXP7-- LDR Light sensor](#exp07)
*   [EXP8-- Flame sensor](#exp08)
*   [EXP9-- LM35 Temperature Sensor](#exp09)
*   [EXP10-- IR Remote Control Using TSOP](#exp10)
*   [EXP11-- Potentiometer analog Value Reading](#exp11)
*   [EXP12-- 7 Segment Display](#exp12)

\-- Experiment01 --
===================

  

### Components Required

  

*   Arduino UNO
*   A Breadboard
*   Male to male jumper wires (x2)
*   LED
*   USB cable to connect the arduino
*   Resistor

  

### Circuit Diagram

  
![](site\images\exp01.png)

### Code

```
 void setup()  
    {  
    pinMode(10, OUTPUT);  
    }  
    void loop()  
    {  
    digitalWrite(8, HIGH);  
    delay(1000); // Wait for 1000 millisecond(s)  
    digitalWrite(8, LOW);  
    delay(1000); // Wait for 1000 millisecond(s)  
    }
```

### Video Tutorial

  
[Go to Top](#top)

\-- Experiment02 --
===================

### Components Required

  

*   Arduino board \*1
*   USB cable \*1
*   Red M5 LED\*1
*   Yellow M5 LED\*1
*   Green M5 LED\*1
*   220Ω resistor \*3
*   Breadboard\*1
*   Breadboard jumper wires\* several

  

### Circuit Diagram

  
![](site\images\exp02.png)

### Code

 ``` 
 int redled =10; // initialize digital pin 8.  
    int yellowled =7; // initialize digital pin 7.  
    int greenled =4; // initialize digital pin 4.  
    void setup()  
    {  
    pinMode(redled, OUTPUT);// set the pin with red LED as “output”  
    pinMode(yellowled, OUTPUT); // set the pin with yellow LED as “output”  
    pinMode(greenled, OUTPUT); // set the pin with green LED as “output”  
    }  
    void loop()  
    {  
    digitalWrite(greenled, HIGH);//// turn on green LED  
    delay(5000);// wait 5 seconds  
    digitalWrite(greenled, LOW); // turn off green LED  
    for(int i=0;i<3;i++)// blinks for 3 times  
    {  
    delay(500);// wait 0.5 second  
    digitalWrite(yellowled, HIGH);// turn on yellow LED  
    delay(500);// wait 0.5 second  
    digitalWrite(yellowled, LOW);// turn off yellow LED  
    }  
    delay(500);// wait 0.5 second  
    digitalWrite(redled, HIGH);// turn on red LED  
    delay(5000);// wait 5 seconds  
    digitalWrite(redled, LOW);// turn off red LED  
    }
```

### Video Tutorial

  
[Go to Top](#top)

\-- Experiment03 --
===================

### Components Required

  

*   Arduino UNO
*   A Breadboard
*   Male to male jumper wires (x2)
*   LED
*   USB cable to connect the arduino
*   Resistor

  

### Circuit Diagram

  
![](site\images\exp03.png)

### Code

 ``` 
 int BASE = 2 ; // the I/O pin for the first LED  
    int NUM = 6; // number of LEDs  
    void setup()  
    {  
    for (int i = BASE; i < BASE + NUM; i ++)  
    {  
    pinMode(i, OUTPUT); // set I/O pins as output  
    }  
    }  
    void loop()  
    {  
    for (int i = BASE; i < BASE + NUM; i ++)  
    {  
    digitalWrite(i, LOW); // set I/O pins as “low”, turn off LEDs one by one.  
    delay(200); // delay  
    }  
    for (int i = BASE; i < BASE + NUM; i ++)  
    {  
    digitalWrite(i, HIGH); // set I/O pins as “high”, turn on LEDs one by one  
    delay(200); // delay  
    }  
    }
```

### Video Tutorial

  
[Go to Top](#top)

[GTech - Group of Technology](index.html) [ABOUT ME](aboutme.html)  
  
  
[LEVEL 1](level1.html) [LEVEL 2](level2.html) [LEVEL 3](level3.html) [LEVEL 4](level4.html)

 [![](site/assets/img/common/fsoc-youtube.png)](https://www.youtube.com/channel/UCGkitrEFM78C0YXJgZoWYZA) [ ![](site/assets/img/common/fsoc-facebook.png) ](https://www.facebook.com/gooddaywork/) [ ![](site/assets/img/common/fsoc-instagram.png) ](https://www.linkedin.com/company/goodday-work) [ ![](site/assets/img/common/fsoc-twitter.png) ](https://twitter.com/gooddaywork) [![](site/assets/img/common/fsoc-email.png)](mailto:info@goodday.work)
