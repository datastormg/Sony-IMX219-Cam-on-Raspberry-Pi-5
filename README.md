# Sony-IMX219-Cam-on-Raspberry-Pi-5
Configuring  Sony IMX219 Cam on Raspberry Pi 5


## Raspberry Pi 5 – IMX219 Camera Setup (Bookworm)

This guide explains how to connect and configure an **IMX219** camera on the **Raspberry Pi 5** running Raspberry Pi OS **Bookworm**, using the new `rpicam-apps` instead of the legacy `libcamera-*` commands.

---

###  Requirements

- **Raspberry Pi 5**
- **IMX219 camera module** (e.g., Raspberry Pi Camera v2)
- Correct **FPC cable** for Pi 5:
  - Pi 5 uses **22-pin, 0.5 mm pitch** CSI connectors.
  - If your camera has the standard **15-pin** connector, use a **22↔15-pin adapter cable**.
- Raspberry Pi OS **Bookworm** (2023+)
- Internet connection

---

### 🔌 Physical Connection

1. **Power off** the Raspberry Pi.
2. Identify the camera port (**CAM0** or **CAM1**).
3. Insert the 22-pin cable into the Pi’s CSI port:
   - Copper contacts **facing the board**.
4. Insert the other end into the camera module:
   - For 15-pin cameras, copper contacts usually **face the lens**.
5. Secure the connectors by pressing down the locking tab.

---

### ⚙️ Configuration

Open the firmware config file and follow the steps in the codes files
   
   sudo nano /boot/firmware/config.txt

   https://forums.raspberrypi.com/viewtopic.php?t=371121
