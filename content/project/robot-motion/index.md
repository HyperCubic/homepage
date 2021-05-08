---
title: Robot Control with Reinforcement Learning
summary: Generate various robot motions in simulation environment
tags:
- Reinforcement Learning
- Computer Animation
- Physics Simulation

# Optional external URL for project (replaces project detail page).
external_link: ""

profile: false
share: false
show_date: false
date: 2020-11-01

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

This project aim at training robot to perform highly dynamic skills using a vectorized simulation environment called {{< staticref "https://raisim.com/" "newtab" >}}RaiSim{{< /staticref >}}. We use Reinforcement Learning (more specificly PPO) to train a robot to perform several highly dynamic skills such as running jump, flipping, double jump and wall flipping. To make the training easier, we also use Curriculum Learning that gradually change the environment and reward function so that the agent's policy does not get trapped in a local maximum.

## Demos

##### Running Jump
{{< video src="running_jump.mp4" controls="yes" >}}


##### Backflip
{{< video src="backflip.mp4" controls="yes" >}}

##### Sideflip
{{< video src="sideflip.mp4" controls="yes" >}}

In order to succeed, we make it easier in the following two tasks: the trunk of robot can only move in its sagittal plane and robot's motion is also symmetric about its sagittal plane.

##### Double Jump
{{< video src="double_jump.mp4" controls="yes" >}}

##### Wallflip
{{< video src="wallflip.mp4" controls="yes" >}}
