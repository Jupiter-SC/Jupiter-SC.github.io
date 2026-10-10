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

**If you're reading this, this page is WIP. Congrats you get to see it being half done. You can message me via LinkedIn or Email if you want more details before this page is finished.** All of those pictures will be turned into short captioned videos :). I have many to-dos in my comments... Getting footage is boring and tedious... I'm making a plugin to make it a bit less of a pain..

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
* I needed to create a visually disctinct shader style based on the artists and I's shared vision. And work on tooling to speed up work for Artist and Designer

# My Contributions
* Creating the main surface shader, with a slight hand-drawn and grainy asethetic

* A recolouring shader to speed up Artist workflow and allow for easy variations

* A procedural room layout system with editor featuring a recursive style to speed up Designer workflows


  </div>

</div>
<br>


<br>

<!-- Surface Shader -->

<br>
<div style="display:flex;flex-wrap:wrap;gap:10px;margin-top:0">
    <div style="float: left; width: 100%; max-width: 400px; min-width: 200px; margin-left: 20px">

# Surface Shader

* The goal was to make something inspired by hand drawn art with a grainy atmosphere

* It consists of a toon surface shader with hatching and noise offsets, and inverse hull outlines

  </div>
  <div style="float: right; width: 100%; max-width: 800px; min-width: 200px; margin-left: 20px">

{{< video
  src="Clip_Showcase.mp4"
  caption="**Mimic** - Shader showcase"
  autoplay=true
  controls=false
  loop=true
  muted=true
>}}

  </div>
</div>

<!-- For the surface shader have a turn around, and add on each “layer” / part of the shader one at a time (ex base lighting -> toon lighting -> noise offset), with bottom captions explaining whats added -->

<!-- [TODO Replace tiny images with quick annotated videos with zoomed in sections :)] -->

<br>
<div style="display:flex;flex-wrap:wrap;gap:10px;margin-top:0">
    <div style="float: left; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

* It’s a toon shader with 3 light levels, with a noise value added to make the shading splotchy. Then shadowed parts use different hatching textures.

![Toon ShaderGraph image](Shadergraph-Toon.jpg)

  </div>
  <div style="float: right; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

* For the outlines my goal was to create a boiling lines effect. I used the inverse hull method for outlines, and then added a random offset per vertex to make them wobble. It switches between 3 variations based on time.

![Outline ShaderGraph image](Shadergraph-Outlines.jpg)

  </div>
</div>
<br>

<!-- Recolour Shader -->

<!-- For the recolour  shader,  mention  the  reason for having 5  color options was to have them equally spaced and  fix can't   serialize gradients,  and it's faster than using another texture since it can all be done in engine -->

<!-- TODO Show a pipeline video in editor tool screenshot video, formatted kinda like Minions Art!  -->

<br>
<div style="display:flex;flex-wrap:wrap;gap:10px;margin-top:0">
    <div style="float: left; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

<!-- {{< video
  src="Clip_Sky.mp4"
  caption="**Mimic** - Recolour pipeline demo"
  autoplay=true
  controls=false
  loop=true
  muted=true
  ratio=1/1
>}} -->

![Outline ShaderGraph image](Shadergraph-Recolour.jpg)

  </div>
  <div style="float: right; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

# Recolour Shader

* We needed a lot of variations so we did them procedurally
* Takes in BW text → Set colour in engine → Finished product turn around

  </div>
</div>
<br>

<!-- Randomizing Rooms -->

<!-- For the room be sure to show off prop setup and recursive  nature (ben genning some recursives),  then gen the whole room -->

<br>
<div style="display:flex;flex-wrap:wrap;gap:10px;margin-top:0">
    <div style="float: left; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

# Room Randomization

* Editor tool to create randomized rooms and save them as prefabs to use as the actual game levels. Speeds up Design workflow and add more variety

* Recursive structure means rooms can randomize child props (ex: Table with random chairs). Option to tune more specific parts if needed but can be ignore if not needed.

* Full Features: 
  - Recursive struture
  - Save prefab button with name
  - Bounds for position/rotation randomization on child objects (plus a button to actually apply to children since they have their own values) 
  - RoomID list to integrate with gameplay parts 
  - Prop list to pick randomized items from
  - Randomizing texture colours on props
  - I might be forgetting some...

<!-- [TODO Video with zoom ins and bottom captions to show what editing things do] -->

  </div>
  <div style="float: right; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

<!-- {{< video
  src="Clip_Waves.mp4"
  caption="**Mimic** - Using Room Randomization tool in engine"
  autoplay=true
  controls=false
  loop=true
  muted=true
  ratio=1/1
>}} -->


{{< carousel 
  images="Rooms/*" 
  captions="{TODO Captions}"
>}}

**Mimic** - Using Room Randomization tool in engine 

{{< carousel 
  images="Carousel-2/*" 
  captions="Blah"
  aspectRatio=16
>}}

**Mimic** - Recursive Prop Gen

  </div>
</div>
<br>

<!-- Result -->

# Final Result

{{< video
  src="Clip_Showcase.mp4"
  poster="feature.png"
  caption="**Mimic** - Temp video lol"
  autoplay=true
  controls=false
  loop=true
  muted=true
>}}

<br>

<!-- Learning! -->

# Learning Outcomes

* Fun shader stuff!

* Make sure to tailor tools to the users and products.