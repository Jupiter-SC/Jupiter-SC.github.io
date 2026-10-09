---
# Built In
title: "[TODO] Mimic: Tech Art Breakdown"
summary:  'Summary'
weight: 3
date: 2026-09-01

# Organization Stuff
draft: false
type: "Games"
catergories: ['Games']
featured: false

# Header Info
tags: ['Unity', 'C#', 'HLSL', 'Shader Graph']
params:
  projectRole: "Graphics & Tools Programmer"
  projectSize: "5"
  projectTimeline: "1 Week, 2026"
---

<!-- TODO update hero.html or make a shortcode for project information at the top -->

**If you're reading this, this page is WIP. Congrats you get to see it being half done. You can message me via LinkedIn or Email if you want more details before this page is finished.**


{{< video
  src="Clip_Showcase.mp4"
  poster="feature.png"
  caption="**Mimic** - Temp video lol"
  autoplay=true
  controls=false
  loop=true
  muted=true
>}}

<!-- About & Role / Problem Statement -->

<br>
<div style="display:flex;flex-wrap:wrap;gap:10px;margin-top:0">
    <div style="float: left; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

# About the Game

Hunt down the mimic hiding in an old, well-worn motel. The twist? Your only clues as to what the mimic is come from messages made by players who have previously played the game!

Our team's submission to the 2026.2 Brackeys Game Jam is Mimic, an asynchronous puzzle game. The game is as simple as it is written, but the possibilities for trickery and unique experiences are as endless as the number of people playing the game. 

  <div class="iframe-wrapper">
      <iframe id="responsive-iframe" src="https://itch.io/embed/4934283?border_width=0&amp;bg_color=222222&amp;fg_color=eeeeee&amp;link_color=320000&amp;border_color=363636"></iframe>
    </div>
  </div>
  
  <div style="float: right; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">
    
# My Role
* 

* 

* 

  </div>

</div>
<br>


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
  src="Clip_Showcase.mp4"
  caption="**Mimic** - Shader showcase"
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
  caption="**Mimic** - Recolour pipeline demo"
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
* Takes in BW text → Set colour in engine → Finished product turn around

[TODO Show a pipeline video in editor tool screenshot video, formatted kinda like Minions Art!]

  </div>
</div>
<br>

<!-- Randomizing Rooms -->

<br>
<div style="display:flex;flex-wrap:wrap;gap:10px;margin-top:0">
    <div style="float: left; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

# Room Randomization

* Lots of randomization and editor controls. Recursive structure. Option to tune more specific parts (ex: random objects per locator) if needed but can be ignore if not needed. Helpful buttons and stuff

[TODO Video with zoom ins and bottom captions to show what editing things do]

  </div>
  <div style="float: right; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

{{< video
  src="Clip_Waves.mp4"
  caption="**Mimic** - Using Room Randomization tool in engine"
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
  caption="**Mimic** - Not sure what to put here"
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