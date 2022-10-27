# micro bits!
Open this page at [https://ngagnonsci.github.io/servo-puppetry/](https://ngagnonsci.github.io/servo-puppetry/)
Load this as a tutorial at [https://makecode.microbit.org/#tutorial:github:ngagnonsci/servo-puppetry/README](https://makecode.microbit.org/#tutorial:github:ngagnonsci/servo-puppetry/README)

```package
microbit-servos
```

## Welcome! @showdialog
Welcome to the micro:bit! A small circuit board that we can program to do some wonderful and fun things!
Click "Ok" when you instructor tells the whole class to.

## Step 1 
We can change the LEDs on the micro:bit to nearly anything we want. Let's have our make a greeting for when it first starts up. Click next.

## Step 2
Grab a `[basic.showString()]` block from the ``|basic:Basic|`` category. Change what the string says, and drag it into the `[basic.forever(function (){})]` block on the right side of the screen.
```blocks
basic.showString("Hello!!!")
```

## Step 3
Download your code and see how it changes on the micro:bit.

## Step 4
After you've done that, change the message in the `[basic.showString('   ')]` to your name and download the code again.

## Step 5 @showdialog
Great job! Let's get some movement into our programming too. Attach the alligator clips of your servo to the micro:bit.
Brown wire to the "GND", Red wire to the "3V", Yellow wire to the "0"

## Step 6
We want our servo to move every time we press a button, so drag the `[input.onButtonPressed(Button.A, function() {})]` from the ``|input:Input|`` category into your workspace.
```blocks
input.onButtonPressed(Button.A, function () {
	
})
```
## Step 7 
From the ``||servos:servos||`` category, drag a ``||servos:set servo ___ angle to ___||`` into the `[input.onButtonPressed(Button.A, function() {})]` code.
```blocks
servos.P0.setAngle(90)
```