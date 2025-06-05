# 🚦 Traffic Optimization at Intersections using YOLOv8 and Real-Time Scheduling

Managing urban traffic — especially at busy intersections — is one of the biggest challenges in modern cities. Traditional traffic lights operate on fixed timers, which don’t account for the constantly changing traffic conditions. This leads to long waiting times, traffic congestion, and increased pollution.

## 🌐 Problem Statement

Current traffic control systems lack adaptability and fail to respond dynamically to real-time traffic flow or emergency situations. As a result:

* 🚗 Vehicles often wait longer than necessary.
* 🚑 Emergency vehicles struggle to pass through congested intersections.
* 🌫️ Urban air quality worsens due to idling and congestion.

## 💡 Our Solution

We're building an **intelligent traffic signal control system** that adapts in real-time using computer vision and machine learning. By leveraging **YOLOv8** for vehicle detection and a custom **priority-based scheduling algorithm**, our system aims to:

* 📸 Detect and classify vehicles (cars, buses, bikes, ambulances, etc.) from live traffic feeds.
* 📊 Track vehicle counts and positions in each lane using **Ultralytics’ built-in tracker**.
* ⏱️ Dynamically adjust traffic signal timings based on real-time traffic volume.
* 🚨 Prioritize emergency vehicles to ensure quick passage.

## 🧠 How It Works

1. **Vehicle Detection:**
   A custom-trained **YOLOv8** model identifies and classifies vehicles, including emergency types, from traffic camera footage.

2. **Vehicle Tracking:**
   Using Ultralytics' default tracker, the system tracks vehicle positions and counts per lane in real time.

3. **Dynamic Scheduling Algorithm:**
   The algorithm:

   * Prioritizes lanes with emergency vehicles.
   * Allocates green light duration based on vehicle density in each lane.

4. **Signal Control:**
   Based on the input from the tracking system and the scheduling algorithm, the traffic signals are updated on-the-fly to optimize flow.

## 🚀 Features

* ✅ Real-time vehicle detection and tracking
* 🚦 Adaptive traffic light control based on live traffic conditions
* 🚨 Emergency vehicle prioritization
* 📈 Performance benchmarking with traditional fixed-time algorithms

## 🧪 Testing & Validation

We are simulating and testing our solution in realistic intersection environments to measure improvements in:

* Average vehicle wait time
* Emergency vehicle response time
* Overall traffic flow efficiency

## 🔍 Tech Stack

* **YOLOv8** for object detection
* **Ultralytics Tracker** for real-time vehicle tracking
* **Python** for core logic and algorithms
* **OpenCV** for video processing
* **Custom Scheduling Algorithm** for adaptive signal control

---

## 📌 Future Plans

* 🌍 Deploy to real intersections with live camera feeds
* 📊 Collect long-term traffic data for continuous model improvement
* 🤝 Collaborate with urban traffic authorities for pilot programs

---

## 🤝 Contributing

Contributions are welcome! If you're interested in traffic optimization, computer vision, or real-time systems, feel free to open issues or submit PRs.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

Let me know if you'd like this description broken into a `README.md` with code setup instructions and folder structure!
