---
layout: post
title: Bioart Means What?
id: 2025-04-11-bioart-means-what.md
categories:
  - archive of experiments
image: https://img.youtube.com/vi/-9O5i3-ktWI/maxresdefault.jpg
share: "true"
comments: "true"
filename: creativity-in-vitro/_posts/2025-04-11-bioart-means-what.md
tags: 
date: 2025-04-11
author: lina
---
> _Tracking Vocabulary Drift Across the World Using Google Alerts, Python, and OpenAI_


<iframe width="100%" height="400" src="https://www.youtube.com/embed/-9O5i3-ktWI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


## **Act I – Motivation: a missing word**

Sometime last year, I was searching Wikipedia for a term that felt very present in my practice — **biodesign** — and to my surprise, it didn’t exist.

Together with Eduardo Padilha, we started digging for other terms we often use and navigate between. Some were there — like **bioart** — but even then, the question lingered: when I say _bioart_, is the image in your head the same as mine?

In collaborative spaces — especially in inovation — I’ve seen many meetings where people speak the same words but refer to different things. For example: "education". I've heard this word in teacher meetings used five or six different ways. Yet no one stops to ask: what do we mean by that?

And so, one of my facilitation strategies — following what Rafael Nepô calls a _controlled vocabulary_ — is to co-create shared definitions. We don’t go to the dictionary. We build the meaning together. That way, when someone says “education,” we all know which education we’re talking about.

The same applies to “intelligence” in "artificial intelligence." What kind of intelligence are we talking about? That’s probably worth another post in the Codex — but let’s stay focused on **bioart** for now.

---

## **Act II – Listening to the world say "bioart"**

To explore how this word is used globally, I set up a **Google Alerts** subscription. For those unfamiliar: you can enter any term in Google Alerts, and it will email you links every time that term appears online. It’s not the same as Google Trends — which shows you search interest — but rather, it tracks the **appearance of terms in published web content**.

I set mine to capture mentions of:

- **bioart**
    
- **biodesign**
    
- **biohacking**
    
- **3D bioprinting** 
    

And I asked it to track results **worldwide**, in **any language**.

Each day, Google sent me emails with fresh content. After a year, my inbox was full. But what could I do with that?

---

## **Act III – From inbox to insight**

Here’s what I built:

- A **Google Script** running in Google Drive that reads my Gmail inbox.
    
- It looks for messages from Google Alerts.
    
- It extracts the **term**, the **link**, the **title**, and the **description**.
    
- It stores everything into a **Google Spreadsheet**.
    

One year of these terms gave me over **4,000 rows** of structured data — all content indexed by Google over a full year that used the words I care about.

From there, I decided to dive into just one of them: **bioart**.

What does the world mean when it says _bioart_?

And this is where the pipeline of Jupyter Notebooks began — layering techniques of data cleaning, scraping, language detection, metadata extraction, and semantic analysis using the OpenAI API.

---

## Act IV - _Semantic Filtering and Structured Intuition_

### Context

In this entry, I document the development of a semantic analysis pipeline that interfaces with Google Sheets and OpenAI’s language models. The dataset originates from Google Alerts collected around topics like **Bioart**, **Biodesign**, and **Biohacking** — and is filtered, deduplicated, and semantically processed using a sequence of Jupyter Notebooks written in Python.

This work is part of a broader system of creative knowledge curation and machine-assisted reasoning in the research framework **Creativity in Vitro**.

---

### What we built

We structured our workflow into **3 main notebooks**, each with a clearly defined purpose and stepwise logic:

---

#### `0-clean-duplicates.ipynb`

**Removes duplicate links** from a raw feed collected in Google Sheets.

- Reads all rows from `Sheet0`
    
- Removes duplicates based on the link (column B)
    
- Rewrites the sheet with only unique entries, maintaining original structure
    

---

#### `1-url-language-country-analyzer.ipynb`

**Fetches content from URLs and detects language + country metadata.**

- Filters rows where `wordAlert == "bioart"`
    
- Fetches the HTML content of each link using `requests + BeautifulSoup`
    
- Detects:
    
    - **Language** using `langdetect`
        
    - **Country** using meta tags (e.g., `geo.country`, `og:country-name`)
        
- Writes results to columns G–I (`language`, `country`, `text`)
    
- Avoids reprocessing already labeled or blocked entries
    
- Handles API quota limits via chunked writing (200 rows at a time)
    

---

#### `2-semantic-analysis-openai.ipynb`

**Performs semantic analysis using OpenAI's API**, focusing on meaningful clustering of ideas.

- Only processes rows with `wordAlert == "bioart"`
    
- Ignores rows where the `text` field is `"Blocked"`
    
- For each row, OpenAI returns a structured JSON with:
    
    - `"language"` → always in English
        
    - `"country"` → in English
        
    - `"summary"` → 1–2 sentence overview
        
    - `"semantics"` → high-level conceptual domains (e.g., "biofabrication", "critical design")
        
    - `"keywords"` → 5–10 tags, comma-separated
        
- Results are written to columns J–N in exact row alignment with `Sheet0`
    
- All `"Blocked"` rows are preserved with `"Blocked"` in all output fields
    

---

### Prompt evolution

The OpenAI prompt was iterated to ensure:

- Consistent output in English, regardless of source language
    
- Clear separation between `summary`, `semantics`, and `keywords`
    
- Structured JSON format for easy parsing and alignment with the spreadsheet

## Reflection

This system became a form of **structured intuition** — a scaffold to help make sense of a dispersed, multilingual, ungoverned field. It filtered raw alerts into patterns, clusters, and vocabularies that can now be explored, challenged, and shared.

What began as a year of passively collecting Google Alerts became an experiment in **semantic listening**.

Through the lenses of automation, scripting, and API-based reasoning, I wasn't just gathering data — I was asking a question over and over again:

> _When we say “bioart,” do we mean the same thing?_

This project doesn’t seek to fix the meaning of words, but to **trace how they’re used**, and to **build shared understanding** from there — a practice I often return to when facilitating co-creation across disciplines.

In the end, the spreadsheet became more than a database.  
It became a **living glossary**, a way to navigate a field-in-flux,  
and perhaps, a method to listen to the internet like it were a crowd —  
one whispering back hundreds of versions of the same word.

See the next post about VISUALIZATION!

If you're curious about the code and want to explore (or fork) the pipeline,  
you can visit the repository here:  
👉 [github.com/linalopes/bio-terms](https://github.com/linalopes/bio-terms)
