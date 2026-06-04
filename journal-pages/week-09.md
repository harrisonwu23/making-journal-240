---
layout: default
---

# Week 09

[← Back to Home](../index.md)

# DES240 9: Project Statement and Project Refinement

# Class Activities

* Project Statement Development
* Making Sprint
* Round Robin Rapid Reactions
* Project Refinement
* Progress Report Preparation

---

# Project Statement

### Working Title

**ECHO//PROFILE**

### Draft Statement

ECHO//PROFILE is an interactive data-driven visualisation that explores how digital systems construct interpretations of identity through behavioural information.

The project investigates a speculative scenario in which behavioural data is continuously collected and analysed, generating profiles, classifications, and assumptions about users without direct input from them.

Rather than presenting data as objective truth, ECHO//PROFILE exposes how interpretation systems transform incomplete behavioural information into seemingly authoritative identities.

Through profile generation, confidence calculations, misclassification events, and user reflection, the project encourages audiences to question the assumptions embedded within algorithmic profiling systems and consider how data influences identity construction.

---

## Project Statement Evaluation

### What is Working Well?

* Clear focus on behavioural interpretation.
* Strong connection to Data Humanism.
* Links directly to prototype development.
* Clearly communicates the project's critical position.

### What is Missing?

Although the current prototype successfully demonstrates behavioural tracking and profile generation, the visualisation still relies heavily on interface panels, text outputs, and numerical feedback.

At the moment, users primarily experience the project through reading generated information rather than experiencing behavioural interpretation through atmosphere or environmental transformation.

This creates a disconnect between the project's conceptual focus on Data Humanism and its current visual form.

Future development should explore how behavioural information can directly influence visual, spatial, or atmospheric elements so that interpretation becomes something users experience rather than simply observe.

### What Requires Further Investigation?

Several areas require further exploration:

- How uncertainty can be visualised through movement, colour, or atmosphere rather than text.
- How profile generation could become more ambiguous and contradictory over time.
- How users might challenge or influence generated interpretations.
- How environmental responses could communicate behavioural assumptions without relying on traditional interface elements.

Investigating these questions will help move the project away from a dashboard-style system and towards a more immersive data-driven visualisation experience.

---

## Commitment Statement

I will focus on exposing the uncertainty and assumptions involved in behavioural profiling rather than attempting to generate accurate representations of identity.

---

# Peer Discussion

## Project Statement Feedback

### What Was Clear?

Several peers commented that the relationship between behaviour and generated identity was easy to understand.

Comments included:

> "The idea of the system making assumptions about the user is interesting."

> "I immediately understood the connection between behaviour and profiling."

---

### What Needed Further Development?

Several participants suggested that the visual outputs could become more dynamic.

Comments included:

> "I want to see the environment react more."

> "The profile is interesting, but I want to see the data become something visual."

This reinforced the need to move beyond interface-based visualisation.

---

## Round Robin Rapid Reactions

### Reactions Received

> "The profile feels believable even when it might be wrong."

> "It makes me question how online systems classify people."

> "The confidence score makes the profile feel more convincing."

> "I would like to see uncertainty represented visually."

---

### Key Insight

The most valuable insight from the discussions was that participants often trusted the generated profile despite understanding that it was based on incomplete behavioural information.

Several people commented that the confidence score made the profile feel authoritative, even when they recognised that the underlying data was limited.

This revealed an interesting tension between perception and reality. The project becomes most compelling when it demonstrates how systems can appear trustworthy without necessarily being accurate.

As a result, future development will focus on visualising uncertainty and exposing the assumptions embedded within algorithmic interpretation systems.

---

## Progress Report Summary

At this stage, ECHO//PROFILE has evolved from a behaviour-tracking experiment into a critical data-driven visualisation that explores how digital systems construct assumptions about identity through behavioural information.

The project began by investigating how user actions such as movement, interaction frequency, and inactivity could be recorded as data. Early prototypes focused primarily on behaviour tracking and profile generation. However, through feedback, experimentation, and reflection, the project gradually shifted towards questions of interpretation, uncertainty, and algorithmic authority.

A major development since Week 8 has been the introduction of confidence systems, profile volatility, and intentional misclassification. These additions allow the prototype to expose how behavioural information can be transformed into convincing yet potentially unreliable interpretations.

