# 🟢 Opposite-Pair LED Lighting Sequence

**Recommended Time:** 15–20 min  
**Topics:** Digital Output, Timing, LED Control, Sequential Logic

## Description

Write an Arduino program that controls **8 LEDs** connected to digital pins.  
Your task is to light the LEDs in **opposite pairs**, beginning from the outermost LEDs and moving inward.

The required ON sequence is:

1. Turn ON LEDs **1 and 8**, then wait **1 second**  
2. Turn ON LEDs **2 and 7**, then wait **1 second**  
3. Turn ON LEDs **3 and 6**, then wait **1 second**  
4. Turn ON LEDs **4 and 5**, then wait **1 second**

After all pairs have been turned on, turn them **OFF** in the opposite pairing order:

5. Turn OFF LEDs **4 and 5**, then wait **1 second**
6. Turn OFF LEDs **3 and 6**, then wait **1 second**  
6. Turn OFF LEDs **2 and 7**, then wait **1 second**  
7. Turn OFF LEDs **1 and 8**, then wait **1 second** 

Once complete, the full sequence must **repeat indefinitely**.

Your program must print the ON/OFF state of each LED to the Serial Monitor as the sequence runs.

## Input / Output

**Input:**  
- No user input is required.

**Output:**  
- LEDs physically turn ON/OFF following the pair sequence.  
- Serial Monitor prints messages such as:  
  - `"LED #1 is On."`  
  - `"LED #8 is Off."`  

## Example Behavior

The LED pattern should appear to “move inward” as pairs turn ON: (1,8) → (2,7) → (3,6) → (4,5)
Then “move outward” as pairs turn OFF: (1,8) → (2,7) → (3,6) → (4,5)
With a **1-second delay** between all transitions.

# Template:

**TinkerCAD Link**: https://www.tinkercad.com/things/4YEI4BSLE7D-led-blink-simulation-ii?sharecode=jt-emIk-G1mPrQdTtt8rkWRqdhkKCjbeEitk9DUErc0
