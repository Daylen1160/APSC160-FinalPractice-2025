# 🔴 Temperature-Based Weather Indicator with LEDs

**Recommended Time:** 25–30 min  
**Topics:** Analog Input, Digital Output, Conditional Statements, Functions, Serial Communication

## Description

Write an Arduino program that reads the **external temperature** using a sensor connected to **analog pin A0** and displays the **weather state** using **three LEDs** connected to digital pins 2, 5, and 8. The program should:

1. **Read the analog voltage** from the temperature sensor.  
2. **Convert the analog reading** (0–1023) to a voltage (0–5V) using:
`voltageValue = sensorValue * (MAX_VOLTAGE_VAL / MAX_ANALOG_VAL)`

3. **Compute the temperature in °C** using the formula:
`temperatureValue = ((voltageValue * 1000) - 500) / 10`

4. **Turn on the corresponding LED** based on the temperature:

- **Cold (temperature < 0°C):** Blue LED ON, Green and Red LEDs OFF.  
- **Moderate (0°C ≤ temperature ≤ 40°C):** Green LED ON, Blue and Red LEDs OFF.  
- **Hot (temperature > 40°C):** Red LED ON, Blue and Green LEDs OFF.  

5. **Print the temperature and weather state** to the Serial Monitor.

The program must implement the following functions:

- `float findTemp(float voltageValue)`: Converts the sensor voltage to temperature in °C and prints the value.  
- `void turnOnLED(float temperatureValue)`: Determines which LED to turn on based on the temperature and prints the weather state.

## Input / Output

**Input:**  
- Temperature sensor connected to analog pin A0.

**Output:**  
- LEDs indicating weather state: Blue for cold, Green for moderate, Red for hot.  
- Serial Monitor displays the temperature in °C and the corresponding weather description.

## Example Behavior

1. Sensor reads -2°C → Blue LED ON → Serial prints:  
The temperature is -2°C.
The weather is cold.

2. Sensor reads 25°C → Green LED ON → Serial prints:  
The temperature is 25°C.
The weather is moderate.

3. Sensor reads 45°C → Red LED ON → Serial prints:  
The temperature is 45°C.
The weather is hot.

The sequence continues, updating the LED state and Serial Monitor as the temperature changes.

## Template

**TinkerCAD Link:** https://www.tinkercad.com/things/4BXXICF1GpV-temperature-sensor?sharecode=xwuQYecxHJdIN7UifSqSt4z3AKLCIoTlTFs2ChgCp68
