## Challenge 3: Designing a Reliable Homemade Flex Sensor

**Goal**  
For my robotic hand, I wanted to build homemade flex sensors that could detect finger bending and trigger servo movement, without using commercial sensors.

**Initial design (and why it failed)**  
My first design used strips of aluminum foil separated by paper. I expected that bending the finger would change the current flowing through the sensor. In practice, this setup barely responded at all. The electrical change was too small and inconsistent to be useful.

**Why this didn’t work**  
I realized that simply bending the materials wasn’t enough to reliably change the electrical behavior. The contact between the aluminum strips stayed mostly the same, even when the finger bent.

**Second design and key idea**  
I redesigned the sensor to include a small gap in the middle, with parts of the aluminum foil slightly overlapping. When the finger bent, the layers separated instead of compressing, which interrupted the current rather than trying to vary it continuously.

**What improved**  
This design produced a clearer on/off signal, which made it easier to control the servos. Instead of relying on small changes in current, the system responded to a more distinct electrical change.

**Limitations and evidence**  
I do not have a video of the final version of the hand. However, the prototype video shows the original sensor behaving inconsistently, with delayed or unreliable responses, which motivated the redesign.

**What I learned**  
This problem taught me that simplifying a signal can be more effective than trying to measure subtle changes. Designing for reliability mattered more than trying to make the sensor behave like a perfect analog device.
