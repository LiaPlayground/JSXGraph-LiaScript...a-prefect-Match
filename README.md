<!--
author:   André Dietrich; Sebastian Zug
email:    LiaScript@web.de
version:  1.0.0

language: en

narrator: English Female

comment:  45-minute interactive conference presentation introducing the JSXGraph community to LiaScript. Shows how to transform mathematical visualizations into complete learning experiences using `@JSX.Graph`, `@JSX.Script`, and `@JSX.Eval` macros. Features live demos, multimedia integration, and hands-on examples that work everywhere - from smartphones to feature phones. Perfect symbiosis of mathematical visualization power and educational storytelling magic!

logo:     assets/img/logo.jpg

import:   https://raw.githubusercontent.com/liaTemplates/JSXGraph/main/README.md
          https://raw.githubusercontent.com/liaTemplates/ABCjs/main/README.md
          https://raw.githubusercontent.com/LiaTemplates/LiveEdit-Embeddings/refs/heads/main/README.md

@style
@keyframes burn {
  0% { text-shadow: 0 0 5px #ff0, 0 0 10px #ff0, 0 0 15px #f00, 0 0 20px #f00, 0 0 25px #f00, 0 0 30px #f00, 0 0 35px #f00;
  }
  50% { text-shadow: 0 0 10px #ff0, 0 0 15px #ff0, 0 0 20px #ff0, 0 0 25px #f00, 0 0 30px #f00, 0 0 35px #f00, 0 0 40px #f00;
  }
  100% { text-shadow: 0 0 5px #ff0, 0 0 10px #ff0, 0 0 15px #f00, 0 0 20px #f00, 0 0 25px #f00, 0 0 30px #f00, 0 0 35px #f00;
  }
}

.burning-text {
  font-weight: bold;
  color: #fff;
  animation: burn 1.5s infinite alternate;
}
@end

@burn: <span class="burning-text">@0</span>
-->

# JSXGraph & LiaScript ... a perfect Match

