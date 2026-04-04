---
layout: default
title: Projects - Mert Melih Albay
---

<p>
  <a href="index.html">Home</a> | 
  <strong><a href="projects.html">Projects</a></strong> | 
  <a href="../projects.html">TR</a>
</p>

<hr>

<h2 style="color: #2e81b7;">Deep Learning-Based Optical Inspection and Visual Defect Detection Module</h2>
<p>
  The module utilizes deep learning architectures (YOLO) and computer vision (OpenCV) techniques to identify electronic components (resistors, diodes, MOSFETs, ICs, etc.) on a PCB in real-time and autonomously detect visual defects. This unit aims to digitize manual inspection processes and minimize human-induced error margins by analyzing physical anomalies such as missing parts, misalignment, solder bridges, and corrosion through high-resolution imagery.
</p>

<p>
  <span class="proje-vurgu">Dataset Management and Labeling:</span> A unique dataset was created for model performance; PCB components were manually labeled to prepare a high-accuracy training pool.
</p>

<p>
  <span class="proje-vurgu">Data Augmentation:</span> To ensure stable operation under varying lighting conditions, perspective angles, and noise levels; techniques such as rotation, brightness adjustment, and scaling were applied to optimize the model's robustness.
</p>

<p>
  <span class="proje-vurgu">YOLO and OpenCV Integration:</span> The YOLO architecture was employed for real-time object detection. Camera data is processed through the OpenCV library for pre-processing (noise reduction, contrast enhancement) to maximize analysis efficiency.
</p>

<p>
  <span class="proje-vurgu">Autonomous Defect Detection:</span> Using a non-contact analysis method; missing parts, incorrect placement, and solder anomalies are autonomously identified, digitizing the diagnostic process.
</p>

<h4 style="color: #2e81b7;">- System Performance: Object Detection and Defect Analysis Data</h4>
<img src="../assets/002png.png" width="600" height="300">
<img src="../assets/001.png" width="600">

<hr>

<h2 style="color: #2e81b7;">CNC-Probe: 3-Axis Robotic Platform for Thermal and Electrical PCB Analysis</h2>
<p>
  This device aims to perform detailed physical inspections on a PCB using a 3-axis robotic platform. Initially, it maps the board thermally based on suspicious points identified by AI, instantly detecting short circuits and overheating zones invisible to the naked eye. Simultaneously, it performs automatic electrical measurements with an autonomous probe tip, determining the fault location with millimetric precision.
</p>

<h4 style="color: #2e81b7;">- Project Workflow Diagram</h4>
<img src="../assets/Otomatik Optik İnceleme.png" width="700" height="400">

<h4 style="color: #2e81b7;">- System Working Principle</h4>
<p>
  <span class="proje-vurgu">1. Simultaneous Optical and Thermal Scanning:</span> A fixed high-resolution optical camera and an MLX90640 thermal camera operate concurrently to generate a general image and global heat map of the entire PCB in a single pass.
</p>
<p>
  <span class="proje-vurgu">2. AI-Driven Optical Analysis:</span> The trained YOLO model scans the board via the optical image to identify the pixel coordinates of missing, faulty, or suspicious components.
</p>
<p>
  <span class="proje-vurgu">3. Thermal Verification and Data Fusion:</span> Suspicious pixels detected in the optical image are cross-referenced with corresponding regions on the global thermal map. Temperature data in that region is analyzed to software-verify potential short circuits or overheating.
</p>
<p>
  <span class="proje-vurgu">4. Mechanical Coordinate Transformation:</span> Pixel coordinates of verified faulty regions are converted into millimetric X-Y coordinates for the CNC mechanism using a calibration matrix (Homography).
</p>
<p>
  <span class="proje-vurgu">5. Autonomous Electrical Testing:</span> The 3-axis arm directs the measurement probe to these calculated coordinates to perform physical measurements.
</p>

<h4 style="color: #2e81b7;">- Measurement Platform Chassis</h4>
<img src="../assets/CNC KARKASI - 2D(2)_page-0001.jpg" width="600">

<hr>

<h2 style="color: #2e81b7;">High SNR Amplifier for Low-Amplitude Signals</h2>
<p>
  This project is a high-performance pre-amplifier design that boosts weak analog signals from microphones or low-output pickups without exposing them to the circuit's own electrical and thermal noise. The primary goal is to preserve natural sound dynamics using low-noise components and precision impedance matching techniques to achieve a maximum signal-to-noise ratio (SNR).
</p>

<hr>

<h2 style="color: #2e81b7;">Analyzing Synchronous Generator Characteristics under Dynamic Load Conditions via MATLAB GUI</h2>
<p>
  This interactive MATLAB application is designed to visualize and analyze the performance characteristics of a specific synchronous generator under varying power factor conditions. Using a slider, the power factor can be dynamically adjusted to observe changes in input torque, efficiency, and voltage regulation.
</p>

<p>
  <img src="../assets/abc.gif" alt="Project Demo">
</p>
<p>
  <a href="https://www.youtube.com/watch?v=nGcnPR7hnCM" target="_blank">▶️ Project Demo and Video Recording</a>
</p>

<hr>

<h2 style="color: #2e81b7;">Comprehensive Indoor Electrical Installation and Load Distribution Management</h2>
<p>
  This study adopts a holistic engineering approach to the electrical infrastructure requirements of a modern residential building. The process focused on architectural requirement analysis, load estimation, and technical calculation integration to establish a safe and efficient energy distribution system.
</p>

<h4 style="color: #2e81b7;">- 2D Electrical Installation Floor Plan (AutoCAD)</h4>
<img src="../assets/IlluminationFinalProject.jpg" width="600">

<h3 style="color: #2e81b7;">Technical Implementation Details</h3>
<p>
  Architectural plans and general building hierarchy were designed in AutoCAD according to technical standards. Voltage drop (%e) calculations were performed for each line to ensure safe operation. A Load Table was created based on international standards to analyze energy demand and system balance. Detailed light source calculations were completed using the Zijl Method for each room.
</p>

<h4 style="color: #2e81b7;">- Power Distribution and Load Table Analysis</h4>
<img src="../assets/loadingTabel.png" width="600">
<p>
  Total installed power was calculated at 80,504 W; however, a simultaneity factor was applied to normalize demand power to 36,226.8 W to reflect real-time operating characteristics. Dedicated circuits were designed for high-power equipment, including washing machines, dishwashers, and ovens. A 63 A fuse was selected for the main distribution board, and a safe voltage drop value of 0.31% was achieved in the main supply line.
</p>

<p>
  <a href="https://youtu.be/-xOm79f4XDA" target="_blank">▶️ Detailed Project Video on YouTube</a>
</p>
<p>
  <a href="../assets/MertMelihAlbay_CV_ENG.pdf" class="cv-button" download>Download Resume (PDF)</a>
</p>
