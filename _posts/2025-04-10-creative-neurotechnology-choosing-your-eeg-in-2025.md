---
layout: post
title: Creative Neurotechnology - Choosing Your EEG in 2025
id: 2025-04-10-creative-neurotechnology-choosing-your-eeg-in-2025.md
categories:
  - cabinet of curiosities
image: https://img.youtube.com/vi/nIyR9McTo_8/maxresdefault.jpg
share: "true"
comments: "true"
filename: creativity-in-vitro/_posts/2025-04-10-creative-neurotechnology-choosing-your-eeg-in-2025.md
tags: 
date: 2025-04-10
author: lina
---

<iframe width="100%" height="400" src="https://www.youtube.com/embed/nIyR9McTo_8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


## Introduction

To translate brain activity into visual art – a kind of “mind-to-image interface” – it's essential to use high-resolution EEG (electroencephalography) equipment.

In an artistic experimentation context, such equipment must capture detailed neural patterns and be integrated into machine learning systems to generate images (for instance, using generative models like Stable Diffusion).

This report presents the main EEG devices currently available on the market that are suitable for experimental and artistic projects, ranging from **open-source platforms** to professional commercial systems. Each device is evaluated based on key criteria such as **resolution** (number of channels and sampling rate), **portability**, **ease of use**, **integration with AI software**, and **technical support**.

## Criteria for Selecting EEG Equipment

Before listing the devices, it’s important to understand the criteria for choosing a suitable high-resolution EEG:

- **Number of channels:** Devices with **more channels** (e.g., 16, 32 or more) allow for recording electrical activity across multiple brain regions simultaneously, offering greater spatial resolution of neural patterns. To decode complex thoughts and imaginations, a higher channel count is desirable.

- **Sampling rate:** A **higher sampling rate** (e.g., 250 Hz, 500 Hz or more) ensures better temporal fidelity, capturing higher-frequency brain waves. Artistic BCI (brain-computer interface) projects typically benefit from at least ~250 Hz per channel, though professional systems can reach 500–1000 Hz.

- **Type of electrodes (dry vs. wet):** **Dry EEGs** use electrodes that don’t require gel (metal or conductive foam), making setup and cleanup easier, though they may introduce more noise or have reduced conductivity. **Wet EEGs** use gel or saline-based electrodes, offering better electrical contact and signal quality at the cost of longer preparation time. Some modern devices use **saline sponge electrodes** (wet but quick to set up) or hybrids that can function either dry or dampened.

- **Portability and usage context:** In an artistic residency, the ideal device should be **portable and easy to set up** – preferably **wireless** (data transmitted via Bluetooth or Wi-Fi) and battery-powered – allowing participants to move or perform in non-clinical environments. Compact, wireless gear is especially useful for live performances and installations.

- **Ease of use:** This includes headset ergonomics, prep time (placing electrodes, checking impedance), and software usability. For creative purposes, systems that **don’t require complex procedures** (e.g., spending hours placing 64 gel electrodes) are ideal. Fewer channels or dry electrodes usually mean faster setup, though this may come at the cost of data resolution.

- **Integration with software and AI:** The equipment should offer **easy access to raw EEG data**, ideally through libraries or SDKs compatible with languages like Python. Integration with frameworks like **BrainFlow** or BCI toolkits, and compatibility with machine learning environments (PyTorch, TensorFlow) are important. Ideally, the device supports real-time data streaming (e.g., via LSL – Lab Streaming Layer – or native APIs) to feed generative AI models. Open-source devices tend to integrate well with custom tools, while proprietary ones may require specific SDKs or licenses.

- **Price range:** Costs vary widely – from affordable open-source kits (a few hundred dollars) to professional medical-grade systems (tens of thousands). In an artistic context, it’s crucial to balance budget with technical needs. Mid-range devices (US$ **1–5k**) often provide sufficient quality without prohibitive costs.

- **Licensing and support:** **Open-source solutions** (like OpenBCI or DIY projects) offer transparency, active communities, and customization but may require more technical skill. **Commercial proprietary solutions** often come with **professional technical support**, warranties, and solid documentation, though some restrict features (e.g., access to raw data) to certain licenses. For experimental projects, clear documentation and access to support (community or company) are key to solving problems quickly.

With these criteria in mind, the following sections present the **recommended EEG equipment**, grouped by category: open-source/DIY platforms, mid-range commercial headsets, and high-density professional systems. For each, we highlight relevant specs and their suitability for the proposed project.
## 1. Open-Source and DIY Devices