Rather than presenting generated profiles as objective representations of identity, the current prototype highlights the instability of behavioural interpretation and encourages users to question the assumptions embedded within algorithmic systems.

The project is now focused on three interconnected themes:

* Behavioural Data Collection
* Algorithmic Interpretation
* Identity Construction and Uncertainty

The current challenge is moving beyond interface-based feedback and exploring how atmosphere, environmental transformation, and visual behaviour can communicate interpretation more effectively.

Moving forward, I intend to further develop atmosphere generation and uncertainty visualisation while reducing reliance on traditional dashboard-style interfaces.

### Questions for Feedback

1. How can uncertainty be communicated visually rather than through text?

2. Should generated profiles become increasingly unstable over time?

3. How can atmosphere communicate behavioural interpretation more effectively than profile panels?


# Making Sprint

## Sprint Goal

Following the feedback received during the Round Robin discussions, I identified uncertainty as the most important area for further development.

The goal of this sprint was not to improve the accuracy of the generated profile but to investigate how behavioural interpretation could become unstable, contradictory, and open to challenge.

By introducing confidence systems, misclassification events, and profile volatility, I aimed to reveal how algorithmic profiling systems construct assumptions from incomplete information.

The sprint therefore focused on strengthening the project's critical dimension rather than increasing technical complexity.

---

## Experiment 03 — Uncertainty Visualisation

### Aim

To investigate how behavioural interpretation can be communicated as a changing and unstable process rather than a fixed identity.

### Development Overview

Following feedback from Week 8, I focused on moving the project beyond interface-based profile generation and towards a more visual and experiential form of data-driven visualisation.

Previous iterations primarily communicated behavioural interpretation through profile panels, confidence scores, and textual feedback. While these systems successfully demonstrated how behavioural information could be transformed into algorithmic classifications, the experience still relied heavily on reading information rather than experiencing it.

This development phase explored how behavioural interpretation could influence atmosphere, visual behaviour, and environmental conditions. Rather than presenting identity as a fixed profile, the prototype now visualises behavioural influence through changing particle systems, profile instability, and environmental responses.

The goal was to make interpretation feel active, unstable, and continuously reconstructed.



---

### Development Focus

This sprint concentrated on expanding the interpretation layer of the prototype.

Rather than simply displaying behavioural information, the system was refined to expose the process through which behavioural data becomes identity classifications.

Key additions included:

- Dynamic confidence calculations that increase as more behavioural information is collected.
- Misclassification events that intentionally generate questionable interpretations.
- Behaviour logs that reveal how the system reaches its conclusions.
- Profile volatility indicators that show identities changing over time.
- Reflection prompts that allow users to challenge generated profiles.

These additions shifted the project from a behaviour-tracking tool towards a speculative system that questions the reliability of algorithmic profiling.

---

# Project Development

![prototype](<../assets/week-09/protoype screenshoot.png>)

<iframe src="https://editor.p5js.org/harrisonwu23/full/TYVkDdH4Q"></iframe>


![Prototype when not moving](<../assets/week-09/Prototype when not moving.png>)


<details>
<summary><b>Click to check： Prompt to gemini</b></summary>
Based on the current ECHO//PROFILE Week 8 p5.js prototype, create a Week 9 refinement.

Keep ALL existing systems:

- WASD movement
- Behaviour tracking
- Distance travelled
- Click count
- Idle time
- Session time
- Behaviour logs
- Explorer / Observer / Engaged scores
- Confidence system
- Misclassification events
- Reflection prompt
- AGREE / DISAGREE interaction
- Profile volatility graph

Do NOT remove any existing functionality.

The purpose of this iteration is to move beyond interface-based profiling and begin exploring atmosphere, uncertainty, and environmental visualisation.

The project should feel less like a dashboard and more like a data-driven visualisation experience.

--------------------------------------------------
1. Atmosphere Layer
--------------------------------------------------

Create a dynamic atmospheric system driven by behavioural interpretation.

Explorer:
- More particles
- Larger movement radius
- Expanded visual space

Observer:
- Slower particle movement
- Larger soft aura
- Calm visual behaviour

Engaged:
- Increased activity
- More connections
- More visual motion

The atmosphere should continuously respond to behavioural scores.

