---
title: "Starcatcher: Tech Art Breakdown"
summary:  'I worked as a Graphics Programmer / Tech Artist and got to do some cool things. This page is WIP'
weight: 2

date: 2026-09-01

draft: false
type: "Games"
catergories: ['Games']
tags: ['WIP', 'Unity', 'C#', 'HLSL', 'Shader Graph']
featured: true
---

<!-- TODO update hero.html or make a shortcode for project information at the top -->

If you're reading this, this page is WIP. Congrats you get to see it being half done. You can message / email me via LinkedIn if you want more details this page is finished.

{{< video
  src="Clip_Turnaround_Small.mp4"
  poster="feature.png"
  caption="**Starcatcher** - Main scene turnaround"
  autoplay=true
  controls=false
  loop=true
  muted=true
>}}

<!-- About  -->

<br>
<div style="display:flex;flex-wrap:wrap;gap:10px;margin-top:0">
    <div style="float: left; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

# About the Game

Launch into space, grab stars falling out of the sky, and throw them back into the stratosphere!

Our submission to this summer's MelonJam 2026 is STARCATCHER, an action movement game. Use an expressive movement system to go up to the stars, then watch the sparks fly as you bring back order to the earth.

We ended up ranked #4 in Graphics, #5 in Polish, and #7 in Innovation!

  </div>
  <div style="float: right; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

<iframe frameborder="0" src="https://itch.io/embed/4792848?bg_color=222222&amp;fg_color=eeeeee&amp;link_color=fadb5b&amp;border_color=363636" width="552" height="167"><a href="https://masoncrochetiere.itch.io/star-catcher">STARCATCHER by Mason Crochetiere, Brandon Bell, Jupiter SC, trashedtomato</a></iframe>
  </div>
</div>
<br>

<!-- Role / Problem Statement -->

<br>

# My Role

* As a Graphics Programmer / Technical Artist, I used my unique background in Programming and Art to program shaders and tools to further the visuals of our game

* I did this by collaborating with the team specifically with artist Brandon (linked in Itch page) to define an art direction

* Then I went ahead and made the shaders and systems required. Starting the Water shader, to refamiliarize myself with Unity since I have programmed Gerstner Waves before. Then the Star/Sun Shader since it was the centerpiece. Next the sky system, as it was integrated with game mechanics. Lastly Terrain.

<br>

<!-- Star Shader -->

<br>
<div style="display:flex;flex-wrap:wrap;gap:10px;margin-top:0">
    <div style="float: left; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

# Star Shader

* [TODO] Explain Shader Graph with screenshots

  </div>
  <div style="float: right; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

{{< video
  src="Clip_Sun_Shader.mp4"
  caption="**Starcatcher** - Stars Shader"
  autoplay=true
  controls=false
  loop=true
  muted=true
  ratio=1/1
>}}

  </div>
</div>
<br>

<!-- Sky -->

<br>
<div style="display:flex;flex-wrap:wrap;gap:10px;margin-top:0">
    <div style="float: left; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

{{< video
  src="Clip_Sky.mp4"
  caption="**Starcatcher** - Sky System playing"
  autoplay=true
  controls=false
  loop=true
  muted=true
  ratio=1/1
>}}

  </div>
  <div style="float: right; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

# Sky System

* Extending Unity’s built in skybox shader by setting those values
* Includes setting values that aren’t the skybox too, like fog colour and fading in the stars
* Helpful editor buttons to save current values as variables and slider for testing
* There’s also a skysphere with a gradient of the fog colour to make the horizon fade in better.

[TODO in editor tool screenshot]

  </div>
</div>
<br>

<!-- Water -->


<br>
<div style="display:flex;flex-wrap:wrap;gap:10px;margin-top:0">
    <div style="float: left; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

# Water Shader

* Gerstner waves stylized by blending to white based on height
* HLSL

[TODO quick explanation. I've done Gerstner waves before though]

  </div>
  <div style="float: right; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

{{< video
  src="Clip_Waves.mp4"
  caption="**Starcatcher** - Gerstner Wave Shader"
  autoplay=true
  controls=false
  loop=true
  muted=true
  ratio=1/1
>}}

  </div>
</div>
<br>

<!-- Terrain -->

<br>
<div style="display:flex;flex-wrap:wrap;gap:10px;margin-top:0">
    <div style="float: left; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

{{< video
  src="Clip_Terrain.mp4"
  caption="**Starcatcher** - Terrain Shader on final terrain, and a material sphere... Not Particularly intersting"
  autoplay=true
  controls=false
  loop=true
  muted=true
  ratio=1/1
>}}

  </div>
  <div style="float: right; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

# Terrain Shader

* Based on surface normals
* Shader Graph

[TODO Again screenshot of SHader Graph with explanations. This is very simple lol]

  </div>
</div>
<br>


<!-- Result -->

# Final Result

{{< video
  src="Clip_Turnaround_Small.mp4"
  poster="feature.png"
  caption="**Starcatcher** - Main scene turnaround (again)"
  autoplay=true
  controls=false
  loop=true
  muted=true
>}}

<br>

<!-- Learning -->

# What I Learned

* The power of a shared vision! By ensuring we all communicated frequently and with enough detail, we enabled quite smooth asynchonous communicataion. Meaning even when working at different times, each team member already knew exactly what to work on 

* Similarly, setting art goals with references and mood boards really reduces analysis paralysis. Having a goal makes it so much easier to determine Definitios of Done. By discussing artsyle with the team, deciding on something starry with plenty of gradients, Brandon was able to put together a mood board which worked as a blueprint for my shaders and colours!