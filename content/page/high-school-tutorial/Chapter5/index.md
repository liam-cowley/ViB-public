---
title: "Chapter 05 - Create your own LLM Assistant"
date: 2023-15-05T10:35:35-06:00
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
Build an AI assistant that knows about robot programming! Learn Retrieval Augmented Generation (RAG) to create a specialized chatbot that helps you program robots using course materials as its knowledge base.

For Entering Chapter five click here:
<a class="btn btn-success" target="_blank" href="chapter5/"><b>Chapter 5!</b></a>
</div>

<!--more-->

# Welcome to the Bonus Chapter!

Today you'll build a specialized AI assistant. Instead of a generic chatbot, yours will be trained on everything you've learned this week.

**Goal**: By the end of this session, you will have created an AI assistant that can answer questions about robot programming, using Retrieval Augmented Generation (RAG).

## Prerequisites
- Any experience with the previous chapters is helpful (but not required independent of each other)

---

# What Is Retrieval Augmented Generation (RAG)?

**Problem**: Generic AI assistants don't know about your specific domain (robot programming).

**Solution**: Teach the AI by giving it documents. RAG works like this:
1. You provide documents (course materials, documentation, tutorials)
2. When someone asks a question, the AI searches those documents
3. The AI uses relevant passages to formulate an answer

This makes the AI specialized without expensive retraining.

---

# Building Your Assistant

We'll use **RAGFlow** (open-source) and **LLaMA3.2** (open-source LLM from Meta).

## Step 1: Set Up RAGFlow

Go to the RAGFlow instance provided and sign up.

### Configure the Model

1. Go to your **Profile** → **Model Providers**
2. Add **Ollama** with these settings:
   - Model type: `chat`
   - Model name: `llama3.2:3b`
   - Base URL: `http://ollama:11434`
3. Go to **System Model Settings** and set the default chat model to `llama3.2:3b`

## Step 2: Create a Knowledge Base

1. Go to **Knowledge Base** → Create a new one (give it a name)
2. Adjust parameters if you want, or leave defaults
3. Save your knowledge base

## Step 3: Upload Documents

1.Go to **File Management**
2. Upload the course materials you downloaded
3. Link the files to your knowledge base
4. Go to **Knowledge Base** → your KB → **Dataset**
5. Click the play button next to files to process them

## Step 4: Create Your Assistant

1. Go to **Chat** → **Create an Assistant**
2. Name it something meaningful
3. Select your knowledge base
4. Create it!

## Step 5: Test It

Start a new chat and ask questions like:
- "What is URDF?"
- "How do I move a robot?"
- "What is a LocationDesignator?"
- "How do I query a knowledge base?"

Your assistant will search the knowledge base and answer using the course materials.

---

## Make It Better

### Try Different Prompts

Some questions work better than others. Experiment with:
- Specific questions: "How do I use PyCRAM to move the robot?"
- General questions: "Tell me about robotics"
- Questions with examples: "How do I perceive objects like in Chapter 2?"

### Adjust Assistant Settings

In your assistant configuration, you can:
- **Change the initial prompt** - tells the assistant how to behave
- **Adjust temperature** - higher = more creative, lower = more precise
- **Select different knowledge bases** - teach it different topics

---

## Create Your Own Domain

You're not limited to robotics! Create an assistant for:
- Your favorite subject from school
- A hobby or interest
- Documentation from any project
- A book or article collection

**[Launch RAGFlow →](https://ragflow.io/)**

---

## What You've Built

A specialized AI that:
- Knows your domain (robot programming)
- Can answer specific questions
- Uses documents as its knowledge source
- Runs completely with open-source tools

This is the same technique used by many professional organizations to create domain-specific AI assistants.

## Instructor Contact

<div class="main-well-flex-container" style="margin:20px;align-items: center;">
  <div style="flex:30%;">
      <img src="img/arthur.jpg" style="clip-path: circle(35%);">
  </div>
  <div style="flex:70%;">
    <h3>Arthur Niedzwiecki</h3>
    <a href="mailto:aniedz@cs.uni-bremen.de">aniedz@cs.uni-bremen.de</a>
  </div>
</div>
