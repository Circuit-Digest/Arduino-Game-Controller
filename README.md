# 🎮 Arduino Game Controller using Arduino Uno R4

Stressful day? Deadlines, noise, overthinking, endless scrolling… sometimes the best thing you can do is pause everything and play a game. Games have always been more than just entertainment — they refresh the mind and reset our mood.

This project brings back the nostalgia of classic joysticks and buttons, but with modern hardware. We build a **DIY Arduino Game Controller** using **Arduino Uno R4**, a joystick module, and push buttons that work as a **USB keyboard device** for PC games.

---

## 🔧 Project Overview

- Board acts as a **USB HID Keyboard**
- Joystick controls **arrow key movement**
- Push buttons trigger **custom keyboard keys**
- Plug & play with PC games that support keyboard input
- Beginner-friendly and fun to build

---

## 🧰 Components Required

| S.No | Component         | Quantity | Description |
|----|------------------|----------|------------|
| 1 | Arduino Uno R4 | 1 | Main controller |
| 2 | Push Buttons | 4 | Game action inputs |
| 3 | Joystick Module | 1 | Directional control |
| 4 | Vero Board | 1 | Neat and stable wiring |
| 5 | Jumper Wires | As required | Connections |

---

## 🔌 Circuit Diagram

- Joystick **X → A0**, **Y → A1**
- Push buttons → **Digital Pins (2–5)**
- Buttons use **INPUT_PULLUP**
- Arduino Uno R4 connected via USB

*(Refer to the circuit diagram image in the repository)*

---

## ⚙️ Hardware Setup

All components are mounted on a Vero board for a clean setup.  
The joystick provides analog movement, while buttons give digital input.  
Once connected to a PC, the Arduino is detected as a **keyboard device**.

---

## 🧠 Working Principle

1. Arduino Uno R4 initializes as a USB keyboard  
2. Joystick position is continuously monitored  
3. Based on joystick movement:
   - Left / Right / Up / Down arrow keys are sent
4. Button presses send mapped keys (`W`, `A`, `S`, `D`)
5. Keys are released automatically when input stops

This creates a smooth and responsive game control experience.

---

🎯 Applications

PC games with keyboard support

DIY arcade controller

HID device learning

Electronics and Arduino practice

📌 Conclusion

This project demonstrates how simple hardware inputs can be converted into digital commands using USB HID communication. It’s a compact, efficient, and educational project that blends nostalgia, electronics, and real-time control systems.

❓ FAQ

Q1. Can I use this with any PC game?
Yes, as long as the game supports keyboard controls.

Q2. Why the startup delay?
It ensures proper USB keyboard detection.

Q3. Can I change button keys?
Absolutely — just modify the key mappings in code.

Q4. Is this beginner friendly?
Yes! Perfect for Arduino and HID beginners.
