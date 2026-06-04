---
layout: default
---

# Week 07

[← Back to Home](../index.md)

# DES240 7: Data-Driven Visualisation Development

# Class Activities

* Concept Sketch Development
* Peer Feedback Exchange
* Making Sprint
* What If Variations
* Progress Report Preparation

---

# Project Development

## Revisiting the Design Question

### Design Question

**How might we visualise the ways digital systems interpret and construct personal identity through behavioural data?**

Following the development of the initial project framework in Week 6, this week focused on transforming the conceptual structure of **ECHO//PROFILE** into an early functional prototype.

Rather than concentrating on final visual aesthetics, the goal was to test whether behavioural information could successfully function as a data source and whether those behaviours could be transformed into meaningful interpretations.

This marked the project's transition from planning into active experimentation.

---

# Concept Sketch Development

## Original Concept

The original concept focused on a linear transformation process:

```text
┌─────────────┐
│ Behaviour   │
└──────┬──────┘
       ↓
┌─────────────┐
│ Data        │
│ Collection  │
└──────┬──────┘
       ↓
┌─────────────┐
│ Interpretation │
└──────┬──────┘
       ↓
┌─────────────┐
│ Atmosphere  │
└──────┬──────┘
       ↓
┌─────────────┐
│ Identity    │
│ Profile     │
└──────┬──────┘
       ↓
┌─────────────┐
│ Reflection  │
└─────────────┘
```

The concept emphasised the invisible relationship between user behaviour and algorithmic interpretation.

---

## Peer Feedback

### Observation 01

> "The profile feels interesting, but I want to understand how the system reaches its conclusions."

### Observation 02

> "The atmosphere seems disconnected from the generated profile."

### Observation 03

> "It would be interesting if users could disagree with the profile."

### Question 01

> "What behaviours influence the profile most strongly?"

### Question 02

> "How accurate is the profile intended to be?"

### Question 03

> "What happens if the system gets it wrong?"

---

## Reflection on Feedback

The feedback revealed that the interpretation process itself was more interesting than the final profile.

Initially, I had focused on the generated identity output. However, peer responses suggested that users may be more curious about how behavioural data is translated into assumptions.

This prompted a shift towards making the interpretation process visible.

Rather than hiding the algorithmic logic, future iterations will expose the relationship between behavioural actions and generated conclusions.

---

## Revised Concept Sketch

```text
┌─────────────┐
│ Behaviour   │
└──────┬──────┘
       ↓
┌─────────────┐
│ Data        │
│ Collection  │
└──────┬──────┘
       ↓
┌─────────────┐
│ Interpretation │
│ Rules       │
└──────┬──────┘
       ↓
┌─────────────┐
│ Profile     │
│ Construction│
└──────┬──────┘
       ↓
┌─────────────┐
│ User        │
│ Reflection  │
└──────┬──────┘
       ↓
┌─────────────┐
│ Profile     │
│ Accepted?   │
└─────────────┘
```

### Concept Development Diagram

```text
User Behaviour
      │
      ▼
Behaviour Tracking
      │
      ▼
Interpretation Rules
      │
      ▼
Generated Profile
      │
      ▼
User Response
      │
 ┌────┴────┐
 ▼         ▼
Agree   Disagree
```

---

# Making Sprint

## Experiment 01 — Behaviour Tracking Prototype

### Aim

To test whether user behaviour can be successfully recorded and transformed into a dynamic dataset.

### Prototype Overview

A simple p5.js environment was created where users control a circle using WASD movement.

The prototype continuously records behavioural information and displays collected data through a live debugging interface.

### Behaviours Recorded

| Behaviour      | Data Collected     |
| -------------- | ------------------ |
| Movement       | Distance Travelled |
| Clicking       | Click Count        |
| Inactivity     | Idle Time          |
| Session Length | Session Duration   |
| Activity       | Movement Time      |

---

### Prototype Structure

```text
User Input
   │
   ├── WASD Movement
   ├── Mouse Click
   └── Idle State
          │
          ▼
Behaviour Tracking System
          │
          ▼
Live Dataset
          │
          ▼
Debug Panel Display
```

---

## Experiment Findings

The prototype successfully demonstrated that user behaviour can be converted into measurable information.

However, the experiment also highlighted a limitation:

