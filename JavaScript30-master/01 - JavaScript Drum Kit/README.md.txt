**This code was not created by me, it's based on a tutorial and learning purposes**

Notes about Day 1 Project

Title: Javascript Drum Kit

Purpose: Associate Keys pressed on a keyboard to pair with data-key's assigned to sounds in our html

*This project came with all the css and html.  No Javascript was written yet.

First of all used the window event listenter to check for 'keydown'.

To test that we were actually grabbing that, we console.logged the value.

The correct data key's can be found by inspecting the page elements in a browser and pressing the keys that you want to assign sounds to

Created a function that handles playing the sounds called playSound(e), accepts the window event as a parameter

**This function uses query Selector on the document and grabs key codes.  We compare the key codes to our data-key values in our html.

-------------------------------------------------------------------------------

We wrote functionallity for pressing same key on the keyboard to get the sound to repeat.

used the audio.currentTime property and set it to 0.
also used the audo.play() method to play the sound.

The key's needed to have access to the .playing class in our css, so we used the key's classList and added to it.  

-------------------------------------------------------------------------------

Ran into the issue of the animation never going away after a key was pressed, so we wrote a function for removing the transition

Bassically we used this (instance) this.classList.remove('playing').  We removed the 'playing' class our keys.  

We also checked if every key had the propertyName of 'transform' 

----
The page activley listens for the keys transitioend property to become true.  when that happens removeTransition is called.
-----------------------------------------------------------------------------

**Take Aways**

I Feel like I learned more about what you developer can access from the DOM through the window model. also learned a little more about how 'this' works.

It was neat to learn how data-keys in html worked and that they can work can be useful for javascript.