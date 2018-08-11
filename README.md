# Career Day App

This is a cute demo I used for Career Day at my daughter's school in Kindergarten and 1st grade. It is built using [Polymer](https://www.polymer-project.org/) 1.x (perhaps I'll upgrade to Polymer 3 next year).

There are two elements: `career-day-demo` (the demo from Kindergarten) and `career-day-animation-app` (the demo from 1st grade 
with added support for two characters). Currently the app is only using `career-day-animation-app`, but you can change `index.html` 
to see the previous (simpler) demo.

`career-day-animation-app` uses HTML5 Canvas to display a background and lets the user move images around on the screen with 
the keyboard. It currently supports two characters; one can be moved with the arrow keys, and the other can be moved using S, E, D, and X. 
When the characters reach the end of the canvas, they use the Web Speech API to complain. 

For the demo, I picked out a "designer" and a "business analyst" from the class to help me customize the app. The designer got to choose the 
background, and the analyst worked with the rest of the class to choose a character and change what the characters said. 
(It was cool to see which characters and backgrounds each class chose).

Here's what the app currently looks like:

![screenshot](/images/screenshot.png)

However, you can easily change the image, the size of the characters, and what they say. Here's how it looked during the demo for one of the classes:

![screenshot2](/images/screenshot-2.jpg)

# Presentation

There is an accompanying presentation I gave to the kids before the demo in the `presentation` folder (Keynote format).

# Running the App

## Setup

After cloning the repo, make sure you have Node and npm installed. Install the dependencies:

```
npm install
```

Next, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed:

```
npm install -g polymer-cli
```

## Viewing Your Application

```
$ polymer serve
```

## Building Your Application

```
$ polymer build
```

This will create builds of your application in the `build/` directory, optimized to be served in production. You can then serve the built versions by giving `polymer serve` a folder to serve from:

```
$ polymer serve build/default
```
