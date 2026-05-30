# SPEC

SPEC is a personal assistant system written in Python. It is designed to run in the terminal and act as a simple command-based assistant with memory and expandable features.

At the moment, SPEC is focused on building a working base system that can accept user input, store information, and retrieve saved data.

---

## Current Features

- Command-line interface (runs in terminal)
- Accepts user input as commands or messages
- Simple memory system for storing information locally
- Uses JSON files to save and load data
- Basic response handling based on input type
- Persistent storage so information is kept between sessions

---

## How it works

SPEC runs as a loop in the terminal. When started, it loads any saved memory from a local file. It then waits for user input.

When the user types something:
- SPEC checks if it is a command
- If it is a memory command, it stores or retrieves information
- If it is not recognised, it may store it or ignore it depending on logic

All important data is saved locally so it can be used again in future sessions.

---

## Example usage

User input:
- "My name is Charlie"

SPEC response:
- Stores name in memory

User input:
- "What is my name?"

SPEC response:
- "Your name is Charlie"

---

## Project Structure (planned)

- main.py → core program loop
- memory.py → handles saving/loading data
- commands.py → processes user inputs

This structure may change as the project grows.

---

## Future ideas

- Integration with Gemini API for improved responses
- Smart home control using ESPHome devices
- Raspberry Pi sensor integration (motion, temperature, mmWave)
- Web interface for remote control
- Automation features based on events or triggers

---

## Notes

SPEC is still in early development and is being built step by step. The focus right now is making a stable core system before adding advanced features like AI or automation.
