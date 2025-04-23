---
layout: post
title: Artworks Where Brainwaves Speak in Light, Sound and Fabric
id: 2025-04-12-artworks-where-brainwaves-speak-in-light-sound-and-fabric.md
categories:
  - cabinet of curiosities
  - artistic pathology reports
image: https://laurajade.com.au/wp-content/uploads/RED-e1465135775510.jpg
share: "true"
comments: "true"
filename: creativity-in-vitro/_posts/2025-04-12-artworks-where-brainwaves-speak-in-light-sound-and-fabric.md
tags:
  - openBCI
  - emotiv
  - sensors
date: 2025-04-12
author: lina
---

## Intro

A generation of artists has turned their nervous systems into instruments. Since the late 2000s, the democratization of EEG technology — from Emotiv’s sleek neural helmets to OpenBCI’s open-source cranial rigs — has opened the skull not to surgery, but to sculpture, performance, and code.

What follows is a timeline of artistic experiments where brainwaves leave the laboratory and enter the realm of light, sound, and fabric. From stitched thought patterns and immersive opera to neural VR and machine-generated memory ghosts, each project in this archive employs EEG (particularly Emotiv, including its 32-channel model, and OpenBCI) to translate electric whispers of the mind into aesthetic events.

Some use machine learning. Others rely on raw signal mappings. All invite us to ask:  

> _What happens when thought becomes artifact?_

## Timeline of Brainwave-Based Artworks

### 2013–2015 — Brainwriter

**Artists/Collaborators:** Tempt One (Tony Quan), Daniel R. Goodwin, OpenBCI, Not Impossible Labs, Graffiti Research Lab (Zach Lieberman, Theo Watson, James Powderly)  (California, London)
**Device:** Custom OpenBCI-based EEG headset with Olimex active electrodes and Tobii eye-tracking  
**Medium:** Digital graffiti and interactive installations  
**Notes:** An open-source brain-computer interface enabling a paralyzed graffiti artist to create art using brainwaves and eye movements.​

