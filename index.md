<div style="display: flex;">
  <figure style="float: left; width: 25%; ">
    <img src="images/zeger-teaching-1.png" alt="Zeger" />
  </figure>
  <div style="float: left; width: 75%; vertical-align: top;">
   <div style="margin-bottom: 5px; margin-left: 10px;">
    🔭 I’m always open to discuss parttime jobs (freelance)!<br/>
   </div>
   <div style="margin-bottom: 5px; margin-left: 10px;">
    📝 My resume can be downloaded <a href="https://www.hendrikse.name/cvWeb.docx.pdf">here</a><br/>
   </div>
   <div style="margin-bottom: 5px; margin-left: 10px;">
    👯 I’m currently working on my ✨<a href="https://www.hendrikse.name/science/">science &amp; mathematics website</a>✨<br/>
   </div>
   <div style="margin-bottom: 5px; margin-left: 10px;">
    🌱 I’m relearning the stuff I did as a student theoretical physics<br/>
   </div>
   <div style="margin-bottom: 5px; margin-left: 10px;">
    🤔 I’m looking for help creating more scientific 3D visualizations<br/>
   </div>
   <div style="margin-bottom: 5px; margin-left: 10px;">
    💬 Ask me about anything!<br/>
   </div>
   <div style="margin-bottom: 5px; margin-left: 10px;">
    📫 How to reach me: zegerh_＠_yahoo_•_co_•_uk<br/>
   </div>
   <div style="margin-bottom: 5px; margin-left: 10px;">
    ⚡ Fun fact: I love playing the piano 🎹
   </div>
  </div>
</div>
<p style="clear: both;"></p>


# My portfolio
<div style="border-top: 2px solid #cccccc"><br/></div>

## Test-driven development
<div style="border-top: 1px solid #999999"><br/></div>

