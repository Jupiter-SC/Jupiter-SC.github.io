---
title: 'Custom Animation System & Character Controller in Unity'
summary: "We built a completely engine agnostic animation backend and hooked it up to Unity specifics."
weight: 4

date: 2026-02-10

draft: false

type: "Graphics"
tags: ['C#', 'Unity', 'Animation Programming']
catergories: ['Graphics']
---

{{< columns >}}

![Logo](Logo.png)

need to actually put videos / gifs

# About the Process
| |  |
| -----------	| -------------------------	|
| Roles			| Programmer	|
| Team Size		| 3 |
| Timeline		| Dec 2025|
| Technology	| Unity, C# |

<--->

# Overview
* Built fully usable animation pipeline and engine agnostic animation system
* Built a Unity Bridge to translate this information to Unity objects / components
* Used the system to make a character controller to move, jump, dance, pick up a box, and look at objects
* Features:
	* Keyframes, Clips, and Controller
	* Loading Skeletons & Animations
	* FK & IK (CCD) & FK/IK Blending
	* Animation blending & blend tree
	* The actual character controller

{{< /columns >}}

{{< columns >}}

# Structure
Full Scope UML Diagram\
(not *all* class details are shown)

![UML FUll](uml-full.png)

<--->

# Flow
- We convert Unity objects and classes into our own --> then interface with them with the backend system.
- And the program specific way we interface them is controlled by the Unity Program, which includes things like Blending.

{{< /columns >}}

{{< columns >}}

# Unity Bridge
- Acts as adapter from Unity's FBX import (files in resources) to our classes / framework
- Skeleton is the tree structure of transforms in the hierarchy
- Animations are translated into our custom class from Unity's Animation Clip class

![UML Bridge](uml-bridge-unity.png)

<--->

# Unity Program
- Player Controller script handles input and physics. It has and controls Unity Program.
- Unity Program is the driver for our actual animation code using the Animation Player. 
- Plus has our program specific information. It builds / holds the Blend Tree, Transitions, and State Machine.
- Animation information is stored in Anim Nodes, then the Animation Player updates those nodes thru the blend tree

![UML Program](uml-program.png)


{{< /columns >}}


{{< columns >}}

# Blend Trees

- Animation player updates the currently used node, then node evaluates the actual pose output, and animation player applies that to skeleton.
- Interface for node types (includes nodes for state machine!) 
- Anim state is for the Animation state machine and holds which animation to play and the transitions. 
- Then the node itself is a statemachine where that outputs a spatial pose.  this is so kool

![UML Blends](uml-blend-tree.png)

<--->

# The End
This project was kind of a lot and was the culmination of our learning throughout the semester from using C in a different framework.
So we got those takeaways and applied it to a different language and engine.

{{< /columns >}}