|                                            Sebastian Zug                                             |                                             André Dietrich                                              |
| :--------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------: |
| ![Sebastian Zug](https://liascript.github.io/images/author/sebastian-zug_hu6238929735416752404.webp)<!-- style="border-radius: 50%" --> | ![André Dietrich](https://liascript.github.io/images/author/andre-dietrich_hu15822190180767231119.webp)<!-- style="border-radius: 50%" --> |
|      [Sebastian.Zug\@informatik.tu-freiberg.de](mailto:Sebastian.Zug@informatik.tu-freiberg.de)      |      [Andre.Dietrich\@informatik.tu-freiberg.de](mailto:Andre.Dietrich@informatik.tu-freiberg.de)       |
| https://tu-freiberg.de/soro | https://liascript.github.io |

    {{1}}
<section>

## What will we learn today? 🚀

- **From Demo to Course**: Transform your beautiful visualizations into complete learning experiences
- **Zero Installation Headaches**: One markdown file = works everywhere (seriously, even on Nokia 3310!)
- **Assessment Made Easy**: Add quizzes, tasks, and interactive elements around your graphs
- **"It's just Markdown!"**: No new languages, no build processes, no deployment nightmares

</section>


    {{2}}
<section>

## Resources:

- GitHub Project:

  https://github.com/LiaPlayground/JSXGraph-LiaScript...a-prefect-Match

- LiaScript rendered version:

  https://liascript.github.io/course/?https://raw.githubusercontent.com/LiaPlayground/JSXGraph-LiaScript...a-prefect-Match/refs/heads/main/README.md

- Editing version:

  https://liascript.github.io/LiveEditor/?/show/file/https://raw.githubusercontent.com/LiaPlayground/JSXGraph-LiaScript...a-prefect-Match/refs/heads/main/README.md

</section>


## Hello LiaScript - Quick Introduction

    --{{0}}--
Alright, let's start with the million-dollar question: "What exactly IS LiaScript?" Well, imagine if Markdown had a baby with interactive superpowers - that's LiaScript! You already know Markdown is fantastic - you probably use it for documentation, README files, maybe even presentations. But here's the thing: Markdown is @burn(static as hell)! Your beautiful JSXGraph demos deserve so much more than static documentation, don't they?
!?[](assets/vid/speaker.webm#t=0,25)



    --{{1}}--
But here's where it gets exciting for you JSXGraph creators: What if the same Markdown that describes your math concepts could ALSO become interactive visualizations? In LiaScript, a simple data table magically transforms into charts, graphs, or interactive elements - just like your JSXGraph demos, but built right into the narrative!
!?[](assets/vid/speaker.webm#t=25,43)

      {{1-2}}
| Language  | Popularity | Learning Curve | Interactivity |
| --------- | ---------: | -------------: | ------------: |
| HTML      |         90 |             30 |            20 |
| Markdown  |         95 |             10 |             5 |
| LiaScript |          1 |             15 |            95 |

    --{{2}}--
Another tabular structure might generate another type of graph:
!?[](assets/vid/speaker.webm#t=43,47)

     {{2-3}}
<!--
data-type="heatmap"
data-title="Seattle Average Temperature in Fahrenheit"
data-show
-->
| Seattle |  Jan |  Feb |  Mar |  Apr |  May |  Jun |  Jul |  Aug |  Sep |  Oct |  Nov |  Dec |
| -------:| ----:| ----:| ----:| ----:| ----:| ----:| ----:| ----:| ----:| ----:| ----:| ----:|
|       0 | 40.7 | 41.5 | 43.6 | 46.6 | 51.4 | 56.0 | 60.5 | 61.2 | 57.0 | 50.1 | 44.1 | 39.6 |
|       2 | 40.2 | 40.7 | 42.7 | 45.3 | 50.0 | 54.4 | 58.5 | 59.2 | 55.4 | 49.2 | 43.5 | 39.3 |
|       4 | 39.7 | 40.0 | 41.9 | 44.4 | 48.9 | 53.2 | 57.0 | 57.7 | 54.2 | 48.6 | 43.1 | 38.9 |
|       6 | 39.6 | 39.5 | 41.3 | 44.2 | 49.5 | 54.2 | 57.8 | 57.4 | 53.6 | 48.2 | 42.8 | 38.7 |
|       8 | 39.6 | 39.9 | 42.9 | 47.1 | 52.7 | 57.3 | 61.3 | 61.1 | 56.7 | 49.5 | 43.1 | 38.7 |
|      10 | 41.3 | 42.7 | 46.4 | 50.7 | 56.4 | 60.9 | 65.2 | 65.4 | 60.9 | 52.8 | 45.5 | 40.4 |
|      12 | 43.8 | 46.0 | 49.5 | 53.8 | 59.6 | 64.3 | 69.4 | 69.8 | 65.1 | 56.0 | 47.8 | 42.6 |
|      14 | 45.1 | 47.7 | 51.3 | 55.9 | 61.9 | 66.9 | 72.6 | 73.2 | 67.7 | 57.8 | 48.8 | 43.6 |
|      16 | 44.5 | 47.5 | 51.4 | 55.9 | 62.3 | 67.5 | 73.9 | 74.3 | 68.2 | 57.4 | 47.8 | 42.6 |
|      18 | 42.6 | 44.7 | 48.7 | 53.8 | 60.3 | 65.9 | 72.3 | 72.2 | 64.6 | 53.9 | 46.0 | 41.2 |
|      20 | 42.0 | 43.3 | 46.4 | 50.2 | 56.0 | 61.4 | 66.9 | 66.6 | 60.7 | 52.3 | 45.2 | 40.7 |
|      22 | 41.4 | 42.5 | 45.0 | 48.3 | 53.5 | 58.2 | 63.2 | 63.5 | 58.7 | 51.1 | 44.5 | 40.1 |

    --{{3}}--
And of course, I support multimedia content - such as audio:
!?[](assets/vid/speaker.webm#t=47,51)

     {{3-4}}
?[Spotify: Melankolia by Sofia Rutaru](https://open.spotify.com/intl-de/track/76ixwvY9idAF6m9c5rpF3k)

    --{{4}}--
Video too, and as you can see from the demo below, I run on feature phones as well, even if they are offline!
!?[](assets/vid/speaker.webm#t=51,58)


     {{4-5}}
!?[LiaScript on Nokia](https://www.youtube.com/watch?v=U_UW69w0uHE)

    --{{5}}--
But, it is also possible to embed interactive elements from different sites directly, whereby I will try to figure out the best representation for the respective device automatically.
!?[](assets/vid/speaker.webm#t=58,68)

     {{5-6}}
??[The Diagonal of a Square tablet](https://sketchfab.com/3d-models/the-diagonal-of-a-square-tablet-605c9d9573d14b52b8880e14c826e133 "The diagonal of a square tablet” by IPHC Digitzation Lab, on Sketchfab (CC BY 4.0).")

    --{{6}}--
And here's a fun bonus - LiaScript doesn't just handle mathematical visualizations! Want to add some musical notation to your math lessons? Easy! Check this out:
!?[](assets/vid/speaker.webm#t=68,78.5)

     {{6-8}}
```abc
T: GLUECK AUF DER STEIGER KOEMMT
O: Europa, Mitteleuropa, Deutschland
R: Stände -, Bergmanns - Lied
M: 4/4
L: 1/16
K: G
| G8F4A4 | G8z8 | B8A4c4 | B8z4 G2A2 |
B4B4B4A2B2 | c4A3AA4 A2B2 | c4c4c4B2c2 |
d4B3BB4 A4 | G8F8 | G4e4d4 c2A2 | B8A8 | G8z8
```
@ABCJS.eval

    --{{7}}--
The point is: LiaScript isn't just another documentation tool - it's about creating engaging, interactive learning experiences that work everywhere! Mathematical visualizations, musical notation, multimedia content - everything your learners need in one unified platform. And the best part? Your JSXGraph visualizations fit perfectly into this rich ecosystem!
!?[](assets/vid/speaker.webm#t=78.5,99)


    --{{8}}--
So let me put this in perspective for you JSXGraph creators: LiaScript is essentially Markdown with superpowers! And I mean REAL superpowers! You already know Markdown - it's clean, simple, universally supported. But LiaScript takes that familiar foundation and adds incredible interactive capabilities. Multimedia that works everywhere - from desktop to feature phones. Text-to-Speech that can make your mathematical explanations accessible to everyone. JavaScript execution - yes, that includes all your beautiful JSXGraph code! And here's the key: an extensible macro system that transforms your JSXGraph visualizations into educational experiences. This is where the magic happens, folks!
!?[](assets/vid/speaker.webm#t=99,142)

      {{8}}
> **LiaScript = Markdown + @burn(Superpowers)**
>
> - 📝 The Markdown you already know and love
> - 🎬 Multimedia that just works everywhere
> - 🔊 Text-to-Speech for accessibility (imagine your graphs talking!)
> - ⚡ JavaScript execution (yes, including JSXGraph!)
> - 🧩 **Extensible macro system** ← This is where your JSXGraph magic happens!

    --{{9}}--
Now I can see you thinking: "Okay, this sounds cool, but how does this actually help MY JSXGraph work?" That's EXACTLY what we're diving into next! You bring the mathematical visualization genius - JSXGraph. LiaScript brings the storytelling, assessment, and "works-everywhere" magic. Together? They're absolutely perfect! Let me show you how...
!?[](assets/vid/speaker.webm#t=142)

### Let's see where we're starting from! 🎯

> **Quick Community Check: Your LiaScript Journey?**
>
> - [(none)]  "LiaScript? Never heard of it!" (Don't worry, you're about to love it!)
> - [(heard)] "Heard the name, never tried it" (Perfect timing!)
> - [(tried)] "Played with it a bit" (Great, you know the basics!)
> - [(user)]  "I'm already using it regularly" (Awesome, spread the word!)

## How JSXGraph Becomes LiaScript Magic! ✨

    --{{0}}--
Now here's where it gets really exciting for you JSXGraph creators! You might be wondering: "How exactly does my JSXGraph code become part of this LiaScript magic?" Well, the beautiful thing about LiaScript is that it was built from day one to welcome your visualizations with open arms! It's incredibly extensible, and JSXGraph fits in like it was always meant to be there.

    --{{0}}--
Think of it this way: LiaScript has two superpowers that make JSXGraph integration absolutely seamless. First, JavaScript is a first-class citizen - your JSXGraph code runs natively, no translation needed! Second, LiaScript has a macro system that's like giving your code superpowers. When you combine these two features? That's when your mathematical visualizations transform into complete interactive learning experiences!

    --{{1}}--
Let me show you the two building blocks that make this magic possible, and then we'll dive into the JSXGraph integration that will blow your mind:

      {{1}}
> **🚀 Building Block 1: Native JavaScript Power**  
> Your JSXGraph code runs directly - no compilation, no translation, just pure mathematical visualization magic!
>
> **🧩 Building Block 2: Macro System Superpowers**  
> Transform your code into interactive educational experiences with simple, reusable macros!

### JavaScript as First-Class Citizen 🚀

    --{{0}}--
Here's what makes LiaScript perfect for your JSXGraph code: JavaScript isn't some afterthought or hack - it's a first-class citizen! Unlike other Markdown systems or notebooks where JavaScript feels bolted on, LiaScript was designed from the ground up to embrace your code. Your JSXGraph visualizations run natively, directly in the browser, exactly as you intended. No weird wrapper functions, no translation layers, no "please work" moments.

     {{0-2}}
Russia started its invasion of Ukraine
<script format="relativetime" unit="day">
// Define the start date of the invasion
const invasionStartDate = new Date('2022-02-24');

// Get the current date
const currentDate = new Date();

// Calculate the difference in milliseconds
const differenceInMs = currentDate - invasionStartDate;

// Convert milliseconds to days
const differenceInDays = differenceInMs / (1000 * 60 * 60 * 24);

// Calculate the number of full days
const daysSinceInvasion = Math.floor(differenceInDays);

-daysSinceInvasion
</script>.

    --{{1}}--
The code execution is highlighted by the background color of the result and By double-clicking or tabbing on the result of the calculation, the script can be inspected and modified by the learners.


      {{2-4}}
****************************************************************************************

    --{{2}}--
Additionally, scripts can be annotated with any kind of input type. Allowing them to control the execution of the script. The input possibility is highlighted by the border. `@input` is simply a placeholder for the current value of the input, whereby `output` defines something like a topic under which the value is published.


longitude: <script default="13.33125" input="range" output="longitude">@input</script>

latitude: <script default="50.92558" input="range" output="latitude">@input</script>

    --{{3}}--
The example below shows how to use these input values to query the Open-Meteo weather API and display the result as a table. Any other scripts can subscribe to these values by using `@input(\`latitude\`)` and every time the output changes the script is re-executed. When the result is send back to LiaScript using `send.lia(...)`, it is interpreted as LiaScript again (HTML is also possible), so you can use all the features of LiaScript to display the result.

<script run-once="true" style="display: block">
  fetch("https://api.open-meteo.com/v1/forecast?latitude=@input(`latitude`)&longitude=@input(`longitude`)&hourly=temperature_2m")
    .then(response => response.json())
    .then(data => {
      let table = "<!-- data-show data-type='line' data-title='Open-Meteo Weather API (@input(`latitude`) - @input(`longitude`))' -->\n"

      table += "| Time | Temperature |\n"
      table += "| ---- | ----------- |\n"

      for (let i=0; i < data.hourly.time.length; i++) {
        table += "| " + data.hourly.time[i] + " | " + data.hourly.temperature_2m[i] + " |\n"
      }
      send.lia("LIASCRIPT: "+table) }
    )
    .catch(e => {
      send.lia("ups, something went wrong")
    })
  "waiting for the weather"
</script>

***************************************************************************************


    --{{4}}--
Finally, if you work with code and you want to make it editable and executable like in a real software project, then you can bind a script to a code block. This way the code is not only nicely formatted, but also directly executable and editable by the learners.


     {{4}}
``` js     -EvalScript.js
let who = data.first_name + " " + data.last_name;

if(data.online) {
  who + " is online"; }
else {
  who + " is NOT online"; }
```
``` json    +Data.json
{
  "first_name" :  "Sammy",
  "last_name"  :  "Shark",
  "online"     :  true
}
```
<script>
  // insert the JSON dataset into the local variable data
  let data = @input(1);

  // eval the script that uses this dataset
  eval(`@input(0)`);
</script>



### Macro System Superpowers 🧩
<!--
@highlight: <span style="color: @0">__@1__</span>
-->

    --{{0}}--
And here's the second superpower: macros! Think of macros as your personal assistants that take your JSXGraph code and transform it into educational experiences. Instead of writing the same setup code over and over again, you create a macro once, and then you can reuse it with different parameters. Want to create ten different function graphs with different colors? Easy! Want to build interactive geometry lessons with consistent styling? Done! Macros make your JSXGraph code reusable, shareable, and absolutely powerful.

Let me show you how simple this is:

@highlight(red, Your JSXGraph code) becomes @highlight(blue, an educational experience) with just one line!

## JSXGraph Integration - "Your Math Visualization Dreams Come True!" 🚀

    --{{0}}--
Alright, here's where the real magic happens! You've been creating incredible mathematical visualizations with JSXGraph, and now I'm going to show you how to supercharge them with LiaScript. Ready for this? The entire JSXGraph extension for LiaScript is waiting for you at:

https://github.com/LiaTemplates/JSXGraph

    --{{1}}--
But here's the beautiful part - you don't need to understand the internals! Want to use JSXGraph in your LiaScript document? Just add ONE line to your document header: `@import` the extension URL, and boom! You've got all the JSXGraph superpowers at your fingertips. No installation, no build process, no configuration headaches. Just pure mathematical visualization magic!

      {{1}}
```` markdown  @embed
<!--
import: https://raw.githubusercontent.com/liaTemplates/JSXGraph/main/README.md
-->

# Your JSXGraph Magic in LiaScript

```js \@JSX.Graph
board = JXG.JSXGraph.initBoard(BOARDID, { boundingbox: [-12, 12, 12, -12], keepaspectratio: true });
 
 var a = board.create('slider', [[1, -1], [5, -1], [0, 0.3, 1]], { name: 'a' });
 var b = board.create('slider', [[1, -2], [5, -2], [0, 0.7, 1]], { name: 'b' });
 var tau = board.create('slider', [[-5, -3], [5, -3], [0, 0, 0.5]], { name: 'τ' });
 
 for (var i = 0; i < 8; i++) {
     // Use closures to define the 8 curves
     (function(x) { return board.create('curve', [
            (phi) => a.Value() * Math.exp(b.Value() * (phi + Math.PI * x * 0.25 + tau.Value() * Math.PI)), 
            [0, 0], 
            -4 * Math.PI, 8 * Math.PI],
            { curveType: 'polar', strokewidth: 1 }
         );
     })(i);
 }
```
````

    --{{2}}--
There are more templates available here:

      {{2}}
https://github.com/topics/liascript-template


### Method 1: `@JSX.Graph` - "Pure Mathematical Beauty" ✨

    --{{0}}--
Here's your first magic spell! Want to embed a JSXGraph directly into your LiaScript document? Just type `@JSX.Graph` above any JavaScript code block, and watch the magic happen! LiaScript takes your code and transforms it into a living, breathing mathematical visualization. It's that simple - no complex setup, no external dependencies, just pure mathematical beauty rendered instantly!


``` js @JSX.Graph
board = JXG.JSXGraph.initBoard(BOARDID, {axis:true, boundingbox:[-1/2, 1/2, 1/2, -1/2]});
 
var g = board.create('functiongraph', ["2*x*sin(1/x) - cos(1/x)"], {strokeColor: 'red'});
var f = board.create('functiongraph', ["x^2*sin(1/x)"], {strokeWidth:2});
```

### Method 2: `@JSX.Script` - "Interactive Learning Paradise" 🎮

    --{{0}}--
But wait, it gets even better! Meet `@JSX.Script` - your learners' new best friend! Not only does it render your beautiful JSXGraph visualization, but learners can double-click or tab to inspect and modify the code in real-time! Imagine students experimenting with your mathematical concepts, tweaking parameters, seeing immediate results. This is interactive learning at its absolute finest!


``` js @JSX.Script
board = JXG.JSXGraph.initBoard(BOARDID, {
    boundingbox: [-12, 8, 12, -8],
    keepaspectratio: false,
    axis: false,
    pan: {
        needTwoFingers: true
    }
});

var a = board.create('slider', [[-6, -7], [1, -7], [0, 0.5, 2]]);

const view = board.create('view3d',
    [
        [-6, -3],
        [8, 8],
        [[-3, 3], [-3, 3], [-3, 3]]
    ], {});

var vf = view.create('vectorfield3d', [
    [(x, y, z) => Math.cos(y), (x, y, z) => Math.sin(x), (x, y, z) => z],
    [-2, 5, 2], // x from -2 to 2 in 5 steps
    [-2, 5, 2], // y
    [-2, 5, 2] // z
], {
    strokeColor: 'red',
    scale: () => a.Value()
});
```

### Method 3: `@JSX.Eval` - "The Mathematical Playground" 🏗️

    --{{0}}--
And here's the ultimate tool for mathematical exploration: `@JSX.Eval`! This transforms your JSXGraph code into a complete development environment right inside the document. Students can edit, experiment, and see results instantly - with a built-in version history! It's like giving every learner their own mathematical laboratory. Changes persist in the browser, so they can return to their experiments anytime. Pure educational gold!

```js
board = JXG.JSXGraph.initBoard(BOARDID, {
  boundingbox: [-5, 5, 5, -5],
  axis: false,
  showNavigation: false,
  zoom: {
    enabled: false
  },
  pan: {
    enabled: false
  }
});
 
var view = board.create(
  'view3d',
  [[-2.5, -4], [5, 8], [[-2, 2], [-2, 2], [-2, 2]]],
  {
    projection: 'central',
    trackball: {enabled: true},
    depthOrder: {enabled: true},
    xAxis: {visible: false},
    yAxis: {visible: false},
    zAxis: {visible: false},
    xPlaneRear: {visible: false},
    yPlaneRear: {visible: false},
    zPlaneRear: {fillOpacity: 0.2, visible: false}
});

let rho = 1.6180339887;
let vertexList = [
  [0, -1, -rho], [0, +1, -rho], [0, -1, rho], [0, +1, rho],
  [1, rho, 0], [-1, rho, 0], [1, -rho, 0], [-1, -rho, 0],
  [-rho, 0, 1], [-rho, 0, -1], [rho, 0, 1], [rho, 0, -1]
];
let faceArray = [
  [4, 1, 11],
  [11, 1, 0],
  [6, 11, 0],
  [0, 1, 9],
  [11, 10, 4],
  [9, 1, 5],
  [8, 9, 5],
  [5, 3, 8],
  [6, 10, 11],
  [2, 3, 10],
  [2, 10, 6],
  [8, 3, 2],
  [3, 4, 10],
  [7, 8, 2],
  [9, 8, 7],
  [0, 9, 7],
  [4, 3, 5],
  [5, 1, 4],
  [0, 7, 6],
  [7, 2, 6]
];
 
let iterations = 3;   // 0 is a 20 sided icosahedron,  1 is 80 sided, 2 is 320 sided, 3 is 1280 sided, etc
 
/* midpoint between two vertices */
let midPoint = (p1, p2) => [(p2[0] + p1[0]) / 2, (p2[1] + p1[1]) / 2, (p2[2] + p1[2]) / 2];
 
/* calculate the unit vector */
let v3Unit = (v) => {
  let length = Math.sqrt(Math.pow(v[0], 2) + Math.pow(v[1], 2) + Math.pow(v[2], 2));
  return [v[0] / length, v[1] / length, v[2] / length];
};
 
let newFaceArray = [];
 
for (let j = 0; j < iterations; j++) {
  newFaceArray = [];
  for (let i = 0; i < faceArray.length; i++) {
    let f = faceArray[i];
 
    // add three new points at the midpoint of each vertex
    let m0 = midPoint(vertexList[f[1]], vertexList[f[2]]);
    let m1 = midPoint(vertexList[f[0]], vertexList[f[2]]);
    let m2 = midPoint(vertexList[f[0]], vertexList[f[1]]);

    let radius = 2;  // our icos ran from +1 to -1

    let p0 = vertexList.push(v3Unit(m0).map((n) => n * radius)) - 1;  //new vertex point on surface of sphere through centroid and origin
    let p1 = vertexList.push(v3Unit(m1).map((n) => n * radius)) - 1;
    let p2 = vertexList.push(v3Unit(m2).map((n) => n * radius)) - 1;

    // now four faces - the three corner-to-midpoints and then all three midpoints
    newFaceArray.push([f[0], p2, p1]);
    newFaceArray.push([f[1], p0, p2]);
    newFaceArray.push([f[2], p1, p0]);
    newFaceArray.push([p0, p1, p2]);
  }
  faceArray = newFaceArray;   // in case we go around again
}
 
var ico = view.create('polyhedron3d', [vertexList, faceArray], {
  fillColorArray: [],
  fillOpacity: 1,
  strokeWidth: 0.1,
  layer: 12,
  shader: {
    enabled: true,
    type: 'angle',
    hue: 0,
    saturation: 90,
    minlightness: 60,
    maxLightness: 80
  }
});
```
@JSX.Eval

### `@JSX.Load`, Quizzes & State
<!--
persistent: true
-->

    --{{0}}--
If there is too much code and you do not want to polute the main document, you can use the `@JSX.Load` macro to load external code. To simplify the process, there is a link-like syntax for referencing external resources. In another markdown interpreter or on github, this will result in a clickable link, but in LiaScript it will take care of the resource and perform required url transformations on relative urls if required.

__Find the correct mirror position:__

@[JSX.Load](assets/src/mirror.js)

<!-- data-solution-button="false" -->
[[!]]
<script>
if (!!window.mirror) {
  window.mirror[0] > 4.5 &&
  window.mirror[1] == 0 &&
  window.mirror[2] > 1.5 &&
  window.mirror[2] < 1.7
} else {
  false
}
</script>

    --{{1}}--
Quizzes are a great way to assess learning progress. In LiaScript there are different types of quizzes available, such as multiple choice, single choice, text input, or drag & drop. In this case `[[!]]` defines a general quiz, which requires a script to be evaluated in order to mark a quiz as solved. [`mirror.js`](assets/src/mirror.js) defines a global variable `window.mirror`, which is an array of three numbers. This array is checked by the script below the quiz marker.

    --{{2}}--
Finally, the `persistent: true` directive at the top of the document will not preserve the DOM and its state when changing to another slide. Destroying the state comes handy, if you are using Videos, complex scripts, or other resources. In this case it will not destroy the state of the JSXGraph board, so when the user comes back to this slide, the board will be in the same state as before.


## More Integration?

    --{{0}}--
As mentioned earlier, LiaScript has something like an internal publish subscribe mechanism. The result or `output` of a script can be used as an input for another script. Thus, when the output changes all subsequent script will be reevaluted.

Color: <script input="color" default="red" value="red" output="color">"@input"</script>

Formula: <script input="formula" default="2*x*sin(1/x) - cos(1/x)" value="2*x*sin(1/x) - cos(1/x)" output="formula">"@input"</script>

<script style="display: block; width: 100%">
`HTML: <jsx-graph>
board = JXG.JSXGraph.initBoard(BOARDID, {axis:true, boundingbox:[-1/2, 1/2, 1/2, -1/2]});

var g = board.create('functiongraph', ["@input(`formula`)"], {strokeColor: '@input(`color`)'});
var f = board.create('functiongraph', ["x^2*sin(1/x)"], {strokeWidth:2});
</jsx-graph>`
</script>


### Custom Macros II
<!--
@jsx_formula
``` js @JSX.Script
board = JXG.JSXGraph.initBoard(BOARDID, {axis:true, boundingbox:[-10, 2, 10, -2]});
var g = board.create('functiongraph', ["@1"], {strokeColor: '@0'});
```
@end
-->

    --{{0}}--
Finally, based on that what you have learned so far, you can even define your own extension that allow to automate subsequent tasks. In this example a simple block-comment is used, that takes as parameters two values, a color and a formula. The place where to pass the parameters is marked by `@0`, `@1`, etc. The content of the macro is then injected into the document at the position where the macro is used. And then the new macro will be evaluated with the given parameters and generate the desired JSXGraph board.

    {{1}}
@jsx_formula(red,`2*x*sin(1/x) - cos(1/x)`)

    {{2}}
@jsx_formula(blue,`x*x`)


    {{3}}
@jsx_formula(green,`sin(x) * cos(x)`)


## Thank You! 🙏

