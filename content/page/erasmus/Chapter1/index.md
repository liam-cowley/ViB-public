---
title: "Chapter 01 - Creating a Semantic Environment"
date: 2023-13-01T10:35:35-06:00
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
Build a virtual apartment simulation using URDF. Creates a 3D environment with furniture and objects, then learn to ask questions about it using a knowledge base—a skill that enables robots to reason about their world.

For Entering Chapter one click here:
<a class="btn btn-success" target="_blank" href="chapter1/"><b>Chapter 1!</b></a>
</div>

<!--more-->

# Welcome to the First Chapter of Our Hands-On Course!

Today you're building a virtual apartment where robots can work! Watch this video to see what's possible:

<figure class="video_container">
  <video width="100%%" height="300" autoplay loop muted controls>
    <source src="vid/ApartmentDemo.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</figure>

## What You'll Do This Session

1. **Build a URDF environment** - Create a virtual apartment with furniture and objects (fridge, table, etc.)
2. **Visualize it** - See your creation in RVIZ
3. **Ask questions about it** - Use a knowledge base to answer queries like "Where is the milk?" or "What's in the kitchen?"

This teaches robots how to understand their environment and reason about where things are and what they can do.

---

# Part 1: Build Your First URDF Environment

### **Goal**
Create and visualize a working URDF model with a fridge, table, and other kitchen objects.

## What is URDF? (2 min read)

**URDF** = Unified Robot Description Format. It's an XML format that describes physical objects and how they connect.

Think of building with LEGO:
- **Links** = the blocks (a fridge door, a table top, etc.)
- **Joints** = the connectors (hinges, bolts, etc. that let parts move)

URDF also specifies:
- How things **look** (visual appearance)
- How they **collide** (for physics)
- How they **move** (what joints allow what motion)

Two common joint types:
- **Revolute joint** = rotates (like a door hinge) 
- **Prismatic joint** = slides (like a drawer)

## Your Hands-On Exercise

### Task 1: Load and Visualize a Basic URDF
Start with a pre-made URDF file and visualize it in RVIZ. You'll see how the file structure maps to a 3D scene.

### Task 2: Add and Modify Objects
Add a fridge, table, and other furniture to your scene. Modify their positions and properties. For example:
- Place the fridge in the corner
- Put the table in front of it
- Add a chair, cabinet, or other kitchen objects

### What You'll Learn
- How URDF files are structured
- How to position objects in 3D space (using x, y, z coordinates)
- How to define simple shapes (boxes, cylinders)
- How joints control movement

**[Run the interactive hands-on tutorial here →](https://binder.intel4coro.de/v2/gh/IntEL4CoRo/ease_fall_school_2024/33c5e5c?urlpath=lab%2Ftree%2Fday1%2FURDF.ipynb)**

---

# Part 2: Bring Your Environment Intelligence with a Knowledge Base

### **Goal**
Transform your URDF scene into an "intelligent" environment that can answer questions about itself.

## Why Does Your Robot Need This?

Your URDF scene is just geometry. But robots need to *reason* about their world:
- "Where should I look for milk?" (Answer: check the fridge)
- "Can I sit here?" (Answer: yes, there's a chair)
- "What items are in the kitchen?" (Answer: fridge, table, sink...)

This is where knowledge bases come in. They let you tag objects with meaning and ask intelligent queries.

## How It Works (Simple Overview)

1. **You tag your URDF with semantic info**: Mark that the fridge is a "food storage" and the table is for "food prep"
2. **The knowledge base stores these relationships**: Creates a simple map of "what is what" and "what can do what"
3. **You query it**: Ask "Give me all food storage objects" and it returns the fridge

This is a taste of what Chapter 3 digs into much deeper.

## Your Hands-On Exercises

### Exercise 1: Tag Your Objects (Optional)
Learn how to mark URDF objects with semantic labels so a knowledge base can understand them. Try the:

**[Multiverse Knowledge Lab →](https://binder.intel4coro.de/v2/gh/Multiverse-Framework/Multiverse-Docker/c578396?urlpath=lab%2Ftree%2FMultiverse-Tutorials%2Ftutorials%2Fmultiverse_knowledge.ipynb)**

### Exercise 2: Query Your Environment
Ask your knowledge base questions about your scene. Try the:

**[KnowRob Lab →](https://binder.intel4coro.de/v2/gh/sasjonge/semantic-map-lab.git/b146ce1?labpath=notebooks%2Fsemantic_map.ipynb)**

Example queries you might try:
- "What objects contain food?"
- "Where can I place a plate?"
- "Which objects can I grasp?"

---

## Quick Challenge

**Try this:** Add a new object (like a cup or plate) to your URDF environment. Reposition it a few times until it's where you want it. This reinforces how to customize URDF models.

## Further Reading

Want to dive deeper? Check out:
- [ROS URDF Tutorials](https://wiki.ros.org/ROS/Tutorials)
- [URDF format documentation](https://wiki.ros.org/urdf)

---

## Instructor Contact

<div class="main-well-flex-container" style="margin:20px;align-items: center;">
  <div style="flex:30%;">
      <img src="img/sjongebloed_sq.jpg" style="clip-path: circle(35%);">
  </div>
  <div style="flex:70%;">
    <h3>Sascha Jongebloed</h3>
    <a href="mailto:jongebloed@cs.uni-bremen.de">jongebloed@cs.uni-bremen.de</a>
  </div>
</div>
