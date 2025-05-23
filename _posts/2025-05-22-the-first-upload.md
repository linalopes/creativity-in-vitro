---
layout: post
title: The First Upload
id: 2025-05-22-the-first-upload.md
categories:
  - neural harvest
image: https://img.youtube.com/vi/DI5rSIaVZdE/maxresdefault.jpg
share: "true"
comments: "true"
filename: creativity-in-vitro/_posts/2025-05-22-the-first-upload.md
tags: 
date: 2025-05-22
author: lina
---
### Part I — _Data, Memory, and Toquinho_

There’s a moment — somewhere between experiment and ritual — where data begins to feel like memory.

On May 19th, 2025, I uploaded the first raw EEG dataset for _Creativity in Vitro_. It’s a fragile thing, both poetic and procedural: **20 repetitions** of the same **three-loop sequence** of **six lyrical phrases** from _Aquarela_ by Toquinho. Listened to with eyes closed, body still. Recorded continuously, without restarting the interface. Like a mantra looping in the cortex.

Each repetition is the same — and yet, not. Same phrases, same melody. But each loop is **a different brain**, a slightly different Lina. After each three-loop session, I blinked **three times**, deliberately. The blink acted as a **biological marker**, a ripple left in the EEG trace — not to be removed, but to be used.

These sessions were recorded with **OpenBCI Cyton + Daisy**, using **14 gel-based electrodes** arranged according to the **10–20 system**, skipping N9P and N10P for better spatial integrity. The headset doesn’t visualize Fz or Pz, but those points are present in the data — subtly pulsing in microvolts.

Here’s what I discovered:

- The OpenBCI GUI doesn’t create a new file each time you stop and start a session. It appends everything into a **single .csv file**.
    
- At first, this created confusion — signals seemed to "flatline" and restart. But those **gaps were meaningful**: each one marked the end of a session and the beginning of another.
    
- I wrote code to detect those gaps in the **timestamp** column and used them to split the full file into **20 distinct blocks**.
    
- Each block was then trimmed: **7 seconds from the start**, **3 seconds from the end**, to remove noise and stabilization.
    

These 20 blocks — now cleaned and organized — were saved as `.pkl` files.  

In a second notebook, I reopened them to identify the **blink markers** between loops. I didn’t insert any digital triggers — just **pulses of the eyelid**, visible in Fp1 and Fp2. I scanned the signal for **two blinks** per block, and used them to divide each session into **three loops**. That is supposed to give me 60 recordings in total — 3 per block, each tied to a listening of six phrases. Once I can confidently split each session into the 3 loops, the next challenge is to segment each loop into the six lyrical phrases — and that’s where I would really appreciate any insight now.

Next, I’ll divide each loop into six temporal slices, one per phrase — probably by second. It’s not perfect. It’s not clinical. But it’s **radically personal**, and **methodologically transparent**.

The data is raw, human, messy — not a simulation, not synthetic, not idealized. It’s my brain, listening to _Aquarela_, over and over again.  

And now, it’s [available](https://github.com/linalopes/creativity-in-vitro-eeg)



<iframe width="100%" height="400" src="https://www.youtube.com/embed/DI5rSIaVZdE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Part II — _How to Version Raw EEG Data on GitHub with Git LFS_

Uploading large EEG recordings to GitHub requires a few extra steps, since the platform has a 100MB file limit. To manage this, we used **Git Large File Storage (LFS)** to track and store the 122MB `.csv` file. Here's a quick protocol for others working with physiological data:

```zsh
# 1. Install Git LFS (only once per machine)
brew install git-lfs         # or: sudo apt install git-lfs / choco install git-lfs

# 2. Initialize Git LFS in your repo
git lfs install
git lfs track "*.csv"
git add .gitattributes

# 3. Add and commit your large file
git add your_data.csv
git commit -m "Track EEG dataset with Git LFS"

# 4. Push to GitHub (can take a few seconds for large files)
git push origin main
```

If you’ve already committed a file over 100MB, you’ll need to rewrite history using the BFG Repo-Cleaner:

```zsh
# Optional cleanup for previous commits that exceed 100MB
git gc --aggressive --prune=now
bfg --strip-blobs-bigger-than 100M
git reflog expire --expire=now --all
git gc --prune=now --aggressive
git push --force
```






