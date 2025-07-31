Conversational Robotics That Respect Sacred Trust. Privacy-First by Design.

ATHERA is a privacy-anchored, open-source robotics initiative developing soulful, embodied AI companions that operate entirely on user-owned data. We are committed to local inferencing, transparency, and open collaboration — not as marketing, but as a mission. Our ultimate goal is to pioneer emotionally intelligent robotic agents that can counsel, teach, support, and inspire—without ever violating trust.


🧭 Core Principles

Privacy is the core, not a feature — all user data is stored and processed locally. No telemetry, no silent analytics, no cloud dependency. Fully open-source from hardware to firmware to UI. 
Accessible to beginners but extensible for pros. Supports modular AI Personality Skins (APS) inspired by real-world thinkers.

💡 Long-Term Vision

ATHERA is not just a robot. It's a commitment to build: 
A mobile AI companion that is wise, humorous, soulful, and responsive
A platform that enables real-world interaction in:
Counseling & therapeutic services
Teaching, tutoring & mentoring
Aging & disability assistance
Strategy, creativity, and consulting roles

🧠 AI Personality Skins (Experimental):  Modular AI archetypes inspired by the writings, voice, and worldview of influential figures. All locally hosted and opt-in.

- MLK for justice & empathy
- Carl Sagan for curiosity & science
- Bill Gates for business & philanthropy
- Sun Tzu for planning & tactics
- Dave Chappelle for wit & comic relief

🔀 Two-Fork Development Model

Fork #1: Light Prototype (Kickstarter Launch Series)
- Built from common parts. Runs on RPi4. Proof-of-concept.
- Raspberry Pi 4B (ChatGPT API or local LLM)
- USB or I2S mic (INMP441)
- USB speaker or PAM8403 amplifier + 3W speaker
- ESP32 for mobility control over UART
- Repurposed Roomba base
- Python bridge for mic/speaker ↔ LLM ↔ ESP32 This version serves as our documented, public R&D baseline, showing that anyone can build a functioning AI companion using reclaimed tech.

Fork #2: Flagship Upgrade (Crowdsourced)
- Jetson-powered, servo-gesturing, upgradeable avatar.
- Jetson Orin Nano (LLM inferencing onboard)
- High-quality MEMS microphone array
- Premium stereo speakers + Class-D amp
- Arduino Mega or RPi5 as dedicated motor controller
- Upgraded Roomba or custom mobility base
- Servo array for gestural expression (wings, head tilt)
- LED eyes or full display for facial cues This fork represents the community-driven future of ATHERA — a truly expressive, extensible, open robotics platform.

These packs are tributes — not impersonations. No cloud required. No user data leaves the device.

🌐 Stack Overview

# Fork #1
ChatGPT API or open LLM
Roomba (salvaged)
ESP32 via UART
Coqui, Vosk, Whisper
USB mic & speaker
Gestures: None

# Fork #2
Roomba Pro or custom tracked base
Local LLM on Jetson / API fallback
High-fidelity TTS (Piper, faster)
Arduino Mega / RPi5 (serial/i2c)
STT / TTS
MEMS mic array + stereo output
Gestures: Servo limbs, head tilt, wing flaps


🛠️ Installation

Dependencies:
- Python 3.10+
- Node.js (for optional GUI/dashboard)
- ESP32 toolchain / Arduino IDE
- Jetson Jetpack SDK (for Fork #2)
- Whisper, Piper, Vosk, or Coqui TTS/STT tools

Setup (Fork #1)

# Clone the repo
git clone https://github.com/youruser/ATHERA.git
cd ATHERA

# Create Python environment
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt

# Flash ESP32
cd firmware && make flash

Run Local Voice Loop

python scripts/speech_bridge.py

🚀 Get Involved

ATHERA is seeking collaborators to help push the frontier:

- Hardware tinkerers (3D print, CAD, PCB)
- Embedded devs (ESP32, Arduino, Jetson)
- Audio/voice AI experts (mic arrays, acoustic models)
- Open-source storytellers (docs, videos, wiring guides)
- Fork the repo. Join the build. Help evolve the vision.

🔒 Privacy Commitment

- No hidden network calls
- All data stays on-device
- Optional API use is transparent and user-controlled
- Private training goals: local LLM fine-tuning via aggregate pattern learning
- See DATA_SECURITY.md for implementation details.

📁 Repository Layout

.
├── README.md
├── LICENSE
├── HARDWARE.md
├── SOFTWARE.md
├── DATA_SECURITY.md
├── docs/
│   ├── teardown/
│   ├── wiring/
│   ├── photos/
│   └── diagrams/
├── firmware/
│   ├── esp32_controller.ino
│   └── arduino_roomba_driver.ino
├── scripts/
│   ├── speech_bridge.py
│   ├── serial_bridge.py
│   └── mic_test.py

📄 License

Mozilla Public License 2.0 (MPL-2.0)
Shared progress, not proprietary lock-in. Commercial use welcome — with contribution.

🦉 From Garage Hack to Sacred Trust

ATHERA began as a salvaged Roomba and a dream of building soulful AI without surveillance. This is the first serious attempt to solve the Sacred Trust Problem in AI — and we’re doing it together.
The first prototype is a low-cost, owl-shaped companion that surfs on a Roomba. The future version will be smarter, more graceful, and more expressive — but it will never betray your trust.
Kickstarter launch coming soon. Follow the journey. Fork the owl.

