# arduino-4-servo-automated-motion
This project demonstrates the control of **4 servo motors** in a humanoid robot using an Arduino. The servos simulate basic leg movements and hold a neutral standing pose. Additionally, an algorithm for humanoid walking motion is described to support future development of robotic locomotion.

📋 Features

- Sweeps all 4 servo motors (like the Arduino Sweep example) for 2 seconds.
- Holds all servo motors at **90°** to simulate a neutral/standing position.
- Includes a **step-by-step walking algorithm** for future implementation in bipedal robots.

## 🧠 Walking Algorithm Overview

The humanoid walking sequence alternates weight shift and leg lift:
1. Shift weight to one leg.
2. Lift and move the opposite leg forward.
3. Place the leg down and shift weight.
4. Repeat with the other leg.

See `WALKING_ALGORITHM.md` for detailed pseudocode.

## 🛠 Hardware Requirements

- Arduino Uno (or compatible board)
- 4x Servo Motors (SG90 or similar)
- External power source for servos (recommended)
- Jumper wires and breadboard

## 📦 Installation

1. Connect the 4 servos to digital pins: **3, 5, 6, 9**.
2. Upload the code via Arduino IDE.
3. Power the servos and Arduino.
4. Watch the sweep → hold sequence.

## 🔧 How It Works

- The servos sweep back and forth for 2 seconds.
- Then all servos stop at 90° to simulate a balanced humanoid stance.
