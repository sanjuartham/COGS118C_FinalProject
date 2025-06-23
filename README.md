# Exploring the Impact of Emotions on Frequency Spectra in Speech  
*COGS118C Final Project – UC San Diego*

## Project Overview
This project explores how different emotions—Anger, Disgust, Fear, Happiness, and Sadness—affect the **frequency spectrum of speech**. Using short-time Fourier transform (STFT), we analyzed dominant frequency peaks in emotional speech recordings to identify spectral differences and statistically test distinctions between positive and negative emotional tones.

---

## Motivation
When people speak, their emotions are reflected in subtle frequency and pitch shifts. Understanding these patterns helps advance:
- **Emotion-aware AI voice assistants** (e.g., Siri, Alexa)
- **Speech-to-text systems** that adapt to speaker emotion
- **Cognitive neuroscience research** into affective expression

We asked:
- How do emotions affect speech frequency?
- Which frequency peaks dominate for each emotional category?
- Are there measurable differences between positive and negative emotions?

---

## Dataset
- **Source:** Acted Emotional Speech Dynamic Database (AESDD)
- **Format:** `.wav` audio files recorded in **Modern Greek**
- **Emotions:** Anger, Disgust, Fear, Happiness, Sadness
- **Samples:** 598 total, evenly distributed across emotions
- **Speakers:** 6 consistent voice actors, controlling for speaker variability

---

## Methods Summary

- Performed **STFT** on each audio file to transform time-domain speech to frequency domain  
- Focused on **median frequency magnitude** to reduce the influence of outliers  
- Used **Gaussian curve fitting** to extract top 3 dominant peaks in each sample  
- Conducted **independent t-tests** comparing **Happiness (positive)** vs **Sadness (negative)**

---

## Key Results
- Sadness = lower, more stable peak frequencies
- Happiness and Disgust = higher, more varied peak frequencies
- Disgust showed greatest variability in mid-range frequencies
- All 3 dominant peaks showed **statistically significant differences** (p < 0.05) between positive and negative emotions

---

## Team
- **Daniel Kong** – Signal processing, STFT interpretation, graph synthesis  
- **Momei Fang** – Curve fitting, frequency peak detection, statistical analysis  
- **Leah Seseri** – Dataset preparation, preprocessing code, result synthesis  
- **Sanjuktha Artham** – Slide design, presentation scripting, research framing, and proposal development

---

## 👩‍💻 My Role
I collaborated on multiple aspects of this project, including:

- **Co-authoring the research proposal** and outlining our project goals and motivation  
- **Designing and scripting the final presentation slides**, and helping communicate technical findings clearly  
- **Supporting statistical analysis and interpretation**, including t-test setup and frequency comparison logic  
- **Reviewing and refining code**, with a focus on understanding the results and connecting them to our research questions

This repository is shared to reflect my contribution as both a communicator and analytical collaborator in a technical team setting.

---

## Repo Contents

.
├── FinalVersion.ipynb # Full analysis notebook
├── EmotionalDialogue.ipynb # Draft notebooks
├── FindPeaks.ipynb # Peak detection via Gaussian fitting
├── Anger/, Disgust/, etc. # Labeled audio directories
└── README.md # This file

---

## Skills Demonstrated
`Scientific Communication` · `Collaborative Statistical Analysis` · `Slide Design` · `Research Framing` · `Translating Technical Concepts for Mixed Audiences` · `Team Collaboration`

---

## Course Info
**COGS118C: Neural Signal Processing**  
UC San Diego · Winter 2025
