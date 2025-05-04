# AQUASENSE-AI
For this project, we created a variety of models to address a single issue: intelligent canal water leak detection.
check the csv file to explore the data used for those models
we used 4 variables to train the model(timestamp, temperature, flow, pressure)
![image](https://github.com/user-attachments/assets/cae85159-b835-41ea-abe1-44e34791f5ed)
These diagrams give us a detailed look at pressure and flow measurements.Let’s break down what each one tells us and what we can learn from them.
# 1. Pressure Distribution
This chart shows how often different pressure levels occur, with labels for "normal" operation and potential "leaks." The pressure values range from 1.8 to 3.0, and the counts tell us how frequently each value appears.
Most pressure readings cluster around certain points (2.0, 2.5, etc), meaning the system usually operates within these ranges.
If some values show up much more often under "leak" conditions, that could help set thresholds for detecting issues.
# 2. Flow Distribution
The x-axis represents flow values (14, 16, ..., 22), while the y-axis shows counts (0 to 500). This suggests the diagram tracks how often specific flow rates occur over a 6-hour period, not pressure.
The counts tell us how frequently certain flow rates appear. For example, a count of 500 at flow rate "14" means that value occurred 500 times in the 6-hour window.

Peaks (count=500) indicate common operating flow rates—likely "normal" conditions.

Dips (count=0) suggest rare or abnormal flow rates, possibly tied to leaks or system interruptions.
# 3. Pressure over time

This diagram describes the pressure variation over time.
The normal pressure level is between 2.5 and 3; the pressure varies a lot when there is no leak.
When the pressure is low (1.8-2.3), there is a high chance of a leak; the pressure varies less because there is constant water flow. 
# 4. Flow by zone
This chart compares flow rates across different zones (Zone A, Zone B, Zone C) and categorizes them as either:

Normal (expected flow)

Leak (abnormal flow, indicating potential issues)
Zone Performance

Each zone’s flow rate is labeled as Normal or Leak, helping pinpoint where problems occur.

Example: If Zone B has mostly Leak labels, it might have a recurring issue like a pipe crack or valve failure.

Leak Detection

Zones with frequent Leak labels need inspection—low flow could mean blockages, while unusually high flow might signal bursts.

Comparison Across Zones

If Zone A is always Normal but Zone C fluctuates, the problem is likely isolated to Zone C’s equipment or design.
 

