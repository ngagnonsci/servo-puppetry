# micro bits!

## Welcome! @showdialog
Welcome to the micro:bit! A small circuit board that we can program to do some wonderful and fun things!
Click "Ok" when you instructor tells the whole class to.

## Step 1 
We can change the LEDs on the micro:bit to nearly anything we want. Let's have our make a greeting for when it first starts up. Click next.

## Step 2
Grab a ``||basic:show string||`` block from the ``||basic:basic||`` category. Change what the string says, and drag it into the ``||basic:on start||`` block on the right side of the screen.
```blocks
basic.showString("Hello!!!")```

## Step 3
Download your code and see how it changes on the micro:bit.

## Step 4
After you've done that, change the message in the ``||basic:show string||`` to your name and download the code again.

## Step 5 @showdialog
Great job! Let's get some movement into our programming too. Attach the alligator clips of your servo to the micro:bit.
Brown wire to the "GND", Red wire to the "3V", Yellow wire to the "0"

## Step 6
We want our servo to move every time we press a button, so drag the ``||input:on button A pressed||`` from the ``||input:Input||`` category into your workspace.
```blocks
input.onButtonPressed(Button.A, function () {
	
})```
## Step 7 
From the ``||servos:servos||`` category, drag a ``||servos:set servo ___ angle to ___||`` into the ``||input:onButtonPressed()||`` code.
```blocks
servos.P0.setAngle(90)
```

<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