**Behavioural data alone does not contain meaning.**

For example:

```text
Idle Time
   │
   ▼
Possible Interpretations
   ├─ Calm
   ├─ Confused
   ├─ Distracted
   └─ Thinking
```

The system must decide how behaviour is interpreted.

This insight became a significant conceptual discovery and reinforced the project's focus on algorithmic assumptions rather than objective truth.

---

# Technical Skill Building

## Skill Development 01 — Behaviour Tracking

### Skills Practised

* Keyboard input
* Mouse input
* Variable management
* Data collection
* Time tracking

### Learning Outcomes

I learned how behavioural actions can be translated into quantitative information and stored as a dataset.

This experiment provided the technical foundation for future interpretation systems.

---

## Skill Development 02 — Data Interpretation Logic

### Exploration

I began experimenting with simple rule-based interpretation systems.

### Interpretation Rules

| Behaviour Metric           | Interpretation  |
| -------------------------- | --------------- |
| High Movement              | Explorer        |
| High Idle Time             | Observer        |
| High Click Count           | Engaged User    |
| Long Session Duration      | Persistent User |
| Frequent Direction Changes | Curious User    |

---

### Interpretation Mapping Diagram

```text
Distance Travelled
        │
        ▼
   Explorer Score

Idle Time
        │
        ▼
   Observer Score

Click Count
        │
        ▼
 Engagement Score

Session Duration
        │
        ▼
 Persistence Score
```

---

## Skill Development 03 — Live Profile Generation

### Early Profile Logic

The prototype began testing how behavioural information could generate a profile.

### Example Output

| Profile Trait | Score |
| ------------- | ----- |
| Explorer      | 74%   |
| Observer      | 48%   |
| Engaged       | 63%   |

### Profile Mockup

```text
=================================
        ECHO//PROFILE
=================================

Explorer      ███████░░░ 74%
Observer      █████░░░░░ 48%
Engaged       ██████░░░░ 63%

Primary Identity:
EXPLORER

Confidence Level:
74%

=================================
```

---

# What If Variations

## Variation 01

### What if the profile changed in real time?

Instead of generating a profile at the end of the experience, users would watch their identity continuously update as they interact.

### Potential Benefits

* Makes profiling more visible.
* Creates awareness of continuous surveillance.

### System Flow

```text
Behaviour
    │
    ▼
Live Tracking
    │
    ▼
Real-Time Analysis
    │
    ▼
Live Profile Update
```

---

## Variation 02

### What if users could challenge the generated profile?

After receiving a profile, users could agree or disagree with the system's interpretation.

### Potential Benefits

* Encourages reflection.
* Highlights limitations of algorithmic assumptions.
* Creates a dialogue between user identity and machine interpretation.

### System Flow

```text
Generated Profile
        │
        ▼
 User Decision
   ┌────┴────┐
   ▼         ▼
Agree    Disagree
   │         │
   └────┬────┘
        ▼
Reflection Layer
```

---

## Variation 03

### What if atmosphere became the profile?

Rather than displaying profile text, behavioural information could directly transform the environment.

### Example

```text
Explorer
    │
    ▼
More Particles
    │
    ▼
Larger Environment
    │
    ▼
Different Atmosphere
```

### Potential Benefits

* More immersive experience.
* Stronger connection between behaviour and visualisation.

---

## Selected Variation

### Variation 02 — Challenging the Profile

This variation was selected because it introduces reflection and critical thinking.

The project is ultimately concerned with how systems construct identities from incomplete information.

Allowing users to respond to generated profiles may strengthen the project's engagement with Data Humanism and algorithmic interpretation.

### What If Sketch

```text
=================================
      GENERATED PROFILE
=================================

Explorer : 74%
Observer : 48%
Engaged  : 63%

Do you agree with this profile?

[ YES ]      [ NO ]

          ▼

Why?

_________________________

_________________________

Submit Reflection
=================================
```

---

# Documentation

## Behaviour → Interpretation System

### Current System

| Behaviour Data     | Interpretation Output |
| ------------------ | --------------------- |
| Distance Travelled | Explorer Score        |
| Idle Time          | Observer Score        |
| Click Count        | Engagement Score      |
| Session Duration   | Persistence Score     |
| Direction Changes  | Curiosity Score       |

### System Diagram

