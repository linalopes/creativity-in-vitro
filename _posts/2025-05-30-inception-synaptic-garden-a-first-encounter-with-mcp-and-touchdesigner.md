---
layout: post
title: Inception Synaptic Garden - a First Encounter with MCP and TouchDesigner
id: 2025-05-30-inception-synaptic-garden-a-first-encounter-with-mcp-and-touchdesigner.md
categories:
  - relic table
image: https://img.youtube.com/vi/Hll6cFu_QMI/maxresdefault.jpg
share: "true"
comments: "true"
filename: creativity-in-vitro/_posts/2025-05-30-inception-synaptic-garden-a-first-encounter-with-mcp-and-touchdesigner.md
tags: 
date: 2025-05-30
author: lina
---
> _What if your imagination could run continuously, generating images in real time, and other people could interfere—whispering thoughts, injecting metaphors, remixing your neural garden?_


<iframe width="100%" height="400" src="https://www.youtube.com/embed/Hll6cFu_QMI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


That’s the kind of question that led me to explore the **Model Context Protocol (MCP)** for the first time. I had never heard of MCP before, but it quickly became clear that this emerging protocol offers a radically new interface: it lets large language models (LLMs) like Claude not just answer questions, but **act on your computer**, creating things for you in real time—visuals, animations, structures, ideas.

This post is a three-part documentation: a technical experience report, a reflection on creative learning, and finally a glimpse of a possible third phase of _Creativity in vitro_—one in which cultivated imagination becomes collective imagination.

---

## PART 1 — First Contact with MCP and TouchDesigner

MCP stands for **Model Context Protocol**, and it's a JSON-RPC-based bridge that allows language models like Claude to interact directly with tools like Blender, Python, or TouchDesigner. Rather than sending you a code snippet to copy and paste, the model itself performs actions: creating nodes, connecting operators, transforming geometry—live, in your machine.

The protocol is built on top of **JSON-RPC**, a lightweight, language-agnostic protocol (created in 2005) that allows clients to call methods on remote systems using plain JSON.

In my case, I used [touchdesigner-mcp](https://github.com/8beeeaaat/touchdesigner-mcp), which runs as a local Docker container that listens for JSON-RPC instructions coming from Claude.

### Setup process (summarized):

1. Cloned the repo and copied `.env` from the example file
    
2. Ran `docker compose up -d`
    
3. Edited `config.json` in Claude Desktop with the correct `docker-compose.yml` path
    
4. Switched the port from 9981 to 8090 after initial connection issues
    
5. Launched the MCP server with:
    

```
docker compose exec -i touchdesigner-mcp-server node dist/index.js --stdio
```

6. Claude connected and I started with very basic prompts like:
    

```
Create a Circle SOP called petriBase inside /project1
```

#### One note missing from the official docs:

They tell you how to launch Docker with `up -d`, but **not how to bring it down**, which was essential for me every time things got stuck:

```
docker compose down
```

---

## PART 2 — Learning to Speak to Machines (and to Myself)

I’m not an experienced TouchDesigner user. I first tried it in 2020, but my computer at the time couldn’t handle it. Over the years I tried again here and there, but it wasn’t until this year that I decided to explore it for real.

Coming from environments like **Arduino, Processing, p5.js, D3.js, and Pure Data**, TouchDesigner felt... different. It’s visual like Pure Data, sure, but the logic of operators, COMPs, SOPs, CHOPs and the nested architecture took time to sink in. Maybe the closest tool I’ve used before was **Grasshopper** in Rhino, especially for procedural geometries. Still, Touch has its own rhythm.

Why mention this? Because when I started asking Claude to do things via MCP, I quickly realized I had to speak _very clearly_ and go _step by step_. If I gave Claude four or five instructions in one go, things got messy. But if I gave them one by one, not only did it work—it taught me what was going on.

I also realized I need to learn to **speak TouchDesigner better**. The more I know about how nodes are built and connected, the more expressive my conversations with Claude can become.

But even with all these limitations, I was genuinely surprised: within 30 minutes, I had a working scene with instanced spheres, animated with noise, rendered with glow, and built through natural language.

⚠️ I also had to upgrade to **Claude Pro**, since the free plan has a much smaller token limit (around 8k) and disconnects quickly during MCP sessions. The Pro version allowed longer conversations and proper control of TouchDesigner.

As someone who had never built an animation with spheres and procedural logic in TD before, I was genuinely amazed. MCP is not just a protocol—it’s a **creative co-driver** that transforms words into structures.

---

## PART 3 — Imagining a Phase Three: Inception Synaptic Garden

If _Creativity in vitro_ began by cultivating imagination as something grown in vitro—from organoids, from EEG, from memory and machine learning—this next phase invites the world into the dish.

**What if your cultivated imagination could run in real time, as a scene rendered in TouchDesigner, and other people could interact with it—talking, suggesting, distorting, remixing?**

That’s the idea behind a speculative system I’m calling:

### 🧠 _Inception Synaptic Garden_

A generative environment seeded with your imagination—either through pre-trained ML models, text corpora, or neural signals—and made **editable** by other humans, in real time.

People can speak or type; Claude interprets these acts as “injections” into your running system.

The result is not just a collaborative art piece—it’s:

> A system where **language is planted and image grows**.  
> A way of saying that the **mind is porous, cultivable**, and that **authorship is ecological**.  
> A mode of using the MCP as a **living bridge between the organic and the digital, between the intimate and the collective**.

Let this be a seed.
