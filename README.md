# Reflective AI Agent 

## 📌 Overview

This project is a **decision-tree-based conversational reflection agent** designed using **Design Thinking principles**.

It guides users through a structured end-of-day reflection and analyzes responses across **3 behavioral axes**:

-   Axis 1 → Internal / Collaborative / External (Locus of control)
    
-   Axis 2 → Contribution / Entitlement
    
-   Axis 3 → Self-centralism / Altrocentralism
    

Based on responses, the system generates a **personalized reflective summary**.

----------

## 🧠 Core Idea

Instead of free-form AI, this system uses a **controlled decision tree model** to:

-   Maintain psychological consistency
    
-   Ensure meaningful reflection
    
-   Provide predictable and interpretable outcomes
    

----------

## 🧩 Project Structure

```
/tree/
  reflection-tree.json (or .yaml, .csv, .tsv)    ← the tree data
  tree-diagram.png (or .svg, .md with Mermaid)    ←  visual diagram
/agent/
agent.html                                            ←runnable code
  ...
/transcripts/                                      sample runs  
  persona-1-transcript.md
  persona-2-transcript.md
  persona-3-transcript.md
write-up.md                                        ←design rationale
README.md                                          ← How to read the tree / run the agent

```
----------

## 📂 File Explanation

### 1. `reflection-tree.json`

Main brain of the system  

Contains:

-   Nodes (start, question, decision, reflection, bridge, summary, end)
    
-   Options (user choices)
    
-   Signals (axis scoring logic)
    
-   Transitions (flow control)
    

👉 Structure of each node:

```
id, parentId, type, text, options, target, signal

```

----------

### 2. `agent.html`

Handles:

-   Reading JSON
    
-   Navigating tree
    
-   Taking user input
    
-   Scoring axes
    
-   Generating final summary
    

Acts like a **finite state machine**

----------

----------

## ⚙️ How the System Works

### Step-by-step flow:

1.  Start → User greeted
    
2.  User selects how the day felt
    
3.  Follow-up questions based on response
    
4.  Decisions assign **axis scores**
    
5.  Reflection messages shown
    
6.  Flow continues across 3 axes
    
7.  Final calculation:
    
    -   Dominant value in each axis
        
8.  Matching summary is displayed
    

----------

## 📊 Axes Explained

### 🌐 Option 2: Web UI (Recommended)

Just open:

```bash
reflection_chatbot_v3.html

```

in your browser.

No setup required.

----------

## 🔁 Example Flow

```
START
↓
“How did your day feel?”
↓
User selects: Tough
↓
Follow-up question
↓
Axis scoring happens
↓
Reflection message
↓
Next axis
↓
Final summary
↓
END

```

----------

## 🔗 Decision Tree Design

Full visual representation available here:

👉 [https://miro.com/app/board/uXjVHeyAjtg=/?share_link_id=553469720609](https://miro.com/app/board/uXjVHeyAjtg=/?share_link_id=553469720609)

This board shows:

-   All branches
    
-   Axis mappings
    
-   Reflection logic
    
-   Summary combinations
    

----------

## 🎯 Key Features

-   Structured conversational AI
    
-   Multi-axis behavioral analysis
    
-   Emotion-aware questioning
    
-   Deterministic and explainable outputs
    
-   Dual implementation (CLI + Web UI)
    

----------