```text
┌─────────────────┐
│ Behaviour Data  │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ Interpretation  │
│ Rules Engine    │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ Profile Scores  │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ Identity Output │
└─────────────────┘
```

---

## Current Prototype Structure

```text
┌─────────────┐
│ User Input  │
└──────┬──────┘
       ▼
┌─────────────┐
│ Behaviour   │
│ Tracking    │
└──────┬──────┘
       ▼
┌─────────────┐
│ Behaviour   │
│ Dataset     │
└──────┬──────┘
       ▼
┌─────────────┐
│ Interpretation │
│ Logic       │
└──────┬──────┘
       ▼
┌─────────────┐
│ Identity    │
│ Profile     │
└──────┬──────┘
       ▼
┌─────────────┐
│ Reflection  │
└─────────────┘
```

### Prototype Architecture Diagram

```text
User
 │
 ▼
Input Layer
 │
 ▼
Tracking Layer
 │
 ▼
Data Storage Layer
 │
 ▼
Interpretation Layer
 │
 ▼
Visualisation Layer
 │
 ▼
Reflection Layer
```

---

# Progress Report Preparation

## Current Project Status

### Completed

| Task                         | Status |
| ---------------------------- | ------ |
| Project Concept              | ✅      |
| Data Source Definition       | ✅      |
| Visual Research              | ✅      |
| Behaviour Tracking Prototype | ✅      |
| Initial Interpretation Logic | ✅      |

### In Progress

| Task                      | Status |
| ------------------------- | ------ |
| Profile Generation System | 🔄     |
| Visualisation Design      | 🔄     |
| Reflection Layer          | 🔄     |

### Next Steps

| Priority | Task                                 |
| -------- | ------------------------------------ |
| High     | Build atmosphere generation system   |
| High     | Visualise behavioural interpretation |
| Medium   | Test user reflection interactions    |

---

## Questions for Feedback

### Question 01

How visible should the interpretation process be?

### Question 02

Should the profile be accurate or intentionally flawed?

### Question 03

How can the visualisation communicate uncertainty within behavioural data?

---

# Independent Study

## Continued Prototype Development

Following the Making Sprint, I continued refining the behaviour tracking prototype and began exploring how behavioural information could be transformed into generated profiles.

The primary challenge was determining how behaviour should be interpreted. While collecting behavioural information proved technically straightforward, assigning meaning to that information required subjective decisions.

This reinforced one of the central themes of the project: behavioural data does not inherently contain truth. Instead, systems actively construct interpretations through predefined rules and assumptions.

Future development will focus on exposing this process and encouraging users to reflect on the limitations of algorithmic profiling.

---

# Reflection

This week marked the transition from conceptual planning to active experimentation. The Making Sprint allowed me to test whether behaviour could function as a meaningful data source, while peer critique helped reveal new opportunities within the project.

One of the most significant discoveries was recognising the difference between data collection and data interpretation. Although behaviour can be measured objectively, meaning is always constructed through interpretation. This insight shifted my focus away from profile generation alone and towards revealing how algorithmic systems construct assumptions about users.

The What If Variations exercise further expanded the project by introducing possibilities for user reflection and participation. In particular, the idea of allowing users to challenge generated profiles aligned strongly with the project's interest in identity, perception, and Data Humanism.

Technically, I developed foundational skills in behaviour tracking and data management, while conceptually, I began questioning the assumptions embedded within data-driven systems. These developments significantly strengthened the project and established a clear direction for future prototyping.

---

## AI Usage Statement

ChatGPT was used to assist with brainstorming, project planning, documentation structure, reflection writing, and concept development. All experimentation, coding implementation, design decisions, interpretation, and project outcomes were reviewed, modified, and developed by the author.

## Documentation 

# Class activities
- concept sketches
- making
- 'What if' Variations


behaviour tracking of user mouse

<iframe src="https://editor.p5js.org/harrisonwu23/full/6W65RTo9D"></iframe>

it tracks the dot at middle, 



Behavioral emtion interpreter (collecting user's data from click, stay, movement and system read as user's emotions)

<iframe src="https://editor.p5js.org/harrisonwu23/full/vQUoyLjEQ"></iframe>

# Independent Study
- Project development & skill Building
- Progress report (or summary of this)


# Reflection

## AI Usage Statement