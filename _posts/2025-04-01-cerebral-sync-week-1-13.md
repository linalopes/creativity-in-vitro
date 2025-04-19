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


## [Live Lab] How to Build Your Own _Codex_ - technical approach

> This section is both a guide for Eduardo Padilha and a memory capsule for anyone else who might one day join the knowledge management ecosystem.  
> One that holds your research, your chaos, your pattern of thought.  
> This is an infrastructure for alive thinking.

### Step 1: Install Obsidian and Start Thinking

Download [Obsidian](https://obsidian.md/) and install it on your machine.

Create your first Vault. Name it something that matters.  
This will be your personal thinking ecosystem — your seed space.

Start writing. Take notes. Connect them.  
Get to know how Obsidian thinks with you.

### Step 2: Create a Jekyll Site _Inside_ Your Vault

Now, let’s give your thoughts a spine.

You’re going to install [Jekyll](https://jekyllrb.com/), a static site generator that turns Markdown into a navigable site — perfect for sharing your research with the world (or just with yourself in another form).

#### Mac:

Make sure you have [Homebrew](https://brew.sh/) installed.

```bash
brew install ruby
gem install --user-install bundler jekyll
```

#### Windows:

Install [RubyInstaller for Windows](https://rubyinstaller.org/), and make sure to check the option to install DevKit.

Then, in the terminal:

```bash
gem install bundler jekyll
```

#### Now go into your Vault folder and create your Jekyll site:

```bash
cd path/to/your/obsidian/vault
jekyll new .
```

You’ll be prompted about overwriting files — say yes if you’re ready.

Your Jekyll site now _lives inside_ your Vault. Markdown meets structure.

### Step 3: Create a GitHub Account

If you don’t have one yet, create a [GitHub account](https://github.com/).

Think of GitHub as your time machine and your publishing partner.  
It hosts your site, keeps version history, and enables collaboration with future you (or others, if you want).

### Step 4: Install Git on Your Computer

#### Mac:

```bash
brew install git
```

#### Windows:

Install Git from [git-scm.com](https://git-scm.com/download/win)  
After installation, use Git Bash for terminal commands.

#### Then configure your identity:

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```


### Step 5: Initialize Your GitHub Repository

In your terminal, inside your Vault/Jekyll folder:

```bash
git init
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
git add .
git commit -m "First commit"
git push -u origin main
```
Make sure your GitHub repo already exists (create it on the GitHub site before pushing).

### Step 6: Connect Obsidian with GitHub and Publish Your Codex

This step is how your Códex becomes a living website.

You’ve already initialized your Git repository and pushed to GitHub. Now we’ll connect your Obsidian Vault to GitHub and enable **GitHub Pages** to publish your site.

#### a) Enable GitHub Pages on Your Repository

1. Go to your GitHub repository page.
    
2. Click on **Settings** > **Pages** (or find it in the sidebar under “Code and automation”).
    
3. Under **Source**, select `Deploy from a branch`.
    
4. Choose the `main` branch and click **Save**.
    
5. GitHub will generate a public URL like:  
    `https://yourusername.github.io/your-repo-name/`
    

<mark style="background: #FFB8EBA6;">Keep this link — it’s your Codex’s address in the world.</mark>


#### b) Install and Configure the Obsidian Git Plugin

In Obsidian:

1. Go to **Settings** > **Community Plugins**
    
2. Click **Browse**, search for “Obsidian Git” and install it.
    
3. Enable the plugin.
    

Then configure the plugin (in **Settings > Obsidian Git**):

- **Auto commit-and-sync interval**: `10` minutes
	
- **Auto commit-and-sync after stopping file edits**: ✅ 
	
- **Auto Pull on Startup**: ✅ (Yes — this keeps your Vault up to date)
    
- **Commit Message**:  
    Use something like:  
    `"daily commit: {{date}}"`  
    Or customize to your style.
    
- **Vault backup path**: set this to the folder where your Jekyll site lives inside your Vault.


🔄 **Recommended settings for collaboration**

These options help avoid conflicts and keep both ends in sync:

- ✅ **Commit-and-sync** → enables a full sequence:  
    `stage changes → pull from GitHub → commit → push to GitHub`
    
- ✅ **Push on commit-and-sync** → sends your commit immediately after saving
    
- ✅ **Pull on commit-and-sync** → pulls the latest changes before applying yours
    

With these three turned on, you just need to run `Commit and Sync` — and your local vault and remote site will stay aligned.

Perfect for duos, distributed teams, or multi-device workflows.

#### c) Authenticate GitHub from Obsidian

If this is your first time pushing to GitHub, you’ll be prompted for authentication.

- If using **HTTPS**, you may need to enter a **GitHub Personal Access Token** as password.  
    [Generate it here](https://github.com/settings/tokens?type=beta) — make sure it has `repo` permissions.
    
- If using **SSH**, make sure your keys are set up locally and added to GitHub.
    

After the first push, your commits will flow directly from Obsidian.

#### d) Push to GitHub from Obsidian

It's set to run automatically as described above.

Once pushed, GitHub will automatically rebuild your Pages site in a few seconds.

Check your published site at:  
`https://yourusername.github.io/your-repo-name/`

Welcome to the networked chaos.  
Your Codex is now alive.


### Step 7: Serve Your Codex Locally (Optional)

If you want to preview your site as you build it, run:

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000` in your browser.

This is your Codex, live and breathing.


### Final Notes

This is not about tools. It’s about structure for your complexity.

Obsidian holds your thoughts.  
Jekyll gives them form.  
GitHub gives them memory and reach.

Let your _Codex_ grow as you do.  
Between the precise and the poetic.  
Between the unfinished and the infinite.