# Career Day App

This is a cute demo I used for Career Day at my daughter's school in Kindergarten and 1st grade (2018). It is built using [Polymer](https://www.polymer-project.org/) 1.x (perhaps I'll upgrade to Polymer 3 next year).

There are two elements: `career-day-demo` (the demo from Kindergarten) and `career-day-animation-app` (the demo from 1st grade 
with added support for two characters). Currently the app is only using `career-day-animation-app`, but you can change `index.html` 
to see the previous (simpler) demo.

`career-day-animation-app` uses HTML5 Canvas to display a background and lets the user move images around on the screen with 
the keyboard. It currently supports two characters; one can be moved with the arrow keys, and the other can be moved using S, E, D, and X. 
When the characters reach the end of the canvas, they use the Web Speech API to complain. 

For the demo, I picked out a "designer" and a "business analyst" from the class to help me customize the app. The designer got to choose the 
background, and the analyst worked with the rest of the class to choose a character and change what the characters said. Then the designer could 
tweak the size of the characters and the pitch and rate of their voices. 

It was cool to see which characters and backgrounds each class chose; In 2019, I started keeping a copy the version each class created -- see the `src/2019` folder.

![screenshot](/images/screenshot.png)

There is an accompanying presentation I gave to the kids before the demo in the `presentation` folder (Keynote format).

## Install the Polymer-CLI

In order to run the app, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. 

## Viewing Your Application

```
$ polymer serve
```
