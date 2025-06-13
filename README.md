# Intelligent_Excuse_Generator

## Overview

The **Intelligent Excuse Generator AI System** is a cutting-edge, Python-based tool designed to create context-aware, believable, and customizable excuses for various life situations. It supports scenarios such as work, school, social gatherings, and family commitments, and offers dynamic features including proof generation, simulated emergencies, smart ranking, and predictive scheduling. This AI system is ideal for users seeking creative, well-crafted explanations in a pinch.

---

## Key Features

### ✨ Contextual Excuse Generation

Generate realistic, scenario-specific excuses with customizable urgency and tone:

* **Scenarios**: Work, School, Social, Family
* **Urgency Levels**: Low, Normal, High
* **Tones**: Formal or Emotional

### 📋 Proof Generator

Auto-create supporting materials to back up your excuse:

* Fake **chat logs**, **location histories**, and **documents** (e.g., doctor’s notes, appointment slips)
* Files saved in `/proofs/` with timestamps for authenticity

### 📱 Emergency Call & Text Simulator

Simulate incoming calls and emergency texts:

* Custom messages depending on selected scenario
* Text previews for realism and screenshot usage

### 🙏 Guilt-Tripping Apology Generator

Craft believable apologies tailored to your tone:

* Formal apologies for professional contexts
* Emotional apologies for friends and family situations

### 🎤 Voice Output (Offline TTS)

Convert excuses to speech and export as MP3 files:

* Uses `pyttsx3` for offline text-to-speech
* Compatible with Windows (SAPI5), macOS (nsss), and Linux (espeak)

### 🔝 Smart Excuse Ranking Engine

Keeps track of previous excuses and their outcomes:

* Learns which types of excuses work best
* Offers ranked suggestions based on past success rates

### ⏰ Predictive Auto-Scheduling

Analyzes timestamps and usage frequency:

* Predicts your next likely excuse scenario
* Suggests pre-emptive excuses

---

## Project Structure

```
Intelligent_Excuse_Generator/
├── core/
│   ├── excuse_generator.py
│   ├── proof_generator.py
│   ├── emergency_system.py
│   ├── apology_generator.py
│   ├── voice_generator.py
│   ├── ranking_engine.py
│   └── scheduler.py
├── data/
│   └── templates.json
├── proofs/
├── main.py
└── README.md

```

---

## Installation & Setup

### 1. Requirements

* Python 3.7+
* pip (Python package manager)

### 2. Dependency Installation

Install required packages using:

```
pip install pyttsx3

```

> **Note:** Ensure voice engines are set up properly:
>
> * Windows: Uses SAPI5 (default)
> * macOS: Uses `nsss`
> * Linux: Requires `espeak` or `espeak-ng`

### 3. Folder Setup

Place the project directory anywhere on your system. Ensure the following:

* `data/` contains the `templates.json`
* `proofs/` exists and is writable (auto-saves generated files)

---

## Usage Guide

### Launching the App

Run the main script from your terminal:

```
python main.py

```

### Input Prompts

You will be prompted to choose:

* **Scenario**: work / school / social / family *(default: work)*
* **Urgency**: low / normal / high *(default: normal)*
* **Tone**: formal / emotional *(default: formal)*

#### Example:

```
Scenario (work, school, social, family) [work]: school
Urgency (low, normal, high) [normal]: high
Tone (formal, emotional) [formal]: emotional

```

### Output Actions

The system will:

* Display a generated excuse
* Show an apology message
* Save fake proof files in `/proofs/`
* Simulate emergency call/SMS texts
* Generate an MP3 voice message of the excuse
* Show ranking data of previously used excuses
* Predict and display next probable excuse need

---

## Customization & Extensions

* **Templates**: Modify or expand `data/templates.json` to add new excuse types or scenarios.
* **Proofs**: Upgrade proof generation to include image manipulation, scanned docs, or PDF exports.
* **Database Integration**: Store ranking/scheduling data across sessions.
* **UI/UX Enhancements**: Add a Tkinter or web-based GUI frontend for ease of use.
* **Multilingual Support**: Extend template and TTS logic for regional languages.

---

## Troubleshooting

### Voice Generation Not Working?

* Ensure your system has a compatible TTS engine:

  * Windows: SAPI5 pre-installed
  * macOS: Use `nsss`
  * Linux: Install `espeak` or `espeak-ng`

### Python Errors?

* Check that `pyttsx3` is correctly installed.
* Run in a clean virtual environment if issues persist.

### File Permission Issues?

* Make sure `proofs/` directory is writable by your Python process.

---

## Disclaimer

This tool is intended **strictly for entertainment, educational, and research purposes**. Generated content is fictional. Misuse for deception or unethical behavior is strongly discouraged.

Use responsibly.

---

Enjoy your AI-powered excuse-making experience!

---

Enjoy your AI-powered excuse-making experience!
