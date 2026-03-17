---
title: 'Volumetric Clouds'
date: 2026-02-03
draft: false
summary: "Volumetric clouds implemented as a post processing effect using ray marching."
catergories: ['Graphics']
tags: ['C#','Unity', 'Unity URP', 'HLSL']
weight: 3
type: "Graphics"
---

<div style="display:flex;flex-wrap:wrap;gap:10px;margin-top:0">
    <div style="float: left; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">

![Image](feature.png)

</div>
    <div style="float: right; width: 100%; max-width: 300px; min-width: 200px; margin-left: 20px">

# Info
| |  |
| -----------	| -------------------------	|
| Roles			| Programmer	|
| Team Size		| Solo				|
| Timeline		| April 2025 |
| Technology	| Unity, C#, HLSL |

</div>
</div>

<br>

<div style="display:flex;flex-wrap:wrap;gap:10px;margin-top:0">
    <div style="float: left; width: 100%; max-width: 600px; min-width: 200px; margin-left: 20px">


# Overview

- Volumetric rendering is cool!
- Implemented as a post processing effect using ray marching
- Rays march through a 3D noise texture and to light source, calculating light based on that density
- Approximating light scattering with Henyey Greenstein Phase Function

</div>
<div style="float: right; width: 100%; max-width: 300px; min-width: 200px; margin-left: 20px">
    
<div>
{{< github repo="Joshua-S-C/Unity-Clouds" showThumbnail=true >}}
</div>

</div>
</div>

<br>

<div style="display:flex;flex-wrap:wrap;gap:10px;margin-top:0">
    <div style="float: left; width: 100%; max-width: 500px; min-width: 200px; margin-left: 20px">

{{< carousel images="images/*" aspectRatio="16-9" interval="2500" >}}

</div>
<div style="float: right; width: 100%; max-width: 400px; min-width: 200px; margin-left: 20px">

# Editing Params
- 
- 
- 

</div>
</div>

<div style="float: left; width: 100%; max-width: 500px; margin-right: 20px">


</div>