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


## Peer Feedback Documentation

During the concept sketch critique session, I presented my project and collected written feedback from classmates. The responses provided useful insights into how others interpreted the project and revealed several areas that required further clarification.

### skech I showed

![early Proposal concept skecth](<../assets/week-05/Proposal concept image.png>)
**Figure 1** early Proposal concept skecth from chat GPT.


### Feedback Evidence

![Feedback Collection from classmate](<../assets/week-07/feedback from classmate.png>)
**Figure 2** Peer feedback collected during the concept sketch development activity.

---

### Theme 01 — Clarifying the Project Outcome

One participant asked:

> "Are you making an interactive desktop wallpaper?"

This question revealed that the intended outcome of the project was not immediately clear.

Although I understood the project as an interactive data-driven visualisation, some viewers interpreted it primarily as a decorative or atmospheric digital artwork.

This highlighted the need to communicate the project's purpose more clearly and emphasise the role of behavioural data collection and interpretation.

---

### Theme 02 — Data Collection and Real-Time Translation

Another participant commented:

> "How will you collect the data?"

> "Will it be translated in real time?"

This feedback directly addressed one of the project's central mechanisms.

The comment reinforced the importance of making the data collection process visible and understandable.

As a result, I decided that future prototypes should clearly show how behavioural information is recorded and transformed into visual outputs and generated interpretations.

This feedback strongly influenced the development of my Week 7 behaviour-tracking prototype.

---

### Theme 03 — Simplification and Readability

Several comments suggested that the concept contained many interconnected ideas.

Examples included:

> "There's a lot going on."

> "Simplifying could be good."

> "I feel there was too much going on for me to fully understand it."

This feedback suggested that the project was conceptually interesting but visually complex.

Rather than introducing additional features, I realised that simplifying the system structure and visual communication would strengthen the project.

Moving forward, I intend to focus on a clearer behavioural flow:

