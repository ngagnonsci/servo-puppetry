# micro bits and micro servos!
* Open this page at [https://ngagnonsci.github.io/servo-puppetry/beginner-servo](https://ngagnonsci.github.io/servo-puppetry/beginner-servo)
* Follow or test the tutorial at [https://makecode.microbit.org/#tutorial:github:ngagnonsci/servo-puppetry/beginner-servo](https://makecode.microbit.org/#tutorial:github:ngagnonsci/servo-puppetry/beginner-servo)

## Welcome! @showdialog
Welcome to the micro:bit! A small circuit board that we can program to do some wonderful and fun things!
Click "Ok" when you instructor tells the whole class to.

## Step 2 
We can change the LEDs on the micro:bit to nearly anything we want. Let's have add a greeting for when it first starts up. Click next.


## Step 3
Inside the ``||basic:basic||`` category on the left of the screen, grab a ``||basic:show string (   )||`` block. Drag it into the ``||basic:on start||`` block on the right side of the screen and change what the string says. Click the hint (lightbulb) to see what the block looks like.
```blocks
basic.showString("Hello!!!")
```

## Step 4
Download your code by clicking the button on the bottom left of the screen to see how it changes on the micro:bit.

## Step 5
After you've done that, change the message in the ``||basic:show string('hello')||`` to your name and download the code again.

## Step 6 @showdialog
Great job! Let's get some movement into our programming too. Attach the alligator clips of your servo to the micro:bit.

* Black wire to "GND" 
* Red wire to "3V"
* White wire to "0"

![Wiring Diagram](https://ngagnonsci.github.io/servo-puppetry/images/servo-wiring-example.jpg)

## Step 7
We want our servo to move every time we press a button, so drag the ``||input:on button A pressed||`` from the ``||input:Input||`` category into your workspace.
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

## Step 9
We can add even more angles to make the movement change. Computers work really fast though! So if we have more than one position add at least a 500ms ``||basic:pause 500 ms||`` to the code so that the servo completes a movement before starting the next movement. Click the hint to see an example of multiple movements!
```blocks
input.onButtonPressed(Button.A, function () {
servos.P0.setAngle(90)
basic.pause(500)
servos.P0.setAngle(10)
basic.pause(500)
servos.P0.setAngle(65)
})
```

## Step 10 @showdialog
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
