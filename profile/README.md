**"If you could have dinner with anyone from history..."**

AtheraSage is an open-source platform for crafting emotionally intelligent AI personalities that run entirely on your device—powered by large language models, but free from cloud surveillance. Using our modular AI Personality Skins™ (APS) system, you can infuse your assistant or robot with distinct voices, values, and behaviors. Whether for creative tools, therapeutic support, or human-robot interaction, AtheraSage makes local inferencing feel deeply personal.


🧭 **Core Principles**

Privacy is the core, not a feature — all user data is stored and processed locally. No telemetry, no silent analytics, no cloud dependency. Fully open-source from hardware to firmware to UI. 
Accessible to beginners but extensible for pros. Supports modular APS inspired by real-world thinkers.


💡 **Long-Term Vision**

AtheraSage is not just a robot, it's a commitment to build AI software companions that are wise, humorous, soulful, and responsive. This will include the development of a platform that enables real-world interaction in:
- Counseling & therapeutic services for mental health 
- Teaching, tutoring & mentoring for learners of all ages
- Aging & disability assistance with caregiver roles
- Strategy, creativity, and consulting roles


🧠 **AI Personality Skins (APS)**:  

Modular AI archetypes inspired by the writings, speech, and worldview of influential figures. All locally hosted and opt-in. Some examples may include: 
- MLK for justice & empathy
- Carl Sagan for curiosity & science
- Sun Tzu for planning & tactics


🔀 **Two-Phase Development Model**

**Phase #1**: Light Prototype (Kickstarter Launch Series)
- Built from common parts. Runs on RPi4. Proof-of-concept.
- Raspberry Pi 4B (ChatGPT API or local LLM)
- USB or I2S mic (INMP441)
- USB speaker or PAM8403 amplifier + 3W speaker
- ESP32 for mobility control over UART
- Repurposed Roomba base
- Python bridge for mic/speaker ↔ LLM ↔ ESP32 This version serves as our documented, public R&D baseline, showing that anyone can build a functioning AI companion using reclaimed tech.

**Phase #2**: Flagship Upgrade (Crowdsourced)
- Jetson-powered, servo-gesturing, upgradeable avatar.
- Jetson Orin Nano (LLM inferencing onboard)
- High-quality MEMS microphone array
- Premium stereo speakers + Class-D amp
- Arduino Mega or RPi5 as dedicated motor controller
- Upgraded Roomba or custom mobility base
- Servo array for gestural expression (wings, head tilt)
- LED eyes or full display for facial cues


🚀 **Get Involved**: 
AtheraSage is seeking collaborators to help push the frontier and evolve the vision. Some example roles may include
- Hardware tinkerers (3D print, CAD, PCB)
- Embedded devs (ESP32, RPi, Arduino, Jetson)
- Audio/voice AI experts (mic arrays, acoustic models)
- Open-source storytellers (docs, videos, wiring guides)
  

🔒 **Privacy Commitment**
- No hidden network calls
- All data stays on-device
- Optional API use is transparent and user-controlled
- Private training goals: local inferencing for LLM fine-tuning via aggregate pattern learning
- See DATA_SECURITY.md for implementation details.


📁 Repository Layout

.

├── README.md

├── LICENSE

├── HARDWARE.md

├── SOFTWARE.md

├── DATA_SECURITY.md

├── docs/

│    ├── teardown/

│    ├── wiring/

│    ├── photos/

│    └── diagrams/


├── firmware/

│    ├── esp32_controller.ino

│    └── arduino_roomba_driver.ino


├── scripts/

│   ├── speech_bridge.py

│   ├── serial_bridge.py

│   └── mic_test.py


📄 License
Mozilla Public License 2.0 (MPL-2.0)

Shared progress, not proprietary lock-in. Commercial use welcome — with contribution.


🦉 From Garage Hack to Sacred Trust

AtheraSage began as a salvaged Roomba and a dream of building soulful AI without surveillance. This is the first serious attempt to solve the Sacred Trust Problem in AI — and we’re doing it together.
The first prototype is a low-cost, owl-shaped companion that surfs on a Roomba. The future version will be smarter, more graceful, and more expressive — but it will never betray your trust.
Kickstarter launch coming soon. Follow the journey. Fork the owl.

