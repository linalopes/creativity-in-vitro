---
layout: post
title: Protocolo ComfyUI
id: 2025-04-27-protocolo-comfyui.md
categories:
  - relic table
image: https://img.youtube.com/vi/4_37qy9Rfr0/maxresdefault.jpg
share: "true"
comments: "true"
filename: creativity-in-vitro/_posts/2025-04-27-protocolo-comfyui.md
tags: 
date: 2025-04-27
author: lina
---
On our ongoing exploration of _Creativity in Vitro_, where the boundaries between biological imagination and artificial cognition blur under the microscope, we opened a new window—this time into the modular dream-world of **ComfyUI**.

What began as a technical curiosity—a guide to installing ComfyUI on an M3 Mac and deploying it via Google Colab—quickly evolved into a collective exercise in **co-creating machine hallucinations**. We weren’t just learning how to run nodes or style-transfer images. We were learning how to think _with_ the machine, in the fragmented visual grammar of latent spaces.

This study group marks an embryonic stage in our computational wetware—a shared interface for generating, remixing, and intervening in aesthetic processes driven by AI. As always in our Codex, we weren't just asking _how_ to use the tool. We asked: **what kind of imagination is this interface enabling? And whose dreams are we amplifying when we run the prompt?**

TouchDesigner met Teachable Machine in one of the nodes. Open-source pipelines and no-code plugins blurred the line between technical mastery and sensory speculation. We began imagining systems where _organisms train algorithms_, where _gesture teaches logic_, and where _training data becomes a new kind of mythology_.

As we scale up our experiments—from brainwave-responsive GANs to Petri-dish imaginations—this technical detour serves as a vital neural scaffold. A sketch of a possible future where **creativity is modular, embodied, and distributed**.

Because in vitro or in silico, we’re still asking the same question:

> _Can the machine learn to dream us back?_


## Comfy UI Installation in Mac OS

- [ComfyUI on Mac OS](https://comfyui.org/en/install-comfyui-on-m3-macbook-pro)


```bash
conda create -n comfyui python=3.10 -y
conda activate comfyui
```

```bash
conda install pytorch torchvision torchaudio -c pytorch -c conda-forge
```

```bash
brew install cmake protobuf rust
```

```bash
cd ~/Documents
git clone https://github.com/comfyanonymous/ComfyUI.git
cd ComfyUI
```

```bash
pip install -r requirements.txt
```

```bash
python main.py
```


### How to Install ComfyUI and ComfyUI Manager on Google Colab

<iframe width="560" height="315" src="https://www.youtube.com/embed/E6VQptMs0zY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


## Style Transfer (Very Good) Tutorial

In this tutorial, **Sebastian Kamph** demonstrates how to use **ComfyUI for style transfer**, guiding viewers through a workflow that merges the aesthetics of two images into a single, AI-generated composition.

<iframe width="560" height="315" src="https://www.youtube.com/embed/4_37qy9Rfr0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

