---
layout: post
title: On the Boat of Touch Designer
id: 2025-05-05-on-the-boat-of-touch-designer.md
categories:
  - relic table
image: https://img.youtube.com/vi/k358cln4OiY/maxresdefault.jpg
share: "true"
comments: "true"
filename: creativity-in-vitro/_posts/2025-05-05-on-the-boat-of-touch-designer.md
tags: 
date: 2025-05-05
author: lina
---

## A short summary

**Exploring TouchDesigner + Stable Diffusion via ComputerRender API**  

As part of the _Creativity in Vitro_ project, we explored using Torin Blankensmith’s TouchDesigner setup for Stable Diffusion image generation. Without a local GPU, we successfully used the **ComputerRender** API to generate prompts and images directly in TouchDesigner. This method proved lightweight, fast, and cost-effective — ideal for Mac M3 users or anyone experimenting without heavy hardware. The test animation was based on the Brazilian song _Aquarela_, turning lyrics into visual prompts. This experiment reflects our ongoing search for poetic and accessible ways to collaborate with machine imagination.


<iframe width="560" height="315" src="https://www.youtube.com/embed/mRXTR9vcHAs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## The Cloud Rendered a Boat

We are still in **Phase 1** of _Creativity in Vitro_ — the phase of construction, not connection. No neural helmet has yet been donned, no brainwave has whispered its prompt to the machine. But the question ahead is clear:

**Once the model is trained — how will we render its dreams?**

This phase is one of rehearsal.  
In preparation for the moment when brain signals will be translated into text, we now experiment with the second half of the pipeline: **image generation**. After our first test with _ComfyUI_, we turn now to another conjuring tool — **TouchDesigner + Stable Diffusion**.

These are not just software trials. They are _proto-conversations_ with the machines that will one day visualize the interiority of an artist’s mind.  

They ask:  **How do we co-create with visual engines, before the mind arrives?**

To bring this to life, we turned to a new hybrid: **TouchDesigner + Stable Diffusion**. While TouchDesigner provides the spatial logic and compositional canvas, Stable Diffusion brings the latent generativity — a way to summon images from text.

But there’s a caveat.

As a Mac M3 user, my machine lacks the GPU infrastructure needed to run Stable Diffusion locally. Rather than forcing a friction-heavy setup, we sought an alternative: **external rendering through the cloud**. Enter **Computer Render API**, a gateway generously shared by TouchDesigner community alchemist [Torin Blankensmith](https://www.youtube.com/@blankensmithing). In his meticulous [tutorial](https://derivative.ca/community-post/tutorial/generate-ai-images-stable-diffusion-using-image-image-generation-any-top), we found a method to invoke image generation remotely — directly from within TouchDesigner, using a node-based structure of **TOPs** (Texture Operators).

So, I bypass the need for a local GPU by invoking [Computerender](https://computerender.com/), an external API that transforms prompts into images. The latency was minimal, and the process cost only $0.10 for 74 calls. Compared to our earlier rituals with _ComfyUI_ running locally on an M3 Mac, the responsiveness felt like a breath of warm data.

Our first subject: the song _Aquarela_ by Brazilian bard Toquinho. A children’s song in name only, it unfolds a surrealist map of emotional geographies. We chose a single verse — the boat — and submitted its aura as a prompt. The model responded gently.

We also gained new language from this interaction:

- **Seed**: the number that decides the fate of the image.
    
- **Guidance Scale**: how tightly the image follows the text.
    
- **Strength**: how much the input image influences the result.
    

This is only our second contact with TouchDesigner, yet it welcomed us with visual logic and forgiving workflows. The _.toe_ file provided by Torin became our summoning circle.

More experiments to follow. For now, we offer this test animation — a visual echo of a boat, born not from water, but from _latent space_.


<iframe width="100%" height="315"
  src="https://www.youtube.com/embed/k358cln4OiY"
  frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowfullscreen>
</iframe>

📌 _Note to the future self:_ This phase is not about fidelity to vision, but _trust in translation_.  
We ask the machine to imagine, because we, too, are learning how.
