# 🚗 URDF Demo – Simple Car Model (ROS 2 Humble)

A minimal **URDF (Unified Robot Description Format)** demo that visualizes a simple **car-like robot model** in **RViz 2** or **Gazebo**.  
This project is ideal for beginners learning ROS 2 Humble and URDF basics — including links, joints, and visualization.

---

## 📦 Features
- Simple 4-wheel car URDF using `<link>` and `<joint>`
- Launch file for easy visualization in **RViz 2**
- Compatible with **ROS 2 Humble (Ubuntu 22.04)**
- Lightweight and screenshot-ready (no sensors, controllers, or simulation dependencies)

---

## 🛠️ Prerequisites
Ensure you have:
- Ubuntu 22.04 LTS  
- ROS 2 Humble installed  
- colcon build tools

---

```bash
sudo apt update
sudo apt install ros-humble-desktop python3-colcon-common-extensions -y
```
---

⚙️ Building the Workspace
```bash
Copy code
cd ~/ros2_ws
colcon build --symlink-install
source install/setup.bash
```
---

🚀 Launch the Car Model in RViz 2
```bash
Copy code
ros2 launch urdf_demo view_car.launch.py
```

This will:

Start the robot_state_publisher

Launch RViz 2

Display the car_demo.urdf model (a red body with black wheels)


🖼️ Expected View
Once launched, you’ll see:

A red car body

Four black wheels

Positioned on the RViz grid

💡 Tip:
If the model doesn’t appear, set the RViz Fixed Frame to base_link.

---

🗂️ Project Structure
go
Copy code
urdf_demo/
│
├── launch/
│   └── view_car.launch.py
│
├── urdf/
│   └── car_demo.urdf
│
├── package.xml
└── CMakeLists.txt

---
📸 Screenshots

![WhatsApp Image 2025-10-24 at 19 32 05_a3d58e51](https://github.com/user-attachments/assets/a6d5c4dd-9a9a-4e11-b09b-a77f5e9902c1)
