# FusionX-Visualization

Dual Glove + OAK Camera Dashboard — real-time tactile sensor visualization and IMU tracking.

## Download

Grab the latest release from the [Releases](https://github.com/TouchTronix-Robotics/FusionX-Visualization/releases) page:

- **Linux**: `.AppImage` — make it executable and run
- **Windows**: `.zip` — extract and run `touchtronix-demo.exe`

## Linux Setup

### OAK Camera USB Permissions

The OAK camera requires udev rules to access USB devices without root.
Run the following **once** after first install:

```bash
sudo wget -qO- https://raw.githubusercontent.com/luxonis/depthai-python/main/docs/install_depthai.sh | sudo bash
```

Then replug the OAK camera. No reboot required.

### AppImage

Make the AppImage executable:

```bash
chmod +x touchtronix-demo-*.AppImage
./touchtronix-demo-*.AppImage
```

If the app doesn't launch, your system may need FUSE2:

```bash
# Ubuntu 24.04+
sudo apt install libfuse2t64

# Ubuntu 22.04 or older
sudo apt install libfuse2
```

## Windows Setup

No additional setup required — just extract the zip and run `touchtronix-demo.exe`.
The OAK camera drivers are included automatically.
