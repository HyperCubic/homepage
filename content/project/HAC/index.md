---
title: Hierarchical Imitation Learning for maze navigation
summary: Train an ant to navigate through a maze
tags:
- Reinforcement Learning
- Imitation Learning

# Optional external URL for project (replaces project detail page).
external_link: ""

profile: false
share: false
show_date: false
date: 2019-12-01

image:
  focal_point: Smart

links: ""
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

## Introduction

Automatic navigation is an interesting research problem where agent needs to control its limbs and meanwhile find direction to its destination. Hierarchical structure is a natural way of solving this problem. In this project, we first train the low level controller that is able to control the ant to navigate to a certain direction. After that, we train a high level controller using DAgger so that the high level controller can adapt to certain maze. With this method, we successfully train an ant agent navigate from a certain spot to another spot in the maze. Beyond that, we also explore the effect of active learning to improve the sample efficiency of our training process.

## Demos

##### Training
In this stage, we use cursor to guide the agent to destination (yellow cube). Note that because of DAgger, the immediate target (purple cube) does not necessarily coincide with cursor.
{{< video src="training.mp4" controls="yes" >}}


##### Testing
In this stage, the ant is randomly initialized in the maze with a randomly initialized destination. The algorithm will automatically lead the ant to the target.
{{< video src="testing.mp4" controls="yes" >}}
