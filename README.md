# svg-animation 
using HTML, CSS, and 3 lines of JavaScript!
SVG animation did with Dev ED video:

uses Figma to construct the background and Word"Designer"
To create just made a Rectangle and use the Text button to write the text, "Designer". You can use any word you want. 
For the Word added a stroke of 5, and no fill then right Click and use the Copy as SVG 
then place the code into  the body of the HTML file your text editor  of your choice. This should be your index.html file.

Then add an id to your svg element such as "logo" you gonna use this to style your CSS to make the letter animate.
Style your CSS:
Use transform:translate(-50%,-50%) with position: absolute for top & left @ 50% to center the "logo".
https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function/translate
To Animate:
To find each path you have to  use a little javascript loop through the logo path length to get each assign path for each letter.  Start by  document.query all for the logo path. 
Then  to get each path to animate its letter because you have to loop through each path so you can use stroke-dasharray and stroke-dashoffset for each letter path see https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/stroke-dasharray and https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/stroke-dashoffset
 Make sure  you console.log  to get the total length of each path so you can input it in the css.
 Now add each path to your index.css file by using the :nth-child with the stroke-dasharray, stroke-dashoffset, animation with line-anim:(see below for more info) to animate the word
 Last but not less don't forget your keyframes:  https://developer.mozilla.org/en-US/docs/Web/CSS/@keyframes also I added an article I found on Medium for line-animation by Max Houston Oppenheimer if you need more clarification.
 https://dev.to/oppnheimer/you-too-can-animate-svg-line-animation-jgm