--------------------------------------------------
2. Uncertainty Visualisation
--------------------------------------------------

Visualise uncertainty directly.

Instead of only showing confidence percentages:

Create:

- Flickering profile labels
- Shifting identity labels
- Fluctuating profile bars
- Temporary contradictions

Examples:

Explorer
↓

Explorer?

↓

Observer?

↓

Explorer

The profile should occasionally appear unstable.

--------------------------------------------------
3. Behaviour Field
--------------------------------------------------

Create a background field generated from behaviour.

Movement:
creates particle trails

Clicks:
creates ripple waves

Idle:
creates soft fading zones

The environment should gradually become a visual record of interaction history.

--------------------------------------------------
4. Profile Drift System
--------------------------------------------------

Add a new system:

PROFILE DRIFT

Display:

Identity Stability

100%
↓
85%
↓
60%

As more behaviour is collected, the profile can evolve rather than becoming more accurate.

This should support the project's theme that identity is constantly reconstructed.

--------------------------------------------------
5. Interpretation Layer
--------------------------------------------------

Improve generated statements.

Examples:

"The system believes you enjoy exploration."

"It is possible you prefer observation."

"Previous classifications have been revised."

"Behavioural evidence remains incomplete."

The language should feel speculative and uncertain.

--------------------------------------------------
6. Reflection Layer
--------------------------------------------------

After 60 seconds display:

DO YOU AGREE WITH THIS PROFILE?

[ AGREE ]
[ DISAGREE ]

If DISAGREE is clicked:

Reduce confidence.

Trigger profile instability.

Generate:

"User challenged interpretation."

The system should visibly react.

--------------------------------------------------
7. Screenshot-Friendly Layout
--------------------------------------------------

Organise the screen into:

LEFT
Raw Data

CENTER
Atmosphere Visualisation

RIGHT
Profile Generation

BOTTOM
Reflection Layer

The layout should be suitable for academic design documentation.

--------------------------------------------------
8. Code Requirements
--------------------------------------------------

- Clean and commented
- Organised into functions
- Easy to modify
- Use classes where appropriate
- Use only p5.js
- No external assets
- No external libraries

Important:

This prototype is not a game.

It is an experimental data-driven visualisation exploring:

Behaviour
↓
Interpretation
↓
Uncertainty
↓
Identity Construction
↓
Reflection

The visual atmosphere should become more important than the numerical data.

Provide complete p5.js code only.
</details>

The updated prototype introduced atmosphere generation as an additional layer of interpretation.

Behavioural actions such as movement, inactivity, and interaction frequency now influence the visual state of the environment. These changes create a visual record of behavioural activity and allow users to observe how the system responds to their actions over time.

At the same time, the profile generation system was further refined through the introduction of profile volatility and uncertainty. Generated identities are no longer presented as stable outcomes. Instead, classifications may shift, confidence levels may fluctuate, and interpretations may occasionally contradict previous assumptions.

This development reflects the project's central argument that behavioural interpretation is not objective truth but a constructed and continually changing process.

### Technical Development

This iteration required further experimentation with behaviour weighting, profile generation logic, and uncertainty systems.

I explored how behavioural variables could influence generated identities while also introducing mechanisms that destabilise those identities. The challenge was finding a balance between profile consistency and uncertainty. If the system changed too frequently, interpretations appeared random. If the system remained too stable, the critical focus on uncertainty became less visible.

Through iterative testing, I developed a system that maintains believable behavioural classifications while still exposing the instability and subjectivity of algorithmic interpretation.


## Design Evolution

The project has gradually evolved through three stages:

### Stage 01

```text
Behaviour
      ↓
Data Collection
```

Week 6 focused primarily on collecting behavioural information.

---

### Stage 02

```text
Behaviour
      ↓
Interpretation
      ↓
Profile Generation
```

Week 7 explored how behavioural information could generate algorithmic identities.

---

### Stage 03

```text
Behaviour
      ↓
Interpretation
      ↓
Misinterpretation
      ↓
Reflection
```

Week 8 and Week 9 shifted towards uncertainty, questioning, and critical reflection.

---

## Current Direction

The project has gradually shifted away from representing behavioural data and towards exposing the processes through which behavioural information is interpreted.

Rather than asking:

"Can behavioural data accurately represent identity?"

