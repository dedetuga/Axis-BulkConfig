AxisDiscovery_QT
=================

Qt-based GUI tool to discover Axis devices on the network and provision users on multiple devices.

### Capabilities
- Discover AXIS devices and display them in a table.
- Select devices and provision a new user on each via AXIS `pwdgrp.cgi`, highlighting success or failure.
- Configure device settings:
  - Timezone and NTP servers
  - Orientation, capture mode and power line frequency
  - SD card status, mounting and formatting
  - Application management (list and start apps)
  - Enable full-disk encryption

### Compatibility
- Qt 5.15 or Qt 6
- Tested on Linux and Windows (no administrator privileges required on Windows)
- Targets AXIS network devices using the VAPIX HTTP API

### Windows notes (no admin required)

The application now supports Windows without requiring administrative
privileges. Networking is performed using user-mode sockets and the
necessary Winsock initialisation is handled automatically at start-up.
Build and run using standard CMake commands.


