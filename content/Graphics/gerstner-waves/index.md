---
title: "Gerstner Waves"
date: 2026-02-05
draft: false
summary: "A water shader that simulates physically accurate waves using real math done by real smart people"
catergories: ['Graphics']
weight: 1
type: "Graphics"
featured: true

# Header Info
tags: ['C++', 'OpenGL', 'Callisto Engine']
params:
  projectRole: "Graphics Programmer"
  projectSize: "Solo"
  projectTimeline: "Nov - Dec 2023"

  showLogo: false
  showTitle: true
---

**WIP**

![Image](feature.gif)
     
<br>

<div style="display:flex;flex-wrap:wrap;gap:10px;margin-top:0">
    <div style="float: left; width: 100%; max-width: 800px; min-width: 200px; margin-left: 20px">

# Overview

* Made in my rendering engine Callisto
* Uses math done by real smart people to be physically accurate
* Tons of parameters to mess with
* Heightmap of Lake Champlain / Burlington area in there for fun, using real height data from [Tangrams Heightmapper](https://tangrams.github.io/heightmapper/) (so kool!)
* Read the [Wikipedia](https://en.wikipedia.org/wiki/Trochoidal_wave) page 

</div>
<div style="float: right; width: 100%; max-width: 400px; min-width: 400px; margin-left: 20px">
    
<div>
{{< github repo="Jupiter-SC/GPR-200" >}}
</div>

</div>
</div>

<br>

<div style="display:flex;flex-wrap:wrap;gap:10px;margin-top:0">
    <div style="float: left; width: 100%; max-width: 800px; min-width: 200px; margin-left: 20px">

{{< carousel images="images/*" aspectRatio="16-9" interval="2500" >}}

</div>
<div style="float: right; width: 100%; max-width: 400px; min-width: 200px; margin-left: 20px">

# Changing Params
- Ability to add as many waves as you want
- Can change the parameters per wave
    - Frequency, Amplitude, Steepness, Direction
- Colour! (As always)
- Blinn-Phong uniforms

</div>