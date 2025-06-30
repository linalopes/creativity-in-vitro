---
layout: post
title: Demo Day - A reflection on learning, signals, and collective minds at work
id: 2025-06-28-demo-day-a-reflection-on-learning-signals-and-collective-minds-at-work.md
categories:
  - neural harvest
image: https://img.youtube.com/vi/3u_ui4kzc68/mqdefault.jpg
share: "true"
comments: "true"
filename: creativity-in-vitro/_posts/2025-06-28-demo-day-a-reflection-on-learning-signals-and-collective-minds-at-work.md
tags: 
date: 2025-06-28
author: lina
---

> When the Brain Whispers, the Machine Listens

We stepped into the final 40 hours of the Le Wagon Data Science bootcamp not as engineers, but as listeners. Not yet of machines, but of ourselves — of our questions, our assumptions, our quiet doubt. What began as a course in data science became, for us, a living laboratory of thought and intention. A place where _Creativity in Vitro_ — our speculative research on brain-computer interfaces — could unfold not in solitude, but in sync with others.

> _“What if you could write just by thinking?”_  
> That’s how we opened our final pitch. And it wasn’t rhetorical. We meant it.

Today, we live in the era of prompts. We type to create, to search, to learn, to talk to AI. But what if thought itself could become the prompt?

## A Bootcamp Designed for Brains in Transition

There’s a hidden architecture behind great pedagogy. And Le Wagon surprised us with a learning design that was not only technically rigorous but emotionally calibrated — especially for those of us migrating from other disciplines. The asynchronous material paired with the live sessions in a way that made us feel supported but not handheld. Independent, but never lost. Motivated, but never alone.

That rhythm — between self-paced challenge and collective momentum — made all the difference.

## Data That Doesn’t Confess

We decided to build a complete pipeline: OpenBCI headset, Python, Scikit-learn, MNE. Two mental instructions: _“Imagine the sun on your face”_ and _“Relax.”_ Every 4 seconds, the subject heard one of them. We collected neural signals from 8 electrodes. We cleaned, filtered, labeled, and — eventually — trained models to try and tell them apart.

> At first, the models whispered back nonsense.  
> 32% accuracy.  
> Our dataset refused to confess.  
> And yet we listened harder.

In the middle of it, someone on the team asked a question — simple, naïve — that made us rethink everything. It turned out the band-pass filter we were applying was cutting the very frequency range where imagination lived. We had built a perfect system to ignore the signal we wanted most.

> _“Torture the data until it confesses,”_ the saying goes.  
> But in neuroscience, silence is part of the message.

We pivoted. We adjusted. We breathed.

## Frequencies of Thought

After cleaning came feature extraction. And with it, the poetics of cognition:

> _“Band Power,”_ we explained, _“is like tuning into radio stations of the brain — delta, alpha, beta. Hjorth parameters capture the movement of thought: its volatility, its smoothness. Wavelets, on the other hand, are like zoom lenses — catching tiny bursts across multiple scales.”_

We fed these features into a specialized deep learning model — EEGNet. It reached 80% validation accuracy, but struggled to generalize.

Then came the surprise:  
Using just two classic features — Hjorth + Wavelet — and a LightGBM classifier, we reached **98% accuracy**. No signs of overfitting. Sometimes, simpler tools understand better than complex ones.

## A Chorus of Minds

The best questions don’t come from inside the code — they come from across the table.

Cristiane, Tito, Mario — our team — came from different backgrounds. But it was their questions, their curiosity, their beginner’s mind, that helped reshape the direction of the project. They kept asking things I had stopped questioning.

> _“I was closest to the signal. They were closest to the questions I forgot to ask.”_

Together, we laughed at failed models, ran trapinhos of debugging, and celebrated every small step toward clarity. It was a technical sprint, yes — but also a deeply human one.

## Thanks for the Signals

Many people shaped this process.

To **Rodrigo Motta**, for walking with us through the nuances of signal processing and scientific framing.  
To **Dr. João Ricardo Sato**, whose expertise in cognitive neuroscience gave rigor to our questions.  
To **Eduardo Padilha**, who keeps this dialogue between art and data alive.  
And to **CloudWalk**, the company that supported and funded this step of the journey — and never asked us to choose between imagination and implementation.

## What Comes After Thought

With just two mental states — _imagine_ and _relax_ — we created a working prototype for a non-invasive, customizable brain-computer interface. It runs on open hardware. It was trained at home.

> This isn’t science fiction.  
> It’s engineering.  
> It’s imagination, applied.

Next steps include expanding the system’s vocabulary beyond binary states. We want to explore symbolic, emotional, and even affective modes of communication. And we hope to make it open — a living system, co-created with the community.

> Because what we’re really building is this:  
> _A world where thinking is enough to communicate and be understood._

## When the Brain Whispers

If imagination was once the realm of poets and painters, we now know it has frequency bands, voltage shifts, rhythms.

And for a brief, beautiful moment at the end of our bootcamp,  
we heard it.

---
➡️ [Click here to explore the interactive Demo Day presentation](https://criatividade-demoday.vercel.app/)


<iframe src="https://criatividade-demoday.vercel.app/" width="100%" height="600" style="border: none; border-radius: 12px;"></iframe>


---

Presentation in Portuguese

<iframe width="100%" height="400" src="https://www.youtube.com/embed/3u_ui4kzc68?si=WDX_iwELrB75VDff" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>