the project now asks:

"Why do we trust systems that claim to understand us through data?"

This change has significantly strengthened the critical dimension of the project.

The current direction focuses on making interpretation visible, exposing uncertainty, and encouraging users to question the authority of algorithmic systems.

This aligns closely with themes of Data Humanism, surveillance, profiling, and digital identity.

### Why This Matters

As digital systems increasingly rely on behavioural information to personalise experiences, recommend content, and classify users, algorithmic interpretations are becoming a significant influence on how people are understood online.

ECHO//PROFILE aims to make these invisible processes visible by exposing the uncertainty, assumptions, and limitations embedded within behavioural profiling systems.

Rather than encouraging trust in algorithmic classifications, the project invites audiences to critically reflect on how digital systems construct identities from incomplete information.
---


### New Skills Developed

* Dynamic profile generation
* Confidence modelling
* Behaviour weighting
* Data visualisation systems
* Real-time interface updates
* Behaviour volatility tracking

---

### Updated Interpretation System

```text
Distance Travelled
      ↓
Explorer Score

Idle Time
      ↓
Observer Score

Click Count
      ↓
Engaged Score

Behaviour History
      ↓
Confidence

Confidence
      ↓
Profile Authority
```

---

### Technical Reflection

Developing the uncertainty systems revealed how strongly design decisions influence interpretation.

Throughout the process, I experimented with different behavioural weightings, confidence calculations, and profile generation rules. Small changes in these systems often produced dramatically different identity classifications despite using the same behavioural data.

This demonstrated that behavioural interpretation is not an objective process. Instead, it is shaped by the assumptions built into the system.

The prototype therefore became an example of how data can be transformed into multiple possible interpretations rather than a single objective truth.

This insight became one of the most significant conceptual outcomes of the project and further reinforced its connection to Data Humanism.

---

# Progress Report Preparation

## Current Project Status

## Current Project Status

### Completed

- Behaviour Tracking System
- Data Collection Interface
- Real-Time Behaviour Logging
- Profile Generation System
- Confidence Calculation System
- Reflection Layer
- Misclassification Events
- Behaviour Volatility Indicators

### Currently Developing

- Atmosphere-Based Visualisation
- Uncertainty Visualisation
- Environmental Responses
- Alternative Profile Representations

### Key Direction

The project has moved from behavioural tracking towards exposing how algorithmic systems construct assumptions about users through incomplete behavioural information.

Future development will focus on making these interpretations visible through atmosphere, visual transformation, and interaction rather than relying solely on interface-based feedback.

---

## Feedback Questions

### Question 01

How can uncertainty be visualised beyond text-based interfaces?

### Question 02

Should the generated profile become more unstable over time?

### Question 03

How can atmosphere communicate identity construction?

---

# Reflection

This week focused on clarifying the project's direction and committing to a specific design position.

The process of drafting the project statement helped consolidate several weeks of experimentation and reflection into a coherent argument. Rather than seeing the project as a behavioural tracking system, I now understand it as a critical investigation into how digital systems construct assumptions about people through data.

The feedback received during peer discussions highlighted that the most compelling aspect of the project is the relationship between confidence and uncertainty. Participants often trusted the generated profiles despite recognising that the underlying data was incomplete. This tension became increasingly important to the project's direction.

The Making Sprint further reinforced the idea that uncertainty should not be treated as a limitation but as a design opportunity. By visualising instability, contradiction, and misinterpretation, the project becomes less about predicting identity and more about questioning how identity is constructed.

Moving forward, I will continue developing uncertainty as a visible component of the experience while exploring ways to communicate interpretation through atmosphere and environmental transformation rather than solely through interface elements.

This week also clarified a significant shift in my understanding of data visualisation.

Initially, I approached data visualisation as a method for representing information. Through experimentation and critique, I increasingly began to view visualisation as a process of interpretation.

This distinction has become central to ECHO//PROFILE. Rather than visualising data itself, the project now focuses on visualising the assumptions, uncertainties, and consequences that emerge when data is transformed into identity.
---

## AI Usage Statement

ChatGPT was used to assist with brainstorming, project planning, project statement development, documentation structure, reflection writing, and development planning. All experimentation, coding implementation, interpretation, design decisions, and final outcomes were reviewed, modified, and developed by the author.