```text
Behaviour
    ↓
Data Collection
    ↓
Interpretation
    ↓
Profile
    ↓
Reflection
---

### Impact on Project Development

The peer feedback helped reveal that the most important improvement was not adding more features but making the existing system easier to understand.

As a result, I revised the project structure to emphasise:

- Behaviour Tracking
- Data Collection
- Interpretation Rules
- Profile Construction
- User Reflection

This refinement strengthened the project's focus on algorithmic interpretation and improved the clarity of the overall experience.


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

![develop 1](<../assets/week-07/develop 1.png>)
**Figure 3** The ECHO//PROFILE behaviour tracking prototype. Users move a circle using WASD while the system continuously records behavioural information and generates profile interpretations in real time.

![develop 1 moving](<../assets/week-07/develop 1 moving.png>)



<iframe src="https://editor.p5js.org/harrisonwu23/full/GRz_3bHpt"></iframe>


<details>
<summary><b>Click to check： Prompt to gemini</b></summary>
Create a complete p5.js prototype for my DES240 Week 7 Data-Driven Visualisation project.

Project title:
ECHO//PROFILE — Week 7 Behaviour Interpretation Prototype

Context:
This project explores how digital systems collect behavioural data and use it to construct interpretations of user identity. The goal is not to create a finished game, but to make a rough, testable prototype for a design process journal.

The prototype should show:
1. Behaviour tracking
2. Live data collection
3. Simple interpretation logic
4. A generated identity/profile panel
5. Enough visual output for screenshots in a project blog

Use only p5.js drawing functions.
No external assets.
The code must run directly in the p5.js Web Editor.

Canvas:
- 1000 x 600
- White or very light background
- Minimal black/grey interface
- Clean academic data-visualisation style

User Interaction:
- Represent the user as a simple circle.
- Move the circle using WASD keys.
- Allow mouse clicks anywhere on the canvas.

Track these behaviours in real time:
- distanceTravelled
- clickCount
- idleTime
- movementTime
- sessionTime
- interactionCount
- directionChanges

Debug / Raw Data Panel:
Create a left-side panel titled:

RAW BEHAVIOURAL DATA

Display:
- Distance Travelled
- Click Count
- Idle Time
- Movement Time
- Session Time
- Direction Changes
- Current State: ACTIVE / IDLE

Visualisation Area:
In the centre area, show:
- The user circle
- A movement trail behind the user
- Small particles generated by movement
- Click ripple effects when the mouse is clicked
- A soft aura around the user when idle

Interpretation Logic:
Create three profile scores based on behaviour:

Explorer Score:
- Increases with distanceTravelled and directionChanges

Observer Score:
- Increases with idleTime

Engaged Score:
- Increases with clickCount and interactionCount

Scores should be displayed as percentages from 0 to 100.

Profile / Interpretation Panel:
Create a right-side panel titled:

SYSTEM INTERPRETATION

Display:
- Explorer: XX%
- Observer: XX%
- Engaged: XX%

Also display generated interpretation statements, for example:
- "You appear curious."
- "You prefer observation."
- "You actively engage with the system."

The statements should change depending on which score is highest.

Reflection Prompt:
After 45 seconds, display a message near the bottom:

"The system has generated an identity profile from your behaviour."

Then display:

"Do these interpretations represent who you are?"

Add two visual buttons:
[ AGREE ] [ DISAGREE ]

The buttons do not need complex functionality, but when clicked they should update a text label:
- If AGREE clicked: "User accepted the system profile."
- If DISAGREE clicked: "User challenged the system profile."

Important Conceptual Note:
The prototype should make it clear that the system is interpreting behaviour, not revealing objective truth.

Add small text somewhere:
"Behavioural data is being recorded and interpreted."

Code Requirements:
- Clean and commented
- Easy to modify
- Use clear variable names
- Use arrays for movement trail, particles, and click ripples
- Do not use external libraries except p5.js
- Make the layout screenshot-friendly for a design blog

Please provide the complete p5.js code only.
</details>


A simple p5.js environment was created where users control a circle using WASD movement.

The prototype continuously records behavioural information and displays collected data through a live debugging interface.

![develop 2](<../assets/week-07/develop 2.png>)
**Figure 4** Real-time behavioural metrics collected by the system, including distance travelled, idle time, click count, movement time, and session duration.



<details>
<summary><b>Click to check： Prompt to gemini</b></summary>

Based on the current p5.js code for “ECHO//PROFILE — Week 7 Behaviour Interpretation Prototype”, improve the existing code without removing any current functionality.



Do not rewrite the concept from scratch. Refine and extend the current prototype so it becomes stronger as a DES240 Week 7 data-driven visualisation experiment.



Keep all existing features:

- WASD player movement

- Behaviour tracking

- Raw data panel

- Movement trail

- Particles

- Click ripples

- Idle aura

- System interpretation panel

- Explorer / Observer / Engaged scores

- Reflection prompt with AGREE / DISAGREE buttons



Improve the prototype in the following ways:



1. Make the data visualisation clearer

- Add simple bar indicators for Explorer, Observer, and Engaged scores.

- Add a small “recent activity timeline” showing recent behaviour states:

  - Movement

  - Idle

  - Click

- The timeline should update during interaction.



2. Improve the interpretation logic

- Make the profile scores feel more balanced.

- Explorer should be based on distance travelled and direction changes.

- Observer should be based on idle time.

- Engaged should be based on click count and interaction count.

- Keep all scores between 0 and 100.

- Avoid all scores becoming 100 too quickly.



3. Add uncertainty to the system

Because the project critiques algorithmic profiling, the system should show that its interpretation is not objective truth.



Add:

- Confidence Level: XX%

- A short note:

  “This profile is an interpretation, not a fact.”

Confidence should increase slowly with session time and amount of behaviour collected.

4. Improve screenshot quality

Make the layout clearer for blog documentation:

- Left panel: RAW BEHAVIOURAL DATA
- Centre: INTERACTION SPACE
- Right panel: SYSTEM INTERPRETATION
- Bottom: REFLECTION PROMPT
- Use clean typography and spacing.

- Keep the style minimal, academic, and monochrome.

5. Add visual connection between data and profile

When a score increases, show a subtle pulse or highlight on that profile bar.

This should make it easier to see that behaviour is changing the generated identity profile.


6. Add a data log

Add a small log panel that records recent system interpretations, for example:
- “Movement detected → Explorer score increased.”
- “Idle behaviour detected → Observer score increased.”
- “Click interaction detected → Engaged score increased.”

Keep only the most recent 5 log entries.


7. Keep the code clean

- Use clear variable names.
- Add comments explaining the main systems.
- Organise the code into functions where possible.
- Do not use external assets.
- Do not use external libraries except p5.js.
- The code must run directly in the p5.js Web Editor.

Important:

The prototype should still feel like a rough Week 7 experiment, not a final polished game.

The main goal is to show:
Behaviour
↓
Data Collection
↓
Interpretation
↓
Profile Generation
↓
Reflection


Please provide the complete improved p5.js code only.

- make it more visualize
- without using any asset
- Make it looks playful and easy to understand</details>


![added more visual element](<../assets/week-07/added more visual element.png>)


<iframe src="https://editor.p5js.org/harrisonwu23/full/nD1d-rJoO"></iframe>


### Behaviours Recorded

| Behaviour      | Data Collected     |
| -------------- | ------------------ |
| Movement       | Distance Travelled |
| Clicking       | Click Count        |
| Inactivity     | Idle Time          |
| Session Length | Session Duration   |
| Activity       | Movement Time      |

---
![alt text](<../assets/week-07/feedback from classmate.png>)

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