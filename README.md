# **Autonomous Drone Project**

Welcome to the GitHub repository for my Open Source Autonomous Drone. This project brings together the best of open-source software and inexpensive hardware components to create an autonomous drone capable of both GPS waypoint missions, manual control, and soon full autonomy in GPS-Denied environments. Powered by Arducopter and built on a DJI frame, this is an ongoing hobby project I have been working on to learn about AI and Drones.


https://github.com/tmcgirr/Drone/assets/59525360/4c7c00aa-6234-4726-b9c9-2aa4cf8c86cc



---

## **Table of Contents**
- [Features](#features)
- [Components Used](#components-used)
- [Setup & Installation](#setup--installation)
- [Media Gallery](#media-gallery)
- [Links & Resources](#links--resources)
- [Contributing](#contributing)

---
(Updated DJI Phantom 3 Frame)

https://github.com/tmcgirr/Drone/assets/59525360/0599f1e1-abd8-46ec-8554-464f3995b2e9


## **Features**
- **Autonomous Flight:**
    Pre-programmed GPS waypoint missions for hands-free operations.
- **Manual RC Controller Flight:**
    Manual control for precision and exploration.
- **Object Detection:**
    Utilizes the OAK D Lite Stereo/RGB camera for various computer vision tasks.

## **Upcoming Features**
- **Fully Autonomous Flight:** Using 360 Lidar and SLAM (ROS2), the drone will be able to avoid obstacles, map building structures, and continue waypoint missions despite losing radio/telemetry signals.
- **4g Enhanced Range:** Using a 4g Wireless Modem for the Raspberry Pi, the drone will be able to send/receive flight commands and various forms of data anywhere a cell signal can be obtained. (BVLOS when FAA approves this type of operation)
- **Voice Activated Commands:** "Circle me at 30 feet with a 20-foot radius" can be converted from speech-to-text, interpreted by an LLM to analyze the dialog and output commands for drone commands (Possibly [Drone Kit](http://dronekit.io/) circle flight mode around current GPS coords). Think hands-free voice commands with the potential for chained flight commands that can leverage the Object Detection to provide context on the observed environment and perform subsequent actions as needed.
- **Audio Capture:** Fairly standard, however removing the "humming" of motors would be the main challenge. Specific audio pitch range elimination or Neural Net approach from drone training data could be used.
- **Design Upgrades:** Enclosed propellers, smaller or larger frame for increased payload capacity or more portable options, and more aesthetic/functional enclosure.


---

## **Components Used**
- **Frame:** DJI Phantom 3
- **Companion Computer:** RaspberryPI 4
- **Flight Controller:** Pixhawk 6c (Holybro)
- **Telemetry:** MAV link (Holybro)
- **Ground Control:** Mission Planner or Q Ground Control
- **Camera:** OAK D Lite Stereo/RGB (Luxonis)

---

## **Setup & Installation**
Intro to Autonomous Drones [Quickstart](https://docs.px4.io/main/en/getting_started/px4_basic_concepts.html)
1. **Frame Setup:** The DJI 450 frame works well, but I used a gutted DJI Phantom 3 Frame for this build.
2. **Pixhawk/Motor Setup:** Install the Pixhawk 6c Mini, Power Distribution Board, ESC's, Motors, and wiring using [these instructions](https://docs.px4.io/main/en/assembly/quick_start_pixhawk4_mini.html) or [these](https://docs.px4.io/main/en/frames_multicopter/holybro_x500v2_pixhawk6c.html) as they are similar to the Pixhawk 6c Mini.
3. **RC Setup:** There are several RC configurations, but I used the Spektrum RC with a satellite receiver for this build.
4. **RaspberryPI Configuration:** Set up the RaspberryPI as the companion computer following [this guide](https://docs.px4.io/main/en/companion_computer/pixhawk_rpi.html) (I use a direct USB connection instead of RPi GPIO connection)
5. **Camera Integration:** Attach the OAK D Lite Stereo/RGB camera. Detailed guide available [here](https://core-electronics.com.au/guides/oak-d-lite-raspberry-pi/).
6. **Software Installation:** Install Arducopter and configure using either Mission Planner or Q Ground Control. Links & resources are provided below.
[Mission Planner](https://ardupilot.org/planner/docs/mission-planner-installation.html), [Ardupilot Firmware](https://ardupilot.org/planner/docs/common-loading-firmware-onto-pixhawk.html#), or [PX4 Firmware](https://docs.qgroundcontrol.com/master/en/SetupView/Firmware.html)
---

## **Media Gallery**
Here, you'll find images and videos showcasing the drone in action. (Some have the old frame, but otherwise the same)

(Internal Hardware)

https://github.com/tmcgirr/Drone/assets/59525360/252a8ae9-4326-4792-939d-a1d9551b855d

(Telemetry Testing with Mission Planner Ground Control)

https://github.com/tmcgirr/Drone/assets/59525360/414a9271-e654-4dc4-bc48-efa45ea9c846



---

## **Links & Resources**
- **Hardware Links:**
  - DJI Frame (Phantom 3)
  - [Pixhawk 6c Mini](https://holybro.com/collections/autopilot-flight-controllers/products/pixhawk-6c-mini)
  - [OAK D Lite Camera](https://shop.luxonis.com/collections/home-page/products/oak-d-lite-1?variant=42583102456031)
- **Open Source Software:**
  - [Arducopter](https://ardupilot.org/copter/)
  - [Mission Planner](https://github.com/ArduPilot/MissionPlanner)
  - [Q Ground Control](https://docs.qgroundcontrol.com/master/en/)

---

## **Contributing**
I value your contributions and input! Whether it's improving code, adding new features, or reporting bugs - every bit helps. For contribution guidelines, please comment or feel free to send a message

---

Thank you for being a part of my journey into autonomous flight! 🚁💡
