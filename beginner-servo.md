# micro bits and micro servos!
* Open this page at [https://ngagnonsci.github.io/servo-puppetry/beginner-servo](https://ngagnonsci.github.io/servo-puppetry/beginner-servo)
* Follow or test the tutorial at [https://makecode.microbit.org/#tutorial:github:ngagnonsci/servo-puppetry/beginner-servo](https://makecode.microbit.org/#tutorial:github:ngagnonsci/servo-puppetry/beginner-servo)

```blockconfig.global
basic.pause(500)
```

## Welcome! @showdialog
Welcome to the micro:bit! A small circuit board that we can program to do some wonderful and fun things!
Click "Ok" when you instructor tells the whole class to.

## Examples! @showdialog
By the end of this workshop we will be able to make some cool things like this using a micro:bit and a servo.

THESE ARE PHOTOS OF EXAMPLES 
MAYBE 2 OR 3 OF THEM
![Amanda's Example](https://ngagnonsci.github.io/servo-puppetry/images/Amanda-servo-arm-example.gif)

## Step 2 @showdialog
We can change the LEDs on the micro:bit to nearly anything we want. Let's have add a greeting by using a ``||basic:show string (   )||`` code block.
```blocks
basic.showString("Hello!!!")
```

## Step 3 @showhint
Inside the ``||basic:Basic||`` category on the left of the screen, grab a ``||basic:show string (   )||`` block. Drag it into the ``||basic:on start||`` block on the right side of the screen and change what the string says. Click the hint (lightbulb) to see what these blocks look like.
```blocks
basic.showString("Hello!!!")
```

## Step 4 @showdialog
Download your code by clicking the button on the bottom left of the screen. Look at your micro:bit to see if anything changes!

![Download button](https://ngagnonsci.github.io/servo-puppetry/images/download-button.png)

## Step 4
Download your code by clicking the button on the bottom left of the screen to see how it changes on the micro:bit.

## Step 5 @showdialog
Awesome! Let's see what happens when we change some fo the code. 
Change the message in the ``||basic:show string('hello')||`` to your name and download the code again.
```blocks
basic.showString("My Name")
```

## Step 5
Change the message in the ``||basic:show string('hello')||`` to your name and download the code again.

## Step 6 @showdialog
Great job! Let's get some movement into our programming too. Attach the alligator clips of the servo to your micro:bit.

* Black wire to "GND" 
* Red wire to "3V"
* White wire to "0"

![Wiring Diagram](https://ngagnonsci.github.io/servo-puppetry/images/servo-wiring-example.jpg)

## Step 7 @showdialog
The micro:bit has two buttons on it. We can make things happen when we press these buttons. Let's make the servo to move every time we press the "a" button. Drag the ``||input:on button A pressed||`` from the ``||input:Input||`` category into your workspace.

A PICTURE OF A MICROBIT WITH AN ARROW POINTING TO THE BUTTONS

```blocks
input.onButtonPressed(Button.A, function () {
	
})
```

## Step 8 
From the ``||servos:servos||`` category, drag a ``||servos:set servo ___ angle to ___||`` into the ``||input:onButtonPressed()||`` code.
```blocks
servos.P0.setAngle(90)
```
![Servo Diagram](https://ngagnonsci.github.io/servo-puppetry/images/servo-pic_angle.jpg)

## Step 9 @showdialog
We can add even more angles to make the movement change. Computers work really fast though! So if we have more than one position add at least a 500ms ``||basic:pause 500 ms||`` to the code so that the servo completes a movement before starting the next movement.
```blocks
input.onButtonPressed(Button.A, function () {
servos.P0.setAngle(90)
basic.pause(500)
servos.P0.setAngle(10)
basic.pause(500)
servos.P0.setAngle(65)
})
```

## Step 10 @showhint
Add more ``||servos:set servo ___ angle to ___||`` angles and ``||basic:pause 500 ms||`` blocks to the code.

```blocks
input.onButtonPressed(Button.A, function () {
servos.P0.setAngle(90)
basic.pause(500)
servos.P0.setAngle(10)
basic.pause(500)
servos.P0.setAngle(65)
})
```

## Finished! @showdialog
Great job! Finish this tutorial and remember to download the code onto your micro:bit. 
* What can you attach to the servo arm to make something fun out of this movement?
* What else can you do by coding the micro:bit?

![Servo Example](https://ngagnonsci.github.io/servo-puppetry/images/servo-arm-example.gif)

# config blocks 
