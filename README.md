# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: **Laura Pei**

Time spent: **4** hours spent in total

Link to project: https://glitch.com/edit/#!/spiky-tabby-reward

## Required Functionality

The following **required** functionality is complete:

* [x] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [x] "Start" button toggles between "Start" and "Stop" when clicked. 
* [x] Game buttons each light up and play a sound when clicked. 
* [x] Computer plays back sequence of clues including sound and visual cue for each button
* [x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [x] User wins the game after guessing a complete pattern
* [x] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [x] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [x] Buttons use a pitch (frequency) other than the ones in the tutorial
* [x] More than 4 functional game buttons
* [ ] Playback speeds up on each turn
* [x] Computer picks a different pattern each time the game is played
* [ ] Player only loses after 3 mistakes (instead of on the first mistake)
* [x] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough

Here's a walkthrough of implemented user stories:
Winning condition: 
![](https://i.imgur.com/7pF3tnV.gif)
Losing & stop condition: 
![](https://i.imgur.com/W1vObzE.gif)


## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
https://www.w3schools.com/

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 
When working on the submission, one challenge I encountered was getting the images to appear only when the buttons were clicked. When I tried adding code to make the image appear in the script.js file, I ran into styling issues with making the image appear with correct spacing when the user clicked on a button. In the end, I decided to keep the image on the button, no matter whether the button was pressed or not. I also left space for the original color so that we can still see which button is active.
Another challenge I ran into was figuring out how to make the randomization pattern work. I started by researching `Math.random()`, learning that it outputted numbers from 0 to 1. I used `console.log` to play around with the numbers. I figured out that I can multiply the result from `Math.random()` with 6, which is the number of buttons that I had, to get a random number generated between those values. From here, I made a `generatePattern()` function, where I would use a for loop to randomly choose and assign all the values of the list. I then called `generatePattern()` in the line where pattern was originally assigned. This was ultimately the algorithm that I used in my code.


3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
After completing my submission, some questions I had about web development were how I could further expand my horizons after understanding these basic building blocks. Looking at some of the websites that I interact with daily, I know that there's still a lot to learn. I'm curious about what other tools we can use  that work alongside HTML, CSS, and JavaScript in order to create beautiful and functional websites. For one, I'm interested in learning a little bit more about how we can store data persistently such that I can add and delete from this database, whether I'm restarting the server or not.

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 
If I had a few more hours to work on this project, I would spend them trying to figure out the original challenge I ran into, which was making the images appear only when the button is active. In addition, I would try to make the game more complex by implementing some more optional features suggested, and doing some more research on different HTML, CSS, or JavaScript to see what else I can implement from here. For example, if I looked into CSS, I’d implement the `:hover` selector and see if I can make the website more interactive rather than keeping it static. It would also be really fun to implement audio that matched the images I chose. 



## License

    Copyright Laura Pei

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
