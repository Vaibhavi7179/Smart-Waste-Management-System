# Smart Waste Management & Bin Level Detection System

## Overview

The Smart Waste Management & Bin Level Detection System is a software-based IoT simulation project that monitors garbage bin fill levels and provides real-time status updates through an interactive dashboard. The system simulates ultrasonic sensor readings, calculates bin fill percentages, generates alerts for full bins, and stores monitoring data for analysis.

This project demonstrates core Internet of Things (IoT) concepts such as data acquisition, real-time monitoring, dashboard visualization, alert generation, and data logging without requiring physical hardware.

---

## Problem Statement

Traditional waste collection follows fixed schedules regardless of whether bins are full or empty. This leads to:

* Unnecessary collection trips
* Increased fuel consumption
* Higher operational costs
* Overflowing waste bins
* Poor environmental hygiene

The proposed system provides a smart monitoring solution that helps optimize waste collection operations by tracking bin fill levels and generating alerts when bins approach capacity.

---

## Objectives

* Simulate waste bin level monitoring
* Calculate fill percentage automatically
* Display bin status in real-time
* Generate alerts when bins are full
* Store historical monitoring data
* Visualize waste collection trends

---

## Features

* Real-time waste bin monitoring
* Fill percentage calculation
* Empty, Half-Full, and Full status detection
* Automatic alert generation
* Historical data logging
* Interactive dashboard using Streamlit
* Data visualization using charts
* CSV report generation

---

## Technologies Used

| Technology | Purpose                   |
| ---------- | ------------------------- |
| Python     | Core Programming Language |
| Streamlit  | Dashboard Development     |
| Pandas     | Data Processing           |
| CSV        | Data Storage              |
| VS Code    | Development Environment   |

---

## Project Architecture

```text
Simulated Bin Data
        ↓
Python Application
        ↓
Fill Percentage Calculation
        ↓
Status Classification
        ↓
Alert Generation
        ↓
Dashboard Visualization
        ↓
CSV Data Logging
```

---

## Project Structure

```text
Smart-Waste-Management-System/
│
├── data/
│   └── bin_log.csv
│
├── simulator.py
├── app.py
├── requirements.txt
└── README.md
```

---

## Installation

### Step 1: Clone Repository

```bash
git clone https://github.com/yourusername/Smart-Waste-Management-System.git
```

### Step 2: Navigate to Project

```bash
cd Smart-Waste-Management-System
```

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Running the Project

Execute the following command:

```bash
python -m streamlit run app.py
```

The dashboard will open automatically in your browser.

If it does not open automatically, visit:

```text
http://localhost:8501
```

---

## Fill Level Logic

The system assumes a bin height of 30 cm.

### Formula

Fill Percentage = ((Bin Height - Distance) / Bin Height) × 100

### Status Classification

| Fill Percentage | Status    |
| --------------- | --------- |
| 0% - 49%        | Empty     |
| 50% - 79%       | Half Full |
| 80% - 100%      | Full      |

---

## Sample Output

| Distance (cm) | Fill (%) | Status    |
| ------------- | -------- | --------- |
| 28            | 6.67     | Empty     |
| 15            | 50.00    | Half Full |
| 5             | 83.33    | Full      |

---

## Dashboard Components

* Distance Reading
* Fill Percentage
* Bin Status
* Alert Notification
* Historical Trend Chart
* Monitoring Log Table

---

## Applications

* Smart Cities
* Municipal Waste Management
* Educational Campuses
* Shopping Malls
* Railway Stations
* Airports
* Corporate Parks

---

## Future Enhancements

* ESP32 Hardware Integration
* Ultrasonic Sensor Support
* GPS-Based Bin Tracking
* Mobile Application Notifications
* Route Optimization
* AI-Based Waste Prediction
* Cloud Database Integration
* Multi-Bin Monitoring

---

## Learning Outcomes

Through this project, I learned:

* IoT System Design Concepts
* Real-Time Monitoring Systems
* Dashboard Development
* Python Programming
* Data Logging and Visualization
* Alert Management Systems
* Smart City Technology Applications

---

## Author

**Vaibhavi S K**

Bachelor of Engineering (Computer Science)

IoT Mini Project – Smart Waste Management & Bin Level Detection System

---

## License

This project is developed for educational and academic purposes.