This category includes EEG equipment with open hardware and software designs, or those aimed at makers, offering maximum flexibility. They're best suited for researchers and artists with technical familiarity, as they allow for modifications and direct integration with custom code.

- **[OpenBCI Cyton (8 or 16 channels)](https://shop.openbci.com/products/cyton-biosensing-board-8-channel?srsltid=AfmBOoqRQ5FiDSOAsi0iKfjD6-w_qtdiUUUg-fd7nIz_Npmwrlc93GKv#:~:text=PIC32MX250F128B%20microcontroller%2C%20giving%20it%20lots,each%20of%20the%20eight%20channels):**  
  The Cyton is a popular open-source biosensing board used in both art and research. The base board offers **8 EEG/EMG/ECG channels** with 24-bit resolution and **250 Hz per channel** sampling rate.  
  By adding the optional [Daisy module](https://shop.openbci.com/products/cyton-daisy-biosensing-boards-16-channel?srsltid=AfmBOoqODuEP2lDd12goGwaHPXanIGlDUScqYm2ocxDq7GfXHql3hNHH#:~:text=The%20OpenBCI%20Cyton%C2%A0Board%20and%20OpenBCI%C2%A0Daisy,each%20of%20its%2016%20channels), you can expand to **16 channels**, in which case the sampling rate becomes 125 Hz per channel.

  The Cyton is compatible with various electrode types – both passive (Ag/AgCl gel discs) and active – and can be used with accessories such as the **Ultracortex** headset (a 3D-printed headset supporting dry or semi-dry electrodes). It communicates wirelessly via USB dongle (BLE or similar) and runs on battery, making it very portable.

  This is a **research-validated device** (comparable to high-end medical systems) with a mature open-source ecosystem. It supports free data recording/visualization software and integrates seamlessly with [BrainFlow](https://brainflow.readthedocs.io/en/stable/) and libraries like OpenBCI Python and BCI Lab, making it ideal for real-time generative AI experiments.

  **Cost:** The 8-channel kit is around **US$999**, and the full 16-channel version is approximately **US$1,500**. Open-source hardware with strong documentation and community support make this one of the best entry points for artistic BCI projects.

- **OpenBCI [Ganglion (4 channels)](https://shop.openbci.com/products/ganglion-board):**  
  A lower-cost option from OpenBCI, the Ganglion board provides **4 channels** with a sampling rate of ~200 Hz. It uses snap or touch-proof electrodes. While it has lower resolution (12–16 bits) and fewer channels, it's highly portable and was launched at a price of around **US$199**.

  Though it may not provide enough spatial resolution for complex mental image reconstruction, it’s still a great open-source tool for basic signal prototyping, and it integrates with BrainFlow for easy data access and experimentation.

- **[FreeEEG32 (32-channel DIY)](https://www.crowdsupply.com/neuroidss/freeeeg32#:~:text=FreeEEG32%20is%20a%20stackable%2C%20open,to%20expensive%2C%20proprietary%20EEG%20technology):**  
  FreeEEG32 is an open-source board created as a low-cost alternative to proprietary high-density EEG systems. It features **32 channels** via four 8-channel ADCs (AD7771) with 24-bit resolution and simultaneous sampling, theoretically supporting up to **16,000 samples per second per channel** (though typical usage is 250–1000 Hz).

  It emphasizes signal quality (noise <0.22 µV) and features a powerful Cortex-M7 microcontroller for on-board processing. See more specs [here](https://www.crowdsupply.com/neuroidss/freeeeg32#:~:text=FreeEEG32%20combines%20four%208,acquisition%20and%20much%2C%20much%20more).

  Licensed under the AGPL, the project was launched via crowdfunding and remains one of the most advanced open EEG hardware designs to date. While it’s not a plug-and-play system (you’ll need to assemble or adapt it into a cap), it offers full integration with [BrainFlow](https://brainflow.readthedocs.io/en/stable/SupportedBoards.html#:~:text=FreeEEG%C2%B6), making it highly usable in Python-based ML pipelines.

  **Estimated cost:** **US$300–500**, depending on availability. It doesn't come with electrodes or a headset, so you’ll need to provide those. But for technically inclined artists, it’s one of the most powerful and flexible options available.

Other open-source or DIY EEG projects exist, such as the original **OpenEEG** (8 channels), but **OpenBCI** and **FreeEEG32** currently stand out due to their quality and community support. All these devices integrate excellently with custom software, and were designed for **creative and scientific experimentation beyond clinical settings**.

## 2. Mid-Range Commercial Headsets

This category includes **commercial portable EEG devices** aimed at enthusiasts and basic research. They typically offer 4 to 14 channels in easy-to-use formats (tiaras or wireless headsets), with ready-to-go software and SDKs. These are well-suited for artistic projects that prioritize **convenience and usability**, even if they sacrifice some resolution compared to 32+ channel systems.

- **[Emotiv EPOC X (14 channels)](https://www.emotiv.com/products/epoc-x?srsltid=AfmBOoqYPvvdEjmNPcN6tnfknE30LGzmhTiJNVhJuAJ_ZAvcvzw7XAT_#:~:text=%23%2014,20%20System):**  
  Emotiv is one of the pioneers in consumer-grade EEG and BCI tools for developers. The **EPOC X** is their latest model, featuring **14 EEG channels** positioned according to the 10–20 system (covering frontal, parietal, and temporal areas).  
  It uses felt sensors soaked in saline solution (_saline electrodes_) that must be moistened before use but are easier to clean than gel. These pads can be rehydrated during sessions.

  Battery life is around **9 hours**, and data is transmitted via **Bluetooth 5.0** to a USB receiver, offering freedom of movement. The device samples data at **128 Hz** (standard mode) or **256 Hz** (Pro mode). The effective resolution is 14 bits.

  To access raw EEG signals at 256 Hz, a research license (Emotiv PRO) is required. The headset is ergonomic, with adjustable bands and semi-dry electrodes that can be set up in minutes. Emotiv provides a multi-platform SDK (Python, C++, MATLAB, etc.), along with visualization and logging software.

  For AI integration, developers can use EmotivPRO to stream real-time data into Python. However, raw data access may require purchasing a license.

  **Price:** The hardware costs **US$999**, with optional license upgrades for full features.  
  In short, the EPOC X is a well-balanced solution: **14 channels, portable, and easy to use**, making it ideal for capturing general brainwave patterns (alpha waves, emotional states, etc.) and widely used in art and music projects. While 14 channels might not deliver the same detail as a 32-channel system, many interactive creations have been built with Emotiv — it’s arguably the most widespread “creative EEG” headset to date.

- **[Emotiv Insight (5 channels)](https://www.emotiv.com/products/insight):**  
  Another Emotiv product, the **Insight**, is a lightweight headset with **5 channels** (approximately AF*, T*, P* locations), fully dry, and designed for comfort (it resembles a sleek headband). It samples at 128 Hz and is marketed for wellness and entry-level research.  
  Due to its low channel count, it only provides limited information (e.g., attention, relaxation), and is less suited for generating inputs to image-based generative models.  
  We mention it here for completeness — in general, the EPOC X is recommended over the Insight unless **extreme ease and mobility** are prioritized and resolution can be sacrificed.

- **[Muse 2 / Muse S (4 channels)](https://eu.choosemuse.com/products/muse-2#:~:text=Muse%202%20%7C%20Muse%E2%84%A2%20EEG,CMS%2FDRL%29):**  
  The **Muse** family consists of minimal EEG headbands initially designed for meditation, but widely adopted by artists and developers thanks to their low cost and simplicity. The **Muse 2** and **Muse S** feature **4 EEG channels** (AF7, AF8 in front, TP9, TP10 behind the ears), plus auxiliary reference channels.

  They operate at **256 Hz** with 12-bit resolution and connect via Bluetooth to mobile devices or PCs (note: on PC, you need a special BLE adapter like the BLED112 dongle). The electrodes are dry (direct skin contact), and slightly moistening the skin improves conductivity.

  Muse is extremely **portable and discreet**, and can be worn in seconds. However, its **4-channel limit** restricts the amount of information captured: it's enough to detect general mental states (relaxation, attention) or simple patterns (blinks, frontal shifts), but not complex mental imagery.

  Nevertheless, Muse has been used in affordable BCI research. InteraXon provides an SDK, and the community has developed tools like _Muse LSL_ and integration with [BrainFlow](https://brainflow.readthedocs.io/en/stable/SupportedBoards.html#:~:text=Muse%C2%B6).  

  **Price:** About **US$250–300**, making it accessible for initial prototyping or installations with multiple participants. In a _“thought-to-image”_ project, Muse might work for exploratory stages or basic demos, but it likely lacks the spatial resolution needed to train a robust image reconstruction model.

- **[Neurosity Notion 2 / Crown (8 channels)](https://neurosity.co/tech-specs#:~:text=Brain%20Imaging):**  
  The **Neurosity Crown** (and its predecessor Notion) is a modern wearable EEG aimed at developers, known for combining onboard computing and web connectivity. It’s a headband with **8 dry active EEG sensors** positioned over central and parietal regions (~CP3, C3, F5, PO3, PO4, F6, C4, CP4) and two reference sensors on the sides (T7, T8).

  Sampling is done at **256 Hz** with low-noise circuitry (~0.25 µV RMS). A unique feature is its built-in quad-core processor that supports on-device computation and Wi-Fi/Bluetooth streaming.

  Neurosity focuses on applications like attention tracking (e.g., music playback based on concentration), but the Crown is general-purpose enough for broader BCI use.

  The company provides a flexible SDK and [API for JavaScript and Python](https://github.com/neurosity/neurosity-sdk-python#:~:text=GitHub%20github,250Hz%20means%20the%20data), and the device is supported by [BrainFlow](https://brainflow.readthedocs.io/en/stable/SupportedBoards.html#:~:text=Neurosity%C2%B6).

  This makes it relatively easy to access raw **8-channel EEG data** for feeding into AI models. The Crown is **comfortable and easy to wear**, fully dry, and has a battery life of about 3 hours.

  One potential downside is its reliance on a proprietary ecosystem — while the data is accessible, some functionality depends on cloud services and login-based APIs, which could introduce friction.  

  **Price:** Starting around **US$999**, sometimes with optional subscription services. For artistic purposes, the Crown offers a good middle ground: **8 well-placed dry channels**, great usability, and Python integration, allowing for fast experimentation. While it doesn’t match 32-channel systems, it might capture enough signals from key brain regions for user-specific imagination recognition, especially when paired with machine learning.

- **Other mid-range commercial devices:**  
  Several other companies offer EEG headsets for simplified BCI and research:

  - _BrainBit_: A 4-channel Russian-made headband, similar to Muse.  
  - _OpenBCI Galea_: A high-end headset combining EEG (10 dry channels), other sensors, and VR – very innovative, but still emerging and **extremely expensive** (~US$30k).  
  - _NeuroSky MindWave_: 1 dry channel, ultra-cheap – good only for educational intros, not complex applications.  
  - _Bitbrain Versatile_: Spanish startup offering 8–16 dry-channel systems focused on usability and applied research.  
  - _Wearable Sensing DSI-24_: A 24-channel dry EEG headset (derived from Cognionics) – more professional, discussed in the next section.

Devices in this category generally offer **developer documentation** and active user communities. Emotiv and Muse, in particular, are frequently used in artistic projects (neurofeedback installations, audiovisual performances reacting to EEG, etc.).

For a project aiming to translate thoughts into images, these headsets can be great for quickly building a functional prototype — accepting some loss in reconstruction precision. The next section will cover higher-resolution systems for those seeking maximum neural detail.

## 3. High-Density Professional EEG Systems

This category includes **professional/laboratory-grade EEG systems**, ranging from portable high-density options (up to 32 channels) to traditional clinical systems (64+ channels). These devices offer **the highest signal quality and resolution**, but they come with high costs and require more complex setup. They may be suitable for art-science collaborations involving access to a neuroscience lab or significant funding — especially when detailed neural data is needed to train more ambitious AI models.

- **[Emotiv EPOC Flex (32 channels)](https://www.emotiv.com/products/flex-saline?srsltid=AfmBOoob5Y6My-QduKidjeEmF2M1mH_KLUkkGmhkFV_6TciNJ9Sam0Yk#:~:text=):**  
  An extension of the Emotiv lineup, the **Flex** is a modular **32-channel** EEG system available in two versions: **saline** (felt pads) or **gel** (Ag/AgCl electrodes).  
  It uses a stretchable fabric cap with 74 possible electrode positions (choose 32) and a central controller unit that clips onto the top or back of the head. Data is transmitted **wirelessly** via Bluetooth Low Energy.

  Internally, it samples at 2048 Hz and down-samples to **256 Hz per channel** with 24-bit resolution. It includes CMS/DRL references and a built-in IMU sensor (motion tracking).

  In terms of **signal quality**, the Flex offers **better spatial coverage** than the EPOC X. The saline version uses moist felt pads (faster to set up, but may need rehydration after ~1 hour), while the gel version requires gel application but offers the **highest conductivity**.

  **Setup time:** Emotiv estimates 20–30 minutes for 32 electrodes with gel, or slightly less with saline — still much faster than conventional clinical systems.

  For integration, access to raw EEG data requires the Emotiv PRO license, but once unlocked, you can use the same SDK as the EPOC.

  **Use case:** Researchers already use the Flex for mobile EEG studies. Emotiv even provides an e-book with example applications in field research.

  **Price:** A full Flex kit ranges from **US$2,500–5,000**, depending on electrode type and licensing. This makes it a compelling **“affordable high-density”** option, compared to medical systems that may cost 3–5x more. For artistic AI-driven projects, the Flex offers **32 wireless channels** — ideal for training models to recognize visual imagination features, assuming one can manage the operational complexity and software licensing.

- **g.tec g.Nautilus PRO (32/64 channels):**  
  Austrian company g.tec produces high-end EEG systems used in BCI and neuroscience research. The **g.Nautilus** is their wireless wearable line, available in **32 or 64-channel** configurations.

  It features a rigid adjustable band with built-in electrodes — available in **dry “g.Sahara”** or traditional **wet** versions. Although wearable, it is **medical-grade**, transmitting data wirelessly via a proprietary radio protocol at **500 Hz per channel**, 24-bit resolution.

  Notable for its **signal quality and stability**, the 32-channel version can be mounted relatively quickly, especially with dry pressure electrodes. These sensors are designed to gently press through hair and contact the scalp, avoiding the need for gel.

  A gel-based cap alternative offers even better signal but takes more prep time. The Nautilus also includes motion sensors and can integrate fNIRS modules in hybrid versions.

  **Cost and access:** It’s a **premium system**, typically purchased by labs. The 32-channel version often exceeds **US$30,000**, depending on the configuration. g.tec provides full software suites (e.g., g.HIamp) and APIs in MATLAB/C++, with possible LSL compatibility via products like Unicorn.

  **Artistic usage:** Best accessed through a **partnership with a lab** or equipment loan. If available, it delivers **top-quality wireless EEG data**, suitable for decoding subtle mental signals across the cortex — ideal for training sophisticated generative AI.  

  Summary: g.Nautilus is a **state-of-the-art wearable EEG**, but unless institutional support is in place, it's more of a reference point than a practical option for short-term art residencies.

- **[Neuroelectrics Enobio 32 (32 channels)](https://www.neuroelectrics.com/products/research/enobio/enobio-32#:~:text=Enobio%2032%20allows%20for%20easy,based%20electrodes):**  
  A portable high-density option from Spanish company Neuroelectrics. The **Enobio 32** connects via Wi-Fi and records **32 channels at 500 Hz**, 24-bit resolution.

  Designed for ease of use: setup with **dry electrodes takes ~4 minutes**, and gel/hybrid options take ~20 minutes for higher signal quality.

  It uses a fabric EEG cap with electrode ports and a small electronic module for data transmission. The Enobio runs on battery and includes internal data storage.

  Interface-wise, it comes with **NIC2 software** for setup, visualization, and data export, and integrates easily with LSL. It’s FDA-cleared for medical use, and is also used in VR/BCI experiments and “at-home EEG” studies.

  **Support:** Includes detailed manuals and professional customer service. Used in innovative art-science projects for its balance of quality and portability.

  **Price:** Also in the **tens of thousands of dollars**, though Neuroelectrics offers academic partnerships and rental options. If available, it provides **32 rich EEG channels** with flexible electrode options — perfect for mental image reconstruction through AI.

- **Brain Products LiveAmp (32 channels):**  
  German company Brain Products offers the **LiveAmp**, a portable **32-channel** amplifier (expandable to 64). It’s worn on the body and connects to an EEG cap via ultrathin wires.  
  It streams via Bluetooth at up to **1000 Hz**, with simultaneous SD card recording. It uses gel electrodes and delivers research-quality data.

  Although it uses Bluetooth, it achieves high rates when configured properly. With 32 channels, it supports all typical EEG paradigms (SSVEP, P300, etc.) and is well-suited for AI integration. Setup requires 15–30 minutes with gel.  
  It’s supported via the **ActiChamp SDK** and LSL compatibility.

  **Price:** Around **US$20,000**.

- **Clinical systems (64+ channels):**  
  At the top end are medical/research EEGs like those from **Compumedics Neuroscan** and **BioSemi**.  
  For example, the _Neuroscan SynAmps_ or _BioSemi ActiveTwo_ offer **64, 128, or 256 channels**, with up to 2 kHz sampling and full scalp coverage (some even record ultra-high frequencies).

  These systems use **wet gel caps** or high-density sponge arrays. They are not wireless — users are tethered by cables — making them impractical for live or interactive artworks.  
  However, they are the **gold standard in EEG signal quality**.

  **Use in art:** Requires direct lab collaboration, technician assistance, and significant investment (e.g., a 64-channel BioSemi can exceed **US$100k**).  
  Still, some performances have been done in labs using these systems to generate sound or visuals from brain waves.

  They provide SDKs and software (e.g., Scan 4.5 for Neuroscan, MATLAB interfaces for BioSemi), allowing data to be routed into AI pipelines via middleware.

  **Summary:** These systems capture **the richest brain data possible**, but they’re **logistically unfeasible** for most artistic residencies. Their best role is in generating high-quality training datasets for use later with more mobile devices.

## Comparison of Selected EEG Equipment

The following table summarizes the key specifications of some of the EEG devices discussed, comparing them based on the main selection criteria (channels, sampling rate, electrodes, etc.), and includes links for further information or purchase where applicable.


| **Equipment**                     | **Channels**         | **Sampling Rate**                                                                                                                  | **Electrodes**                                                                                                               | **Ease of Use**                             | **Software Integration**                                                                                                                            | **Approx. Price**                                                                                                                        | **License/Support**                           | **Link**                                                                               |
| --------------------------------- | -------------------- | ---------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------- | -------------------------------------------------------------------------------------- |
| **OpenBCI Cyton** (8ch / 16ch)    | 8 (expandable to 16) | 250 Hz (8ch) / 125 Hz (16ch)<br><br>[shop.openbci.com](https://shop.openbci.com/products/cyton-daisy-biosensing-boards-16-channel) | Passive or Active (gel or dry)<br><br>[shop.openbci.com](https://shop.openbci.com/products/cyton-biosensing-board-8-channel) | Moderate (manual setup; optional headset)   | Excellent – Open-source, compatible with BrainFlow                                                                                                  | US$ 999 (8ch kit)<br><br>~ US$ 1.5k (16ch)<br><br>[shop.openbci.com](https://shop.openbci.com/products/cyton-biosensing-board-8-channel) | Open-source (HW & SW); active community       | [shop.openbci.com](https://shop.openbci.com/products/cyton-biosensing-board-8-channel) |
| **FreeEEG32** (DIY open-source)   | 32                   | Typically 256–1000 Hz (up to 16 kHz max)<br><br>[crowdsupply.com](https://www.crowdsupply.com/neuroidss/freeeeg32)                 | Passive – requires EEG cap/gel                                                                                               | Low (DIY kit; needs assembly and expertise) | Excellent – Open-source, supported via BrainFlow<br><br>[brainflow.readthedocs.io](https://brainflow.readthedocs.io/en/stable/SupportedBoards.html) | ~US$ 300–500 (est.)                                                                                                                      | Open-source (AGPL); community-supported       | [crowdsupply.com](https://www.crowdsupply.com/neuroidss/freeeeg32)                     |
| **Emotiv EPOC X** (14ch)          | 14                   | 128 Hz (standard) or 256 Hz (Pro)<br><br>[emotiv.com](https://www.emotiv.com/products/epoc-x)                                      | Saline electrodes (moistened felt)<br><br>[emotiv.com](https://www.emotiv.com/products/epoc-x)                               | High (wireless headset; quick setup)        | Good – Proprietary SDK (requires license for raw data)                                                                                              | US$ 999<br><br>+ (Pro license)<br><br>[emotiv.com](https://www.emotiv.com/products/epoc-x)                                               | Proprietary; support via Emotiv (docs, forum) | [emotiv.com](https://www.emotiv.com/products/epoc-x)                                   |
| **Emotiv Flex** (32ch saline/gel) | Up to 32             | 256 Hz (downsampled from 2048 Hz)<br><br>[emotiv.com](https://www.emotiv.com/products/flex-saline)                                 | Saline (sponges) or Gel (Ag/AgCl)<br><br>[emotiv.com](https://www.emotiv.com/products/flex-gel)                              | Medium (32ch cap; ~20 min setup)            | Good – Emotiv SDK (Pro license required for raw data)<br><br>[emotiv.com](https://www.emotiv.com/products/flex-saline)                              | ~US$ 3–5k (incl. license)                                                                                                                | Proprietary; Emotiv Pro support               | [emotiv.com](https://www.emotiv.com/products/flex-saline)                              |
| **Muse 2 / S** (4ch)              | 4 (+2 aux)           | 256 Hz<br><br>[eu.choosemuse.com](https://eu.choosemuse.com/products/muse-2)                                                       | Dry (direct skin contact)                                                                                                    | Very High (plug-and-play headband)          | Good – Open SDK; BrainFlow supported<br><br>[brainflow.readthedocs.io](https://brainflow.readthedocs.io/en/stable/SupportedBoards.html)             | US$ 250–400                                                                                                                              | Proprietary; strong dev support               | [eu.choosemuse.com](https://eu.choosemuse.com/products/muse-2)                         |
|**Neurosity Crown** (8ch)|8|256 Hz<br><br>[neurosity.co](https://neurosity.co/tech-specs#:~:text=Ultra,uVrms)|Dry active (flexible Ag/AgCl)<br><br>[neurosity.co](https://neurosity.co/tech-specs#:~:text=Passive%20%2B%20active%20sensors)|Very High (band-style; no prep; ~3h battery)|Very Good – Native SDK + BrainFlow<br><br>[brainflow.readthedocs.io](https://brainflow.readthedocs.io/en/stable/SupportedBoards.html)|~US$ 999|Proprietary; dev support (cloud + SDK)|[neurosity.co](https://neurosity.co/tech-specs#:~:text=Sensors)|
|**g.tec Unicorn** (8ch)|8|250 Hz, 24-bit<br><br>[unicorn-bi.com](https://www.unicorn-bi.com/#:~:text=match%20at%20L210%20Advanced%20EEG,and%20250%20Hz%20per%20channel)|Hybrid dry (can use gel)|High (ready-to-use headset)|Good – Dedicated SDK; BrainFlow compatible<br><br>[brainflow.readthedocs.io](https://brainflow.readthedocs.io/en/stable/SupportedBoards.html)|~€4–5k|Proprietary; g.tec support|[unicorn-bi.com](https://www.unicorn-bi.com/#:~:text=match%20at%20L210%20Advanced%20EEG,and%20250%20Hz%20per%20channel)|
|**Neuroelectrics Enobio 32** (32ch)|32|500 Hz, 24-bit<br><br>[pubcompare.ai](https://www.pubcompare.ai/product/eyriCZIBPBHhf-iFRhaL/#:~:text=User,in%20a%20normal%20office%20setting)|Dry or Hybrid gel<br><br>[neuroelectrics.com](https://www.neuroelectrics.com/products/research/enobio/enobio-32)|Medium (4–20 min setup depending on electrodes)|Very Good – NIC software + LSL; SDK available<br><br>[pubcompare.ai](https://www.pubcompare.ai/product/eyriCZIBPBHhf-iFRhaL/#:~:text=User,in%20a%20normal%20office%20setting)|~€20–30k|Proprietary; professional support|[neuroelectrics.com](https://www.neuroelectrics.com/products/research/enobio/enobio-32)|
|**g.tec g.Nautilus** (32–64ch)|32 / 64|500 Hz (typical)|Dry special or Gel|Medium-Low (professional-grade system)|Good – APIs (MATLAB, LSL); g.tec support|>US$ 30k|Proprietary; professional support|_(See manufacturer)_|
|**Neuroscan / BioSemi** (64+ch)|64 to 256|1 kHz or more|Gel (wet cap)|Low (slow setup; not portable)|Varies – Dedicated software (MATLAB, EEGLAB)|>US$ 50k|Proprietary; professional support|_(See manufacturer)_|

**Legend:**  
_Ease of use_ is evaluated qualitatively (considering setup time, ergonomics, and portability).  _Integration_ refers to the availability of SDKs or compatibility with open-source frameworks (BrainFlow, LSL, etc.).  Prices are approximate and may vary depending on region and support packages.


## Final Considerations

For a project aiming to translate thoughts into images, choosing the right EEG device involves balancing **data resolution** with **artistic practicality**.

**Open-source devices like OpenBCI Cyton** stand out by offering a flexible platform, relatively affordable and well-integrated with AI tools — an excellent choice for prototyping and creative experimentation.

**Commercial headsets like the Emotiv EPOC X**, on the other hand, offer ease of use and a ready-to-go design, which can accelerate the initial phases of the project — especially when the goal is to quickly get an artist up and running with the device to generate visual material.  

If the goal is to extract the maximum detail from brain patterns (for example, distinguishing very specific imagined concepts or reconstructing complex mental images), then investing in **32-channel or higher** systems — such as the Emotiv Flex or a research-grade EEG cap — may be necessary. But this also requires more time, money, and potentially technical assistance.

A critical point is ensuring **real-time access to EEG data** and connecting it to machine learning models. All the listed devices support this, but with varying levels of effort:

- With open-source devices like OpenBCI, you can stream data directly (via BrainFlow, LSL, or APIs) into your Python code (e.g., with PyTorch) and start training models right away.
- With proprietary devices like Emotiv, you’ll need to use their official SDKs (sometimes with additional license costs) to access raw signals and integrate them into your AI pipeline.

In artistic contexts, where improvisation and fast experimentation are key, the **quality of documentation and support** makes a big difference. In that regard, OpenBCI and Emotiv offer plenty of resources geared toward creative users, while companies like g.tec and Neuroelectrics provide more traditional (yet solid) professional support — especially useful when there’s a tech team involved.

To conclude, **there is no single “best” EEG device**, but rather the one that best fits your project conditions:

- If **portability and budget** are crucial, and moderate resolution is acceptable, then options like the **Emotiv EPOC X** or a **Cyton 8ch kit** with a wearable headband can do the job.

- If you want to **maximize channels without sacrificing mobility**, the **Emotiv Flex 32** or an open-source solution like **OpenBCI with Daisy module** or **FreeEEG32** in a cap can provide richer data — giving your mind-to-image interface more information to work with (at the cost of added complexity).

- If you're working in an artistic residency with access to a neuroscience lab, leveraging a **professional high-density EEG system** (32+ channels from g.tec, Neuroelectrics, etc.) could raise the ceiling on what brain signals can reveal — potentially improving AI outcomes.  
  However, even with the best equipment, decoding imagination is an enormous challenge that demands multiple layers of signal processing and model training.

In short, this report mapped out the most relevant EEG equipment options for turning brain activity into visual art. Based on this overview, you can evaluate which tools align best with the practical needs and creative ambitions of the "Creativity In Vitro" project.

Each device has its strengths and trade-offs — but all of them bring us closer to the dream of **materializing imagination directly from neural signals**, merging technology and art in a truly interdisciplinary pursuit.


## Others Not Included in the Main Survey — But Thank You Anyway

- **X.on EEG Headset**:  
  Developed by Brain Products, the **X.on** is a wireless EEG headset that combines ease of use with high-quality signal acquisition. It uses saline-based sponge electrodes and comes with companion apps for Android™ and Windows®, allowing fast access to brain signals. It’s also compatible with the PEER app for iOS devices, making it suitable for capturing Event-Related Potentials (ERPs).  
  [Accueil + MindTec Store](https://www.bionic-france.fr/BrainProducts?utm_source=chatgpt.com)  
  [Flyer PDF – MindTec Store](https://www.mindtecstore.com/mediafiles/Sonstiges/Shop/X.on/Brain%20Products-_Flyer_Xon_EN.pdf?srsltid=AfmBOoqfoMYtYvz5exYe1Vg8B5YF6r3Gcv7WTexsCa_iq5yHCVV8whpP&utm_source=chatgpt.com)

- **NeuroTechX**:  
  While not a hardware manufacturer, **NeuroTechX** is a nonprofit organization that supports the advancement of neurotechnology worldwide. They offer educational resources, networking opportunities, and support for neurotech-related projects. If you're seeking community or learning materials in the field, NeuroTechX is a great place to start.

- **BioSemi ActiveTwo**:  
  A high-end EEG system widely used in academic research, the **ActiveTwo** supports up to **256 recording channels**, with **24-bit resolution per channel**, and full DC operation with a wide input range. It’s suitable for EEG, ECG, and EMG recordings.  
  [BioSemi Official Site](https://www.biosemi.com/products.htm?utm_source=chatgpt.com)

