---
layout: post
title: Field Note on Navigating Knowledge with GraphRAG · with Gabriel Frontera
id: 2025-04-17-field-note-on-navigating-knowledge-with-graphrag-with-gabriel-frontera.md
categories:
  - alchemists
  - code operatory
image: https://microsoft.github.io/graphrag/img/GraphRag-Figure1.jpg
share: "true"
comments: "true"
filename: creativity-in-vitro/_posts/2025-04-17-field-note-on-navigating-knowledge-with-graphrag-with-gabriel-frontera.md
tags: 
date: 2025-04-17
author: lina
---
**Codex Entry 047 · April 2025**  
**Participants:** Lina Lopes, Eduardo Padilha, Gabriel Frontera  
**Connected by:** Pedro Terra

> _“Everyone here is trying to organize knowledge.”_

This note captures a meeting that began as an introduction and quickly turned into a convergence of epistemological strategies.

We had the chance to present _Creativity in vitro_ to Gabriel Frontera — currently working at Cloudwalk — invited by Pedro Terra, who suspected a fertile crossover between our practices.

Gabriel, who deals with massive and rigid technical documentation (payment systems, regulatory manuals, corporate dead matter), brought his tools for breathing relational life into static texts. And what emerged, in between the pulses of LLMs, graphs, and queries, was the shared obsession: **How do we inscribe knowledge into navigable form?**

### **GraphRAG, or the semi-living skeleton of texts**

Gabriel introduced a system that extracts meaning out of markdowns and PDFs — not as keywords, but as **concepts**. It's the GraphRAG, a tool that uses LLMs to:

- Create **tables of entities**: each with a concept title, a generated description, and usage frequency.
    
- Map **relationships** between entities, constructing a kind of **conceptual lattice**.
    
- Visualize this as a **Knowledge Graph**, not unlike the connective tissue of a brain... or a creature stitched from texts.
    

These aren’t word clouds. These are **semantic organs**.

A single word like _bank_ can refer to a place to sit or a place to save money — GraphRAG retrieves the _contextual identity_ of that word and maps its place within a cognitive structure.

> _The algorithm is not looking for noise — it’s sketching the internal organs of an idea._

### **The Nicolelis Echo**

When we shared the broader vision of _Creativity in vitro_ — brainwaves, speculative intelligence, narrative organs — Gabriel remarked:

> _“This reminds me of Nicolelis.”_

A comparison that humbled us. Nicolelis builds neural bridges across continents and rats; we, perhaps, build poetic bridges between AI and inner life. Still — we felt the spark.

Gabriel himself is exploring health and wearables as a research path. The idea of using graph structures to trace not only **semantic relationships**, but also **patterns in lived data**, felt uncannily close to our own work.

### **Shared Questions (still bleeding):**

- What is a **Semantic Ontology**, and how is it built?
    
- What makes a **Knowledge Graph** different from a vector database?
    
- At what stage does the graph emerge — **before or after** LLM analysis?
    
- What does it mean to **“knowledge graph”**? What techniques can we use to do so?
    
- How do we define a **concept**, as opposed to a word?
    
- What determines **community structure** inside a graph?
    
- How can graphs reveal **latent tensions and invisible linkages** between texts?
    
- Can we use graphs to trace **conceptual evolution over time**?


## Traces from the Conversation: Tools & Links

During our conversation, Gabriel shared a few resonant references — useful for anyone interested in animating a corpus of texts into a living, relational entity.

**Walkthrough video**

A clear and engaging walkthrough of GraphRAG in action:

<iframe width="560" height="315" src="https://www.youtube.com/embed/6vG_amAshTk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


**Converting PDFs into usable text**

To feed your own documents into GraphRAG (or any NLP workflow), it’s often helpful to convert `.pdf` files into `.txt` or `.md`. Gabriel suggested using:

- [Docling – usage guide](https://docling-project.github.io/docling/usage/)
- [Docling CLI reference](https://docling-project.github.io/docling/reference/cli/)

⚠️ _Note: Very large documents (1000+ pages) may take several hours to process._


**Official GraphRAG documentation**

Dive into Microsoft’s own explanation of the system — including how it builds hierarchical community graphs, and how it enhances LLM responses via graph-structured retrieval.

🔗 [GraphRAG · Microsoft GitHub](https://microsoft.github.io/graphrag/)

