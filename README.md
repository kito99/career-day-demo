# Career Day App

This is a cute demo I used for Career Day at my kids' elementary school (in 2017-2019, 2022-2023 and 2025). It is built using 
[Polymer](https://www.polymer-project.org/) 1.x (perhaps I'll upgrade to [LitElement](https://lit-element.polymer-project.org/) next year).

There are two elements: `career-day-demo` (the demo from Kindergarten) and `career-day-animation-app` (the demo from 1st and 2nd grade  
with added support for two characters). Currently the app is only using `career-day-animation-app`, but you can change `index.html` 
to see the previous (simpler) demo.

`career-day-animation-app` uses HTML5 Canvas to display a background and lets the user move images around on the screen with 
the keyboard.
It currently supports two characters; one can be moved with the arrow keys,
and the other can be moved using W, A, S, an D. 
When the characters reach the end of the canvas they use the Web Speech API to complain. 
If someone clicks on them, they also make a sound.

For the demo, I picked out a "designer", a "product owner", and a "tester" from the class to help me customize the app. The designer got to choose the 
background, and the analyst worked with the rest of the class to choose a character and change what the characters said. Then the designer could 
tweak the size of the characters and the pitch and rate of their voices. I introduced a couple of bugs (such as the key assignments) for the tester
to discover.

I also gave this presentation at [CodeMash/KidzMash](https://www.codemash.org/) 2020, where I added some more characters 
(including baby yoda) and the ability for the characters to make a sound when you click on them. 

It was cool to see which characters and backgrounds each class chose; In 2019, I started keeping a copy the version each class created -- 
see the `src/presentaton-snapshots` folder.

Here's what the app currently looks like:

![screenshot](/images/screenshots/screenshot.png)

However, you can change the image, the size of the characters, and what they say. Here's how it looked during the demo for one of the classes:

![screenshot2](/images/screenshots/screenshot-2.jpg)

# Presentation 

There is an accompanying presentation I gave to the kids before the demo in the `presentation` folder (Keynote format).

# Running the App

## Setup

After cloning the repo, make sure you have Node and npm installed. Install the dependencies:

```
npm install -g bower
```

Next, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed:

```
npm install -g polymer-cli
```

## Viewing Your Application

```
$ polymer serve
```

Then point your browser to: https://localhost:8081 (or whichever port the polymer CLI says it is using)

> NOTE: This will work on any web server; the Polymer CLI is not required. 

## Building Your Application

```
$ polymer build
```

This will create builds of your application in the `build/` directory, optimized to be served in production. You can then serve the built versions by giving `polymer serve` a folder to serve from:

```
$ polymer serve build/default
```
