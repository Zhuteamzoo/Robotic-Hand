# 🦾 How My Robotic Hand Works

For this project, I used a glove with **aluminum foil sensors** to control a **robotic hand made with servos and strings**.

## How I Built It
I placed **two pieces of aluminum foil** on each finger of a glove — one on top and one on the bottom.  
In the **middle of each finger**, I left a small gap so that when I **bend my finger**, the two foil pieces don’t touch.  
When the finger is **straight**, they touch each other and complete the circuit.

Each pair of aluminum foil pieces was connected to the **Arduino’s digital pins**.  
Then, I connected **servo motors** to the robotic hand. I tied **strings from each servo to each finger** of the robotic hand.  
The code on the Arduino reads whether the foil is **touching or not** and moves the servo motor based on that signal.

## How It Works
- When my finger is **straight**, the aluminum foil **touches** → signal is **HIGH** → servo **stays still**.  
- When my finger is **bent**, the aluminum foil **does not touch** → signal is **LOW** → servo **pulls the string** and **bends the robotic finger**.  
- When I straighten my finger again, the foil connects → the servo moves back to its original position.

In simple terms:  
👉 My real finger position controls the foil sensor  
👉 The foil sensor sends a signal to the Arduino  
👉 The Arduino tells the servo motor to move  
👉 The servo pulls the string to bend the robotic finger

This way, the **robotic hand copies the movement of my real hand**.
