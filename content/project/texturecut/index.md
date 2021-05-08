---
title: Automatically cut texture with importance map
summary: A pipeline automatically generates/optimizes texture image from a textured mesh
tags:
- Computer Graphics
- Texture Image
# Optional external URL for project (replaces project detail page).
external_link: ""

profile: false
share: false
show_date: false
date: 2019-05-01

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

### Introduction

To reduce distortion of a texture image, people use energy function to quantize distortion and optimize on it in order to generate texture image that save most of the information. Based on {{< staticref "https://github.com/Roipo/Autocuts" "newtab" >}}AutoCuts{{< /staticref >}}, we implement a pipeline that not only generate texture images with low distortion, but also consider the content of texture image: namely we do not cut through important area on texture image.

### Demo

{{< video src="Parameterize.mp4" controls="yes" >}}

{{< figure src="EarthMap_2500x1250.jpg" caption="Original texture image" >}}
