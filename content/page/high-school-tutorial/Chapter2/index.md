---
title: "Chapter 02 - First Plan - Robot Movement and Perception"
date: 2023-13-02T10:35:35-06:00
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
Move your robot to find objects! Learn to navigate the robot to a table and use its camera to detect a milk carton. Understand how perception works in robotics.

For Entering Chapter two click here:
<a class="btn btn-success" target="_blank" href="chapter2/"><b>Chapter 2!</b></a>
</div>

<!--more-->

# Welcome to Chapter 2: Robot Movement and Perception

Today you'll teach a robot to move and see. You'll navigate it across your virtual apartment and use its camera to spot objects.

**Goal**: By the end of this session, you will have a robot that moves to a table and detects a milk carton using its camera.

## Prerequisites
- Completed Chapter 1 – basic URDF knowledge
- No computer vision experience needed (we'll guide you through it)

---

# What You'll Do Today

## Section 1: Set Up Your Robot Simulation
- Import PyCRAM and Bullet World
- Load your URDF environment from Chapter 1
- Initialize the robot

## Section 2: Move Your Robot
- Use location designators to specify where to go
- Navigate to a table in your virtual kitchen
- See how the robot plans its path automatically

## Section 3: Detect Objects with Camera
- Capture images from the robot's camera
- Use simple color detection to find a milk carton
- Learn basic image processing techniques

## Section 4: Understand Perception Challenges
- Experiment with occlusion (blocked objects)
- Test different lighting conditions
- See how distance affects detection

**[Open the hands-on notebook →](chapter2.ipynb)**

---

## Key Concepts (Simplified)

**Location Designators**: Tell your robot "go to a spot near the table" instead of giving exact coordinates. PyCRAM figures out the details.

**Object Detection**: Use the robot's camera to find objects by their color or shape. Real robots use more advanced methods, but we'll start simple.

**Perception Challenges**: Objects can be hidden, poorly lit, or too far away. Good perception systems handle these problems.

## Exercises You'll Complete

1. **Move to different locations** in your environment
2. **Detect objects** using the robot's camera
3. **Experiment with perception challenges** like blocked views or dim lighting
4. **Try detecting different colored objects** (red apple, blue cup, etc.)

## What You'll Learn

- How robots navigate without crashing
- Why seeing objects is harder than it seems
- How to break down "find the milk" into code steps

## Challenge

Can your robot find the milk carton when it's in different positions? What happens if you move it inside the fridge?

---

## Further Resources

- [PyCRAM Documentation](https://pycram.readthedocs.io/en/latest/)
- [OpenCV for Image Processing](https://www.opencv.org)

## Related Videos

**How your robot plans movements and perceives:**

### Exercise 1: Move Your Robot
Write code to tell your robot to navigate to a table. You'll learn:
- How to specify target locations
- How the robot plans a path (without hitting things)
- How to execute the movement in simulation

### Exercise 2: See Like Your Robot
Use the robot's camera to detect objects. You'll:
- Capture what the camera sees
- Use image processing to find a milk carton
- Learn about challenges: if objects are hidden or in shadows, detection gets harder

### Exercise 3: Understand Perception Challenges
Real perception is messy. You'll experiment with:
- Occlusion (objects blocked by other things)
- Lighting conditions
- How small or far away the target is

**[Launch the hands-on lab →](https://binder.intel4coro.de/v2/gh/sunava/pycram/dc53ccb77028762ef20161a9cdbd88a8ce53980b?urlpath=lab%2Ftree%2Fdemos%2Fpycram_fallschool_2024%2F02_robot_simulation_perception.ipynb)**

### Exercise 4: Simple Object Recognition (Optional)
Try a beginner-friendly perception tool:

**[RoboKudo Getting Started →](https://binder.intel4coro.de/v2/git/https%3A%2F%2Fgitlab.informatik.uni-bremen.de%2Ffmuehlis%2Frobokudo-lab.git/74f0ed78fbb103a6b4d190bf0e1acae5703c73f4?urlpath=lab%2Ftree%2Frobokudo.jupyterlab-workspace)**

---

## What You'll Learn

- Robots need to plan paths without crashing into things
- Perception (seeing) is harder than it sounds—occlusions and lighting matter
- How to break down a task like "find the milk" into code

## Challenge

Try different locations in your environment. Can your robot find the milk carton when it's in different positions? What happens if you put it inside the fridge?

---

## Further Resources

- [PyCRAM Documentation](https://pycram.readthedocs.io/en/latest/)
- [PyCRAM + RoboKudo Integration](https://pycram.readthedocs.io/en/latest/notebooks/interface_examples/robokudo.html)
- [OpenCV (for image processing)](https://www.opencv.org)
- [Open3D (for 3D perception)](https://www.open3d.org)

## Related Videos

**How your robot plans movements and perceives:**

<figure class="video_container">
  <iframe width="100%" height="360" src="https://www.youtube.com/embed/pv_n9FQRoZQ?si=j3CB2Sj4itd_1qlC" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen="true"></iframe>
</figure>

**Object recognition with RoboKudo:**

<figure class="video_container">
  <iframe width="100%" height="360" src="https://www.youtube-nocookie.com/embed/8jvDl-P2ba0?si=AGOn8iCWjDShdMeJ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen="true"></iframe>
</figure>

---

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