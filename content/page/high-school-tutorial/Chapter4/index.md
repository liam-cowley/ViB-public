---
title: "Chapter 04 - Completing the Full Transportation Task"
date: 2023-14-04T10:35:35-06:00
subtitle: ""
tags: ["Research"]
dropCap: false
displayInMenu: false
displayInList: true
draft: false
resources:
- name: ActionButtons
  src: "buttons.json"
---
<div class="hidde-after-preview">
Complete the full task! Combine everything you've learned to program the robot to deliver milk from the fridge to the table. This is your integration challenge.

For Entering Chapter four click here:
<a class="btn btn-success" target="_blank" href="chapter4/"><b>Chapter 4!</b></a>
</div>

<!--more-->

<div class="main-well-flex-container" style="margin:20px;align-items: center;">
  <div style="flex:30%;">
      <img src="transportation_task.png" width="200" style="clip-path: circle(35%);">
  </div>
</div> 

# Welcome to the Final Day of Our Hands-On Course!

Today you'll integrate everything: the environment (URDF), movement (navigation & grasping), perception (detecting objects), and knowledge (reasoning about actions).

**Goal**: By the end of this session, you will execute a complete milk delivery task: navigate to the fridge, open it, find the milk, grasp it, and place it on the table.

## Prerequisites
- Completed Chapters 1–3
- Understanding of URDF, perception, planning, and knowledge queries

---

# Orchestrating the Full Task

You'll write a high-level plan that orchestrates all components:

1. **Query Knowledge Base**: "What do I need to do to get the milk?"
2. **Plan Movement**: Navigate to the fridge
3. **Perceive**: Use your camera to find the milk
4. **Grasp**: Pick up the milk
5. **Transport**: Move to the table
6. **Place**: Put the milk down

The simulation will execute your plan step-by-step, and you'll see if it works!

## Your Hands-On Exercises

### Exercise 1: Write Your Task Plan
Use PyCRAM to write code defining:
- The goal (transport milk from fridge to table)
- The constraints (don't crash, grasp gently, etc.)
- The sequence of actions

### Exercise 2: Execute and Debug
Run your plan in simulation:
- Does the robot navigate correctly?
- Does it perceive the milk?
- Can it grasp and move it?

Fix any issues and try again.

### Exercise 3: Test Variations
Change the scenario:
- Move the milk to a different location
- Add obstacles
- Change the target location (e.g., counter instead of table)

How robust is your plan?

---

## Running Your Code

**[Launch the Full Simulation Lab →](https://binder.intel4coro.de/v2/gh/sunava/pycram/1a68c62696a07e1c288613cee303364f47041461?urlpath=lab%2Ftree%2Fdemos%2Fpycram_fallschool_2024%2F04_full_robot_simulation.ipynb)**

---

## Simulation Videos

Watch examples of the task completed:

**Box Opening and Object Manipulation:**
<figure class="video_container">
  <video width="100%%" height="300" autoplay loop muted controls>
    <source src="img/268483153-e2509d42-39ad-4fa1-8224-2bcc55ef098f.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</figure>

**Human-Robot Collaboration in VR:**
<figure class="video_container">
  <video width="100%%" height="300" autoplay loop muted controls>
    <source src="img/Pr2DemoX2.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</figure>

---

## What You've Accomplished

By completing this course, you've learned:
- How to model environments with URDF
- How to move and perceive with robots
- How to reason about tasks with knowledge bases
- How to orchestrate complex robotic behaviors

These are the fundamentals of autonomous robot programming!

## Instructor Contact

<div class="main-well-flex-container" style="margin:20px;align-items: center;">
  <div style="flex:30%;">
      <img src="img/vanessa.jpg" style="clip-path: circle(35%);">
  </div>
  <div style="flex:70%;">
    <h3>Vanessa Hassouna</h3>
    <a href="mailto:hassouna@cs.uni-bremen.de">hassouna@cs.uni-bremen.de</a>
  </div>
</div>
