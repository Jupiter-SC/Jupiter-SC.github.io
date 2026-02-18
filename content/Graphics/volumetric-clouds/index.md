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

{{< columns >}}

![Main GIF](feature.png)

<--->

# Overview

- Volumetric rendering is cool!
- Implemented as a post processing effect using ray marching
- Rays march through a 3D noise texture and to light source, calculating light based on that density
- Approximating light scattering with Henyey Greenstein Phase Function


{{< /columns >}}

{{< columns >}}

# About the Process
| |  |
| -----------	| -------------------------	|
| Roles			| Programmer	|
| Team Size		| Solo				|
| Timeline		| April 2025 |
| Technology	| Unity, C#, HLSL |

<--->

![Main GIF](feature.png)

{{< /columns >}}

{{< github repo="Joshua-S-C/Unity-Clouds" showThumbnail=true >}}