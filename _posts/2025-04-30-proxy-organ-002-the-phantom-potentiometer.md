---
layout: post
title: "Proxy Organ #002 — The Phantom Potentiometer"
id: 2025-04-30-proxy-organ-002-the-phantom-potentiometer.md
categories:
  - relic table
image: https://img.youtube.com/vi/51ZfV9CgdXY/maxresdefault.jpg
share: "true"
comments: "true"
filename: creativity-in-vitro/_posts/2025-04-30-proxy-organ-002-the-phantom-potentiometer.md
tags: 
date: 2025-04-30
author: lina
---


<iframe width="100%" height="315" src="https://www.youtube.com/embed/51ZfV9CgdXY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


We do not yet possess a neural headset.  
We do not yet have a working Arduino connected to sensors.  
And yet, the system breathes.

Today’s experiment explores the simulation of analog input — as if from a bodily extension, a tremor, a pulse, a ghost limb. We created a proxy organ: a digital potentiometer, simulated with p5.js, oscillating <mark style="background: #FFB8EBA6;">values from 0 to 1023</mark>. This analog ghost feeds into a Flask-based neural bridge, where it is transcribed into JSON and injected into the ComfyUI prompt as a `seed`.

Unlike other integrations — where p5.js is embedded as a node inside the ComfyUI itself (you can check Golan Levin's [github](https://github.com/golanlevin/p5-in-comfyui)) — this approach maintains a **clear external interface**, honoring the ritual of data collection as something that happens **outside** the generation engine. We chose this route to emulate real-world sensor data — EEG, muscle tension, skin conductivity — that may one day be captured from an actual human subject (or organoid).

Each change in the slider triggers a new image, seeded by the current analog value. This simulation, though simple, reveals an essential potential: a direct **brain-to-image** pipeline, mediated through proxies. A primitive loop. A prototype of intuition.

## Still to be learned:

- How to debug ComfyUI effectively;
    
- How to confirm seed mutation in the interface;
    
- How to route real signals from biosensors into this architecture.
    

But something works: two parallel servers running, a browser-based slider, and images born from the ghost of input. This small gesture opens space for what comes next: cultivating actual organoid signals to feed these same pipelines.


> _The machine listens. Even when it hears a simulation._


[Github repository](https://github.com/linalopes/arduino-comfyui)


