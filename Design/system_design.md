# System Design

## Overview
This system is designed to monitor spacecraft data and detect problems early using AI. Instead of engineers watching everything manually, the system will check the data and alert them if something looks unusual.

## Main Components
The system has a few main parts:

1. Data Collection  
This collects sensor data from the spacecraft like temperature, pressure, and power levels.

2. Data Processing  
This step cleans the data and gets it ready to be analyzed. It removes errors and makes sure everything is organized.

3. AI Model  
The AI model learns what normal data looks like. Then it checks new data to see if anything is different or unusual.

4. Alert System  
If something strange is detected, the system sends an alert so engineers can check it.

5. User Interface  
This would allow engineers to see the data and alerts in a simple dashboard.

## How the System Works
The system works in steps:

1. Sensor data is collected  
2. The data is cleaned and prepared  
3. The AI model analyzes the data  
4. If something looks unusual, it is flagged  
5. An alert is sent to engineers  

## AI Method
This system uses anomaly detection. This means the model learns what normal behavior looks like and then finds anything that does not match.

Some examples include:
- Isolation Forest  
- LSTM (for time-based data)

## Data Flow
The data moves like this:

Sensor Data → Processing → AI Model → Alert → Engineer

## Design Goals
- Detect problems early  
- Work in real time  
- Reduce human effort  
- Improve safety  

## Limitations
- May send false alerts sometimes  
- May miss problems if not trained well  
- Needs good quality data  

## Summary
This design shows how an AI system can help monitor spacecraft systems. It makes it easier to catch problems early and helps improve safety during missions.
