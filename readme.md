# ⚙️ MARK LIV — Personal AI Assistant

[![Python](https://img.shields.io/badge/Python-3.11%2B-blue.svg)](https://www.python.org/)
[![PyQt6](https://img.shields.io/badge/UI-PyQt6-green.svg)]()
[![Gemini](https://img.shields.io/badge/AI-Gemini%20Live-orange.svg)]()

**MARK LIV** is a cross-platform, real-time personal AI assistant capable of voice interaction, system control, web search, visual awareness, persistent memory, automation, and customizable skills.

The application supports **Windows, macOS, and Linux** and uses the Gemini Live API for real-time voice communication.

> **Customized and maintained by Saif Yaseen.**

---

## ✨ Features

### 🎙️ Voice & AI

* Real-time voice conversations
* Gemini Live API integration
* Wake-word support with **"Hey Jarvis"**
* Push-to-talk with `Ctrl + Space`
* Multiple Gemini voices
* Automatic language adaptation
* Session continuity
* Self-echo protection

### 🧠 Memory

* Persistent long-term memory
* Local memory storage
* On-demand memory retrieval
* Memory management panel
* Session summaries
* User preference storage

### 🖥️ Computer Control

* Launch applications
* Control volume and brightness
* Wi-Fi control
* Keyboard shortcuts
* Mouse and window control
* Desktop and taskbar operations
* File creation, movement, renaming and organization
* Undo support for supported actions

### 🌐 Web & Information

* Web search
* News search
* Research mode
* Price lookup
* Comparison searches
* Weather information
* Flight searches
* Browser control

### 👁️ Vision

* Screen capture
* Webcam support
* Visual analysis through Gemini
* Dynamic content panel

### 🧩 Plugin & Action System

MARK LIV uses a modular architecture where additional skills can be added through Python files.

Plugins and built-in actions can provide functionality such as:

* Quizzes
* Document analysis
* Messaging
* Reminders
* Weather
* Code assistance
* Game updates
* Browser automation
* File processing

### 🎨 User Interface

* PyQt6 HUD
* Animated avatar
* Real-time lip synchronization
* Facial expressions
* Reactive audio waveform
* Custom HUD colors
* Voice selection
* Avatar/reactor HUD modes
* Hardware monitoring

---

## 🏗️ Technology Stack

| Component            | Technology                 |
| -------------------- | -------------------------- |
| Language             | Python                     |
| AI                   | Gemini Live API            |
| UI                   | PyQt6                      |
| Numerical Processing | NumPy                      |
| Voice                | Real-time audio processing |
| Vision               | Screen/Webcam capture      |
| Automation           | OS-specific controls       |
| Memory               | Local JSON storage         |
| Plugins              | Python modules             |

---

## 📁 Project Structure

```text
MARK-LIV/
├── main.py
├── ui.py
├── setup.py
│
├── actions/
│   ├── web_search.py
│   ├── screen_processor.py
│   ├── reminder.py
│   ├── system_monitor.py
│   ├── computer_settings.py
│   ├── computer_control.py
│   ├── browser_control.py
│   ├── file_controller.py
│   ├── file_processor.py
│   ├── weather_report.py
│   ├── flight_finder.py
│   ├── code_helper.py
│   └── desktop.py
│
├── plugins/
│   ├── quiz.py
│   ├── document_review.py
│   └── _template.py
│
├── memory/
│   ├── memory_manager.py
│   ├── config_manager.py
│   └── long_term.json
│
├── core/
│   ├── prompt.txt
│   ├── avatar.py
│   ├── avatar_mesh.py
│   ├── viseme.py
│   ├── echo.py
│   ├── hotkey.py
│   ├── undo.py
│   ├── confirm.py
│   ├── audio_devices.py
│   ├── plugin_loader.py
│   ├── action_loader.py
│   └── wake_word.py
│
└── config/
    ├── api_keys.json
    └── certs/
```

---

## 🚀 Quick Start

### Requirements

* Windows 10/11, macOS, or Linux
* Python 3.11, 3.12 or 3.13
* Microphone
* Speakers
* Free Gemini API key

A GPU is **not required** because the avatar is rendered using software.

### Installation

```bash
git clone <your-repository-url>
cd MARK-LIV
```

Install the dependencies:

```bash
python setup.py
```

Or:

```bash
pip install -r requirements.txt
```

Start the application:

```bash
python main.py
```

---

## 🔐 Configuration

On first launch, configure your Gemini API key through the application.

Configuration and local data are stored under:

```text
config/
memory/
```

Keep sensitive files out of Git:

```text
config/api_keys.json
config/certs/
memory/long_term.json
```

Never commit API keys or private credentials to a public repository.

---

## 🧠 Architecture

MARK LIV follows a modular architecture:

```text
                    MARK LIV
                       │
        ┌──────────────┼──────────────┐
        │              │              │
      Gemini          UI           Memory
        │              │              │
        └───────┬──────┴──────┬───────┘
                │             │
             Actions       Plugins
                │             │
                └──────┬──────┘
                       │
                Operating System
```

The assistant discovers available actions and plugins at runtime, allowing additional functionality to be added without changing the core application.

---

## 🎯 Main Capabilities

MARK LIV can:

* Hold real-time voice conversations
* Control supported computer functions
* Search the web
* Analyze files
* Analyze screen content
* Remember information locally
* Execute multi-step tasks
* Schedule reminders
* Monitor system hardware
* Control supported browser functions
* Send supported messages
* Provide code assistance
* Customize its appearance and voice

---

## 🛠️ Customization

The assistant can be customized through the application configuration.

Supported customization includes:

* Assistant name
* User name
* Voice
* HUD color
* Avatar/reactor interface
* Wake word
* Enabled plugins
* Memory

Prompt behavior can also be customized through:

```text
core/prompt.txt
```

---

## 🔒 Privacy

Personal information and application memory are stored locally.

Sensitive configuration files should remain excluded from version control.

The Gemini Live API is used for the assistant's AI and real-time voice functionality, so information sent through an active Gemini session is processed by Google's service.

---

## 📌 Project Information

**Project:** MARK LIV
**Type:** Personal AI Assistant
**Language:** Python
**Interface:** PyQt6
**AI:** Gemini Live API
**Platforms:** Windows / macOS / Linux

**Developer / Maintainer:** Saif Yaseen

Portfolio:

**https://saifportfolios.vercel.app/**

---

## 📄 License & Attribution

This repository is based on an existing open-source MARK LIV project.

The original project is licensed under:

**Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)**

The applicable license and required attribution must be retained when redistributing or modifying the project.

This repository represents a customized/modified version maintained by **Saif Yaseen**.

---

<div align="center">

## ⚙️ MARK LIV

### Personal AI Assistant

**Python • PyQt6 • Gemini Live API**

**Customized and maintained by Saif Yaseen**

</div>
