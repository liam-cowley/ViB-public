---
title: "Chapter 03 - Querying the Knowledge Base System"
date: 2023-13-03T10:35:35-06:00
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
On Chapter 3, you'll explore the role of a knowledge base in robot decision-making.
You'll learn how to make queries to the knowledge base to determine the actions the robot must take to accomplish its tasks, such as perceiving objects in the environment.

For Entering Chapter three click here:
<a class="btn btn-success" target="_blank" href="chapter3/"><b>Chapter 3!</b></a>
</div>

<!--more-->

# Welcome to Chapter 3: Querying the Knowledge Base System

Today you'll teach your robot to *think* about what it should do. You'll query a knowledge base to answer questions like "How do I get the milk?" and "What actions do I need to take?"

**Goal**: By the end of this session, you will write queries to your knowledge base that enable the robot to plan actions—for example, determining that it must open the fridge to get the milk.

## Prerequisites
- Completed Chapters 1–2
- Basic understanding of "if-then" logic (helpful but not required)

---

# What You'll Do Today

## Section 1: Connect to Your Knowledge Base
- Import KnowRob client
- Load your knowledge base from Chapter 1
- Connect to the KnowRob server

## Section 2: Ask Basic Questions
- Query what objects are in the kitchen
- Find where the milk is located
- List available containers

## Section 3: Plan Actions with Queries
- Ask what steps are needed to perceive the milk
- Check prerequisites for grasping objects
- Find what actions a robot can perform

## Section 4: Add Your Own Knowledge
- Define new facts about your environment
- Create rules for robot behavior
- Test how new knowledge changes query results

---

## Key Concepts

**Knowledge Base**: A smart database that stores facts about your environment and rules for robot behavior.

**Queries**: Questions you ask the knowledge base, like "Where is the milk?" or "What must I do before grasping?"

**Facts & Rules**: Facts are statements like "Milk is in the fridge." Rules are logic like "To grasp something, you must perceive it first."

## Exercises You'll Complete

1. **Query-driven robot movement** - Use queries to find good locations to move to
2. **Conditional actions** - Check if the fridge is open before trying to perceive milk
3. **Create complete plans** - Combine multiple queries to build full action sequences

## What You'll Learn

- How robots use knowledge to make decisions
- How to ask the right questions to plan actions
- How to add new facts and rules to improve robot behavior

## Challenge

Create a complete plan for getting milk from the fridge. What queries do you need? What new facts might help?

---

## Further Resources

- [KnowRob Documentation](https://knowrob.org/)
- [SPARQL Query Language](https://www.w3.org/TR/sparql11-query/)

## Summary

By the end of this session, you'll have a robot that can reason about what actions to take, making it much smarter than following pre-programmed steps. 
object information and information about observed actions that has been acquired from various sources (manually axiomatized, derived from observations, or imported from the web).

## Step-by-Step Hands-On Exercises
1. **Query the Knowledge Base**: Write simple queries to understand the environment
2. **Action Planning**: Ask questions that require reasoning through facts and rules
3. **Define New Knowledge**: Add your own facts and rules, then test queries

Throughout the exercises, code examples will demonstrate how to perform queries using Python.

Interactive Actions and/or Examples
---

For Hands-On Exercises please use the following Virtual Lab: <a class="btn btn-success" target="_blank" href="https://binder.intel4coro.de/v2/gh/liam-cowley/pycram/fallschool?urlpath=lab%2Ftree%2Fdemos%2Fpycram_fallschool_2024%2F03_Knowledge_Base_Queries.ipynb">Knowledge Base Queries</a>


## Summary

By the end of this session, you'll have a robot that can reason about what actions to take, making it much smarter than following pre-programmed steps.

---

## Instructor Contact

<div class="main-well-flex-container" style="margin:20px;align-items: center;">

  <div style="flex:30%;">
      <img src="img/vanessa.jpg" style="clip-path: circle(35%);">
  </div>

  <div style="flex:70%;">
       <h3> Vanessa Hassouna</h3>
    Tel:  +49 421 218 99651 <br>
    Mail:     <a href="mailto:hassouna@cs.uni-bremen.de">hassouna@cs.uni-bremen.de</a> <br>
      <a style="color:red" href="https://ai.uni-bremen.de/team/vanessa_hassouna">
      <span style="font-size: 15px;">Profile Vanessa Hassouna</span>
    </a>
  </div>
</div>

<div class="main-well-flex-container" style="margin:20px;align-items: center;">

  <div style="flex:30%;">
      <img src="img/alina.jpg" style="clip-path: circle(35%);">
  </div>

  <div style="flex:70%;">
    <h3> Alina Hawkin</h3>
    Tel: +49 421 218 64024 <br>
    Mail: <a href="mailto:hawkin@uni-bremen.de">hawkin@uni-bremen.de</a> <br>
    <a style="color:red" href="https://ai.uni-bremen.de/team/alina_hawkin">
        <span style="font-size: 15px;">Profile Alina Hawkin</span>
    </a>
</div>
</div>


<div class="main-well-flex-container" style="margin:20px;align-items: center;">

  <div style="flex:30%;">
      <img src="../mbeetza.jpg" style="clip-path: circle(35%);">
  </div>

  <div style="flex:70%;">
       <h3> Prof. Michael Beetz PhD</h3>
    Tel:  +49 421 218 64001 <br>
    Mail:     <a href="mailto:beetz@cs.uni-bremen.de">beetz@cs.uni-bremen.de</a> <br>
      <a style="color:red" href="https://ai.uni-bremen.de/team/michael_beetz">
      <span style="font-size: 15px;">Profile Michael Beetz</span>
    </a>
  </div>
</div>