I love teaching people more about [TDD](https://www.hendrikse.name/tdd/).
Strongly recommended: take a look at [my TDD pages](https://www.hendrikse.name/tdd/) 
section that belongs to my TDD repository, which in turn is packed with dozens of 
[coding kata&apos;s](https://www.hendrikse.name/tdd/katas/index.html).

### My [coding dojos](https://www.hendrikse.name/tdd/dojo/index.html)
<div style="border-top: 1px solid #999999"><br/></div>

<div style="display: flex; align-items: flex-end;">
<figure style="float: left; width: 55%; text-align: center">
  <a href="https://www.hendrikse.name/tdd/dojo/index.html">
    <img alt="Online dojo" src="images/DojoInAction.png"/>
  </a>&nbsp;&nbsp;&nbsp;
  <figcaption>A typical setting of an online coding dojo.</figcaption>
</figure>
<figure style="float: right; width: 45%; text-align: center">
  <a href="https://www.hendrikse.name/tdd/dojo/index.html">
    <img src="images/zeger_teaching.jpg" alt="Coding dojo"/>
  </a>
  <figcaption><br/>A typical setting of a coding dojo.</figcaption>
</figure>
</div>
<p style="clear: both;"></p>

## [Interactive simulations & visualizations](https://www.hendrikse.name/science/)
<div style="border-top: 1px solid #999999"><br/></div>

[![JavaScript](https://img.shields.io/badge/JavaScript-007ACC?logo=javascript&logoColor=white)](https://en.wikipedia.org/wiki/JavaScript)&nbsp;&nbsp;
[![Three.js](https://img.shields.io/badge/Three.js-000000?logo=three.js&logoColor=white)](https://threejs.org/)&nbsp;&nbsp;
[![WebGL](https://img.shields.io/badge/WebGL-990000?logo=webgl&logoColor=white)](https://www.khronos.org/webgl/)

I maintain a site containing countless 
[interactive simulations in physics and mathematics](https://www.hendrikse.name/science/).
Some examples are reproduced below.

### [Solar system](https://www.hendrikse.name/science/astrophysics/solar_system.html)
<div style="border-top: 1px solid #ffcc00"><br/></div>

🔧 This [solar_system.html](https://github.com/zhendrikse/science/blob/main/astrophysics/code/solar_system.html) uses JavaScript &amp; [Three.js](https://threejs.org/) <br/>
🧠 [Newton-Raphson method](https://en.wikipedia.org/wiki/Newton%27s_method) for realistic (elliptic) orbits<br/>
👉 Inspired on [solar-system](https://github.com/lukekulik/solar-system) by [Luke Kulik](https://github.com/lukekulik/), [threex.planets](https://github.com/jeromeetienne/threex.planets) by [Jemore Etienne](https://github.com/jeromeetienne/), and
[solarsystem](https://github.com/pint-drinker/solarsystem) by [Dana Wensberg](https://github.com/pint-drinker/)<br/>
🔑 Includes tilt, spin and tidal locking of applicable moons e.g. Earth’s moon<br/>
🚀 Features advanced techniques for rendering earth clouds &amp; subtle corona breathing driven by magnetic turbulence

<div id="planetControls">
  <div class="buttonRow">
    <button data-body="sun">🔅 Sun</button>
    <button data-body="mercury">Mercury</button>
    <button data-body="venus">Venus</button>
    <button data-body="earth">🌍 Earth</button>
    <button data-body="mars">Mars</button>
    <button id="farField1">🔭</button>
  </div>
  <canvas class="applicationCanvas" id="planetsCanvas" style="background: black; aspect-ratio: 19 / 12;"></canvas>
  <div class="buttonRow">
    <button id="farField2">💫</button>
    <button data-body="jupiter">Jupiter</button>
    <button data-body="saturn">🪐 Saturn</button>
    <button data-body="uranus">Uranus</button>
    <button data-body="neptune">🔱 Neptune</button>
    <button id="zoomIn">🔎</button>
  </div>
</div>
<div class="guiContainer" id="solarSystemGui"></div>
<script type="module" src="https://www.hendrikse.name/science/astrophysics/solar_system.js"></script>
<p style="clear: both;"></p>

### [Black hole GPU ray tracing](https://www.hendrikse.name/science/relativity/black_hole_raytracing.html)
<div style="border-top: 1px solid #999999"><br/></div>

⭐ Based on [NASA-BlackHole](https://github.com/cadenmarinozzi/NASA-BlackHole) by [Caden Marinozzi](https://medium.com/@cadenmarinozzi)<br/>
👉 Extended with realistic accretion disk coloring<br/>

<canvas class="applicationCanvas" id="glslBlackHoleCanvas" style="background: black; aspect-ratio: 16/9"></canvas>
<script type='module' src="https://www.hendrikse.name/science/relativity/black_hole_raytracer_glsl.js"></script>
<p style="clear: both;"></p>

### [Falling raindrops](https://www.hendrikse.name/science/nature/raindrop_waves.html)
<div style="border-top: 1px solid #ffcc00"><br/></div>

⭐ Inspired by [this example](https://beltoforion.de/de/unterhaltungsmathematik/2d-wellengleichung.php) from [Recreational Mathematics with Python](https://github.com/beltoforion/recreational_mathematics_with_python)<br/>
🔧 Rewritten in JavaScript and [three.js](https://threejs.org/) by [Zeger Hendrikse](https://github.com/zhendrikse/), see 
  [raindrop_waves.js](https://github.com/zhendrikse/science/blob/main/nature/raindrop_waves.js)<br/>

<canvas class="applicationCanvas" id="raindropsCanvas" style="aspect-ratio: 2 / 1;"></canvas>
<div class="guiContainer" id="raindropsGui"></div>
<script type="module" src="https://www.hendrikse.name/science/nature/raindrop_waves.js"></script>
<p style="clear: both;"></p>

### [3D shapes](https://www.hendrikse.name/science/mathematics/geometric_surfaces.html)
<div style="border-top: 1px solid #ffcc00"><br/></div>

🔧 This [3D shapes renderer](https://github.com/zhendrikse/science/blob/main/mathematics/code/geometric_surfaces.html) is 100% JavaScript using [Three.js](https://threejs.org/).


<script src="https://cdn.jsdelivr.net/npm/mathjs@11.11.0/lib/browser/math.js" type="text/javascript"></script>

<div class="titleDiv" id="surface-title"></div>
<div class="equationDiv" id="surface-equation"></div>
<div class="canvasWrapper" id="surface-canvas-container">
    <canvas class="applicationCanvas" id="surfaceCanvas"></canvas>
</div>
<canvas class="applicationCanvas" id="ringCanvas" style="aspect-ratio: 4 / 1;"></canvas>
<div class="guiContainer" id="gui-container"></div>
<script type="module" src="https://www.hendrikse.name/science/mathematics/parametric_surfaces.js"></script>
<p style="clear: both;"></p>

### [Equipartition of energy](https://www.hendrikse.name/science/thermodynamics/energy_equipartition.html)
<div style="border-top: 1px solid #ffcc00"><br/></div>

🔧 This [energy_equipartition.html](https://github.com/zhendrikse/science/blob/main/thermodynamics/code/energy_equipartition.html) is 100% JavaScript using [Three.js](https://threejs.org/).

<link href="https://unpkg.com/uplot/dist/uPlot.min.css" rel="stylesheet">
<script src="https://unpkg.com/uplot/dist/uPlot.iife.min.js"></script>
<canvas class="applicationCanvas" id="simulationCanvas"></canvas><br/>
<p style="clear: both;"></p>
<div class="buttonRow">
    <button id="pauseButton">&nbsp;Pause&nbsp;</button>
    <button id="bondTypeButton">Bonds as springs</button>
</div>
<p style="clear: both;"></p>
<div id="energyPlot" style="margin:auto;"></div>
<script type="module" src="https://www.hendrikse.name/science/thermodynamics/energy_equipartition.js"></script>

