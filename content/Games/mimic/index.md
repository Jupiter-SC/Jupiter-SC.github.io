---
# Built In
title: "[TODO] Mimic: Tech Art Breakdown"
summary:  'Summary'
weight: 2
date: 2026-09-01

# Organization Stuff
draft: false
type: "Games"
catergories: ['Games']
featured: false

# Header Info
tags: ['WIP', 'Unity', 'C#', 'HLSL', 'Shader Graph']
params:
  projectRole: "Graphics Programmer"
  projectSize: "5"
  projectTimeline: "1 Week, 2026"
---

<!-- TODO update hero.html or make a shortcode for project information at the top -->

If you're reading this, this page is WIP. Congrats you get to see it being half done. You can message / email me via LinkedIn if you want more details this page is finished.

<!-- 
{{< video
  src="Clip_Turnaround_Small.mp4"
  poster="feature.png"
  caption="**Starcatcher** - Main scene turnaround"
  autoplay=true
  controls=false
  loop=true
  muted=true
>}} -->

<!-- About  -->

<br>
<div style="display:flex;flex-wrap:wrap;gap:10px;margin-top:0">
    <div style="float: left; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

# About the Game

Hunt down the mimic hiding in an old, well-worn motel. The twist? Your only clues as to what the mimic is come from messages made by players who have previously played the game!

Our team's submission to the 2026.2 Brackeys Game Jam is Mimic, an asynchronous puzzle game. The game is as simple as it is written, but the possibilities for trickery and unique experiences are as endless as the number of people playing the game. 

  </div>
  
  <div style="float: right; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">
    <div class="iframe-wrapper">
      <iframe id="responsive-iframe" src="https://itch.io/embed/4934283?border_width=0&amp;bg_color=222222&amp;fg_color=eeeeee&amp;link_color=320000&amp;border_color=363636"></iframe>
    </div>
  </div>

</div>
<br>

<!-- Role / Problem Statement -->

<br>

# My Role
* 

* 

* 

<br>

<!-- Surface Shader -->

<br>
<div style="display:flex;flex-wrap:wrap;gap:10px;margin-top:0">
    <div style="float: left; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

# Surface Shader

Toon Hatching Surface Shader & Outlines

* The goal was to make something inspired by hand drawn art with a grainy atmosphere.

* It’s a toon shader with 3 light levels, with a noise value added to make the shading splotchy. Then shadowed parts use different hatching textures.

* For the outlines my goal was to create a boiling lines effect. I used the inverse hull method for outlines, and then added a random offset per vertex to make them wobble. It switches between 3 variations based on time.


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

<!-- Recolour Shader -->

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

# Recolour Shader

* We needed a lot of variations so we did them procedurally
* Takes in BW text → colour

[TODO in editor tool screenshot]

  </div>
</div>
<br>

<!-- Randomizing Rooms -->

<br>
<div style="display:flex;flex-wrap:wrap;gap:10px;margin-top:0">
    <div style="float: left; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

# Room Randomization

* Lots of randomization and editor controls. Recursive structure. Option to tune more specific parts (ex: random objects per locator) if needed but can be ignore if not needed. Helpful buttons and stuff

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

* 

* 