**Description**  
Brainwriter is an open-source project developed to assist Tempt One, a graffiti artist paralyzed by ALS, in creating art again. By integrating a custom EEG headset (built with OpenBCI and Olimex electrodes) and Tobii eye-tracking technology, the system translates brain signals and eye movements into digital drawings. The software, developed using OpenFrameworks, allows for point-by-point sketching, line bending, and interaction with real-world images, enabling Tempt One to produce intricate digital graffiti. The project also featured an interactive installation at the Barbican Centre in London, where participants used their brainwaves and eye movements to control a game, demonstrating the potential of brain-computer interfaces in art and communication. This initiative builds upon the earlier Eyewriter Project and emphasizes the power of open-source collaboration in assistive technology.​[Daniel R Goodwin](https://danielrgoodwin.com/open-source-eeg?utm_source=chatgpt.com). (There was no explicit use of machine learning; the project relied on signal processing and direct mappings from EEG and eye-tracking data to visual output.)

---
### 2013 — NeuroKnitting

**Artists:** Varvara Guljajeva & Mar Canet (Barcelona)  
**Device:** Emotiv EPOC (14 channels)  
**Medium:** Knitted textiles from EEG patterns  
**Notes:** A scarf woven from the electrical activity of the brain.

**Description**  
A project that transformed brain signals into knitwear. The artists captured the brain activity of participants listening to classical music (Bach) and converted this data into a knitted scarf pattern. Using a 14-channel EEG headset, the system measured three aspects of mental state—relaxation, excitement, and cognitive load—and after 10 minutes of listening, translated each second of brainwave data into stitch patterns [var-mar.info](https://var-mar.info/neuroknitting/#:~:text=of%20the%20signal%20coming%20from,by%20the%20act%20of%20listening). The result was a series of unique scarves generated from each listener’s neural activity, creating a personal piece of generative EEG art [designboom.com](https://www.designboom.com/technology/neuroknitting-scarves-made-from-brainwaves/#:~:text=brainwaves%20into%20physical%20garments,lengths%20into%20a%20unique%20pattern). (There was no explicit use of machine learning; the project relied on direct mappings from Emotiv metrics to visual patterns.)

![](https://var-mar.info/wp-content/uploads/2013/06/8956690639_f7c36fb929_k.jpg)

---

### 2015 — Brainlight  
**Artist:** Laura Jade (Sydney)  
**Device:** Emotiv EPOC / EPOC+  
**Medium:** Illuminated brain sculpture  
**Notes:** Real-time light and sound feedback based on emotional EEG data.

**Description**  
An interactive sculpture shaped like a brain that lights up and emits sounds in response to the brain activity of the participant. Created as part of a Master’s project, the work features a large acrylic brain structure lit from within by LEDs. The installation is controlled by an Emotiv EEG headset, such that the sculpture glows according to changes in the user’s brainwaves captured wirelessly [laurajade.com.au](https://laurajade.com.au/interactive-brain-light-research-project/#:~:text=,electroencephalography%29%20wireless%20headset). The software monitors specific brainwave bands—such as alpha (meditation), theta (focus), and beta (excitement)—as well as detected emotional states and facial expressions, translating these into light and sound variations within the sculpture [laurajade.com.au](https://laurajade.com.au/interactive-brain-light-research-project/#:~:text=activity%20of%20the%20brain,light%20display%20within%20the%20brain). Through this setup, the audience experiences a kind of cyber-activation of the brain, where thoughts and emotions control the artwork in real time. (There was no indication of ML use; the project employed Emotiv’s emotional detection suite and direct mappings to audio-visual feedback.)



![](https://laurajade.com.au/wp-content/uploads/RED-e1465135775510.jpg)

---

### 2016 — Noor: A Brain Opera  
**Artist:** Ellen Pearlman (Hong Kong)  
**Device:** Emotiv EPOC+  
**Medium:** Immersive performance opera  
**Notes:** The performer’s emotional EEG states triggered visuals, sound, and text.

**Description**  
Immersive performance described as the **world’s first “brain opera.”** In _Noor_, a performer positioned at the center of a 360° theater controls every element of a multimedia opera — panoramic videos, soundscapes, and even fragments of the libretto — using only her brain activity. The premiere took place at the ISEA 2016 festival in Hong Kong. **Using the Emotiv EPOC+ headset**, the **performer's emotional states trigger segments of video, audio, and text** throughout the performance, while her brainwaves are displayed in real time for the audience [emotiv.com](https://www.emotiv.com/blogs/news/noor-brain-opera-ellen-pearlman?srsltid=AfmBOooRLdKrUtbiWLzZ3meMRDgvgfzzNy0bxhMFyVij3HzMjBW90lie#:~:text=Noor%20is%20a%20fully%20immersive,time%20for%20audience%20viewing.%20Artist). For example, levels of excitement or meditation detected by the EEG can trigger specific scenes or changes in the music. _Noor_ thus explores the intersection of BCI and performing arts, where **the artist’s mind becomes the interface that drives the narrative**. _(The piece used Emotiv’s emotional suite to map emotions to stage events, but did not involve a custom-trained ML algorithm.)_


--- 

### 2016 — Dual Brains

**Artists:** Eva Lee & Aaron Trocola (New York City)  
**Device:** OpenBCI (custom Ultracortex headset)  
**Medium:** Audiovisual performance  
**Notes:** EEG and ECG data from two performers generated synchronized visuals and sound in real time.

**Description**  
Three-minute audiovisual performance featuring **two performers connected through EEG**. Presented at Art-a-Hack 2016 in New York City, _Dual Brains_ featured artists Eva Lee and Aaron Trocola wearing OpenBCI headsets simultaneously to generate sound and visuals in real time. The installation captured both EEG (brainwaves) and ECG (heartbeats), translating this biodata into projected visuals and soundscapes. The result was a **shared audiovisual environment created by their merged neural and cardiac signals** [evaleestudio.com](https://www.evaleestudio.com/whats-new/dual-brains-art-a-hack-performance-goes-live-in-3-2-1/#:~:text=Image%3A%20Art,based%20on%20EEG%20and%20ECG%C2%A0data). Over the course of the performance, brainwave patterns and heart rhythms between the two participants began to synchronize, influencing the aesthetic output — an artistic exploration of **empathic connection and biofeedback between two brains**. _(No machine learning was used; the project relied on real-time integration of filtered EEG and ECG signals.)_

![](https://www.evaleestudio.com/wp-content/uploads/2016/07/Capture_frThoughtworksVideo-5.jpg)

---

### 2016 — _Agnosis: The Lost Memories…_

**Artist:** Fito Segrera (Paris)  
**Device:** OpenBCI (open-source EEG headset)  
**Medium:** Interactive installation  
**Notes:** Drops in attention, measured via EEG, triggered AI-generated memory reconstructions.

**Description**  
Interactive installation that explores memory loss through EEG and artificial intelligence. Colombian artist Fito Segrera developed a system in which an **OpenBCI headset monitors his level of attention — and when attention drops, the system intervenes** [makery.info](https://www.makery.info/en/2016/10/20/linstallation-anti-trou-de-memoire-de-fito-segrera/#:~:text=Colombian%20artist%20Fito%20Segrera%20created,accesses%20data%20generated%20by%20brainwaves). During these lapses, a camera captures a photo of the surrounding environment. In parallel, **image recognition algorithms, online tagging services, and Google's auto-suggestion** interpret both the EEG signals and the images taken, in order to **generate new, associative visual content**, which is compiled into a kind of visual "logbook" [makery.info](https://www.makery.info/en/2016/10/20/linstallation-anti-trou-de-memoire-de-fito-segrera/#:~:text=To%20reconstitute%20his%20lost%20memories%2C,In).

The piece, titled _Agnosis: The Lost Memories…_, presents viewers with a mosaic of true and false memories — real photographs juxtaposed with _fabricated_ images constructed by algorithms based on the artist’s brain activity. In essence, it is a form of **auto-generated augmented reality** that questions how attention and technology shape memory. _(Machine learning is central to the work: computer vision algorithms interpret EEG data indirectly and autonomously to produce new visual content, making AI not just a tool, but a co-creator in the artwork.)_

---

### 2018 — Emotiv VR (_Freud’s Last Hypnosis_)

**Artists/Project:** LS2N & ESBA-TALM, in collaboration with filmmaker Marie-Laure Cazin (Angers/Nantes, France)  
**Device:** Emotiv EPOC (14 channels)  
**Medium:** Neuro-interactive virtual reality film  
**Notes:** EEG-based emotional and cognitive states determined which point of view the viewer experienced within the film.

**Description**  
A **neuro-interactive VR film experience** that merges immersive cinema with brain-computer interfaces to alter narrative perspective in real time. Developed by a French research group (LS2N) in collaboration with the School of Fine Arts of Tours/Angers/Le Mans (ESBA-TALM) and filmmaker Marie-Laure Cazin, the project places the viewer inside a 360° cinematic reenactment of _Freud’s Last Hypnosis_. While immersed in the scene, the viewer wears an Emotiv EPOC headset, enabling them to **“embody” either Freud’s or the patient’s point of view**, based on their mental state [emotiv.com](https://www.emotiv.com/blogs/press/research-project-emotive-vr?srsltid=AfmBOorq7RLEduhtR92BW0qY24xmBM0Eb6HEm_CtQnKSW6vg1NCHLjTp#:~:text=By%20LS2N%20and%20The%20Ecole,their%20emotional%20and%20cognitive%20journey).

The EPOC’s EEG sensors **capture emotional and cognitive responses in real time**, enabling implicit interaction — for instance, levels of engagement or relaxation may influence which storyline branch the viewer is shown. The piece debuted at international events in 2018 (including ACM TVX in Seoul) and was later presented publicly at festivals in 2019.  
_(The project employs EEG-based state analysis to dynamically guide the viewer’s path, likely using Emotiv’s built-in emotional metrics rather than a custom-trained machine learning model.)_

---

### 2021 — Somatic Cognition Immersive Installation

**Artist/Collective:** Ashley Middleton (amiddletonprojects) and team (Berlin/London)  
**Device:** OpenBCI (supported by OpenBCI)  
**Medium:** Immersive installation  
**Notes:** EEG data linked to a virtual body system using real-time machine learning.

**Description**  
Immersive installation combining EEG signals with a virtual body system to explore somatic surveillance and non-conscious cognition. Developed during a residency at Exposed Arts Projects (London, 2020–2021) and presented in _EDGE Neuroart_ workshops in Berlin, the piece offered participants a **meditative, embodied experience within a “virtual sensory system of the body”** [openbci.com](https://openbci.com/community/immersive-eeg-art-cognition-middleton/#:~:text=For%20the%20past%20year%20I,sensing%20system).

The team used an OpenBCI headset to **capture EEG data and close it in a sensory feedback loop** — mapping it in real time to a virtual environment built in _TouchDesigner_. The technical system integrated platforms such as Python, BrainFlow, and the **Wekinator (an interactive machine learning toolkit)** to train real-time mappings between brain activity and aesthetic output [openbci.com](https://openbci.com/community/immersive-eeg-art-cognition-middleton/#:~:text=With%20support%20from%20the%20OpenBCI,technical%20framework%20of%20the%20installation). The first exhibition was planned for September 2021 in London, demonstrating how **AI techniques can translate non-conscious brain signals into artistic experience**.  
_(Machine learning plays a key role: Wekinator was used to train models that connect EEG data to visual and sonic parameters, enabling adaptive interaction.)_

---

### 2024 — The Echo Wave Project

**Authors:** Digital Media students, Toronto Metropolitan University (Mike Faragalla et al.)  
**Device:** Emotiv Insight (5-channel EEG)  
**Medium:** Interactive installation  
**Notes:** Real-time visualization of emotional states using EEG and TouchDesigner.

**Description**  
Interactive art installation focused on **visualizing mental health through brainwave data**. Presented at the _Future Makers_ exhibition in Toronto, _Echo Wave_ invited participants to wear an Emotiv Insight headset and **see their emotional states unfold in real time**. The system extracted EEG-based indicators like relaxation, stress, and excitement from the Emotiv headset [derivative.ca](https://derivative.ca/community-post/echo-wave-project-visualizing-mental-health-touchdesigner/70734#:~:text=Using%20the%20Emotiv%20INSIGHT%20EEG,brainwave%20patterns%20change%2C%20viewers%20visualize), and mapped them through a _TouchDesigner_ visual pipeline.

As the participant’s mental state shifted, **projected particles and abstract shapes changed dynamically**, following a therapeutic color palette (green for calm, blue for focus, red for tension) [derivative.ca](https://derivative.ca/community-post/echo-wave-project-visualizing-mental-health-touchdesigner/70734#:~:text=The%20Echo%20Wave%20Project%20invites,making%20invisible%20mental%20experiences%20tangible). This visual language allowed users to **literally see their brainwaves materialize as abstract art**, making often-invisible internal states visible. The result is a poetic and educational exploration of mental nuance, showing how **accessible interactive EEG art has become in 2024**.  
_(No trained ML models were used; the project relied on Emotiv’s emotional metrics and focused on immediacy and accessibility.)_


