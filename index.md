<div style="display: flex;">
  <figure style="float: left; width: 25%; ">
    <img src="images/zeger-teaching-1.png" alt="Zeger" />
  </figure>
  <div style="float: left; width: 75%; vertical-align: top;">
   <div style="margin-bottom: 5px;">
    &nbsp;🔭 I’m looking for a job (freelance)!<br/>
   </div>
   <div style="margin-bottom: 5px;">
    &nbsp;📝 My resume can be downloaded <a href="https://www.hendrikse.name/cvWeb.docx.pdf">here</a><br/>
   </div>
   <div style="margin-bottom: 5px;">
    &nbsp;👯 I’m currently working on my ✨<a href="https://www.hendrikse.name/science/">science &amp; mathematics website</a>✨<br/>
   </div>
   <div style="margin-bottom: 5px;">
    &nbsp;🌱 I’m currently relearning the stuff I did as a student theoretical physics<br/>
   </div>
   <div style="margin-bottom: 5px;">
    &nbsp;🤔 I’m looking for help creating more scientific 3D visualizations<br/>
   </div>
   <div style="margin-bottom: 5px;">
    &nbsp;💬 Ask me about anything!<br/>
   </div>
   <div style="margin-bottom: 5px;">
    &nbsp;📫 How to reach me: zeger d.o.t. hendrikse at gmail d.o.t. com<br/>
   </div>
   <div style="margin-bottom: 5px;">
    &nbsp;⚡ Fun fact: I love playing the piano 🎹
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

### My [coding dojos](https://www.hendrikse.name/dojo/index.html)
<div style="border-top: 1px solid #999999"><br/></div>

<div style="display: flex; align-items: flex-end;">
<figure style="float: left; width: 55%; text-align: center">
  <a href="https://www.hendrikse.name/tdd/dojo.html">
    <img alt="Online dojo" src="images/DojoInAction.png"/>
  </a>&nbsp;&nbsp;&nbsp;
  <figcaption>A typical setting of an online coding dojo.</figcaption>
</figure>
<figure style="float: right; width: 45%; text-align: center">
  <a href="https://www.hendrikse.name/tdd/dojo.html">
    <img src="images/zeger_teaching.jpg" alt="Coding dojo"/>
  </a>
  <figcaption><br/>A typical setting of a coding dojo.</figcaption>
</figure>
</div>
<p style="clear: both;"></p>

## Interactive 3D simulations & visualizations
<div style="border-top: 1px solid #999999"><br/></div>

I maintain a site containing countless 
[interactive simulations in physics and mathematics](https://www.hendrikse.name/science/).
Some examples are reproduced below.

### 3D visualization of some molecules
<div style="border-top: 1px solid #999999"><br/></div>

- Code developed in collaboration with [MrBlankCoding](https://github.com/MrBlankCoding)
  in [this GitHub repo](https://github.com/MrBlankCoding/Molecule-3d-Visualisation).
- Molecular data taken from [this code](https://glowscript.org/#/user/priisdk/folder/molecules).
- Written in pure Javascript and [three.js](https://threejs.org/).
- Hovering your mouse over each of the atoms displays additional information!

{% include_relative portfolio/molecules.html %}
<p style="clear: both;"></p>

### Spiral galaxy simulation
<div style="border-top: 1px solid #999999"><br/></div>

- Based on the original idea and [article](https://towardsdatascience.com/create-3-d-galactic-art-with-matplotlib-a7534148a319/) by [Lee Vaughan](https://towardsdatascience.com/author/lee_vaughan/).
- This [spiral_galaxy.html](https://github.com/zhendrikse/science/blob/main/astrophysics/code/spiral_galaxy.html) page is a port to Javascript and [Three.js](https://threejs.org/), extended with 
  colouring and fading:
    - **Core / Bulge** (Central Region): yellow-white to reddish color, since the core is
      populated mostly by older stars (Population II), which are cooler and more evolved.
    - **Mid-to-Outer Disk** (Arms): bluish-white color, because the spiral arms host young, hot,
      and massive stars (Population I), which are blue and short-lived. Also, star-forming regions
      and nebulae contribute a diffuse glow.
    - **Outer Halo**: dim red to transparent, as this region contains very old stars and
      globular clusters, often too dim to be noticeable.

{% include_relative portfolio/spiral_galaxy.html %}
<p style="clear: both;"></p>
