---
layout: post
title: Cerebral Sync - Week 1/13
id: 2025-01-01-cerebral-sync-week-1-13.md
categories:
  - meta-codex
image: https://room-recordings.butter.us/Gifs/e5430eef-1868-4c44-a940-e444a9719d2b/output_2.gif
share: "true"
comments: "true"
filename: creativity-in-vitro/_posts/2025-01-01-cerebral-sync-week-1-13.md
tags: 
date: 2025-04-01
author: lina
---
## [Live Lab] Architectures for Chaos

When Eduardo Padilha and I sat down for our very first meeting, we both knew what we were getting ourselves into—or rather, we knew that we didn’t fully know. The scope of _Creativity in vitro_ was never meant to be linear or contained. It’s a living system of processes, a constellation of investigations that open up tabs we may never close. Some paths we’ll follow. Others will stay suspended in the air, waiting for another time, or someone else.

We’re both familiar with the chaos of creative research: layers of scientific documentation, speculative ideas, fragments of fiction, maps of references, scattered across disciplines and temporalities. Each micro-investigation might become a full prototype, a beautiful failure, a fork in another project, or simply a node in someone else’s future. The only way to navigate this living landscape was to design a system that could hold the weight of complexity while remaining fluid.

So we decided to create a _codex_.

Not just a place to document what happens—but a place where what happens can be shaped. A breathing record. And for that, we needed structure.

Because this isn’t the first time Padilha and I have worked together, we already know each other’s quirks and methods. <mark style="background: #FFB8EBA6;">We know our madness has method</mark>. So we started, as we always do, by building an information architecture—a structure for a system that could grow organically, between the complex and the chaotic.

We chose tools that made sense to us. Tools that could expand as the project evolves. Tools we could teach each other. Not because the tools themselves are sacred, but because they serve the system we imagined.

For the architecture of our _codex_, we rely on a triad I’ve grown to love: **Obsidian**, **Jekyll**, and **GitHub Pages**.

Obsidian is where my brain lives. It’s a Personal Knowledge Management (PKM) system that works with Markdown and allows me to create atomic notes, networked thoughts, and daily reflections through the [Zettelkasten](https://en.wikipedia.org/wiki/Zettelkasten) method. It’s flexible, lightweight, and supported by a vibrant open-source community of plugins and integrations. For chaotic thinkers like me, it’s a generous space to grow ideas from seed to structure.

Inside Obsidian, I run a **Jekyll** instance—a static site generator that plays beautifully with Markdown. It’s where our _codex_ takes form and becomes readable, navigable, alive. Jekyll allows us to weave our entries, tags, metadata, and references into a growing body of documentation that looks and feels like a living manuscript.

And finally, all of it lives online via **GitHub Pages**—our public server, our versioning history, our bridge between local thinking and global visibility.

But before any of this was technical, it was a decision: 

> To treat process as form. To make visible the invisible. To honor the path, not just the outcome.


## [Live Lab] How to build a _Codex_ - technical approach

> This section is both a guide for Eduardo Padilha and a memory capsule for anyone else who might one day join the knowledge management ecosystem.  
> It's not just about _what_ to install, but _why_ these pieces matter and how they talk to each other.

### What you are going to do

- A GitHub account
- Obsidian installed
- Git plugin activated in Obsidian
- Git installed and authenticated on your computer (either via SSH or token)
- A cloned repository containing the Jekyll structure
- Jekyll dependencies installed (Ruby + Bundler)


We’ll walk through each of these below, with Mac and Windows options where needed.

### 1. Install Obsidian

Download and install [Obsidian](https://obsidian.md/) for your operating system.

Once installed:

- Open the cloned repository folder as a Vault.
- Install the **Obsidian Git plugin** via Settings > Community Plugins.

### 2. Install Git on Your Machine

#### Mac:

If you type `git` in Terminal and it’s not installed, it will prompt you to install it. You can also install via Homebrew:

```bash
brew install git
```

#### Windows:

Download and install Git for Windows:  
[https://git-scm.com/download/win](https://git-scm.com/download/win)

After installation, open Git Bash to use terminal commands.