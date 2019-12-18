# ble113-sensors
>Wireless sensors designed in the Ong Lab at the University of Oregon.
---
## Table of Contents
1. [Getting Started](#getting-started)
1. [Usage](#usage)
1. [Projects](#projects)
1. [Contributors](#contributors)
1. [License](#license)
---
## Getting Started
The following files are provided by Silicon Labs. A Silicon Labs account is required for download, and may be created for free.
- [SDK v1.5](https://www.silabs.com/documents/login/software/Bluegiga-ble-1.5.0-137.exe) (Required)
- [Datasheet](https://www.silabs.com/documents/public/data-sheets/BLE113-DataSheet.pdf)
- [Software reference manual](https://www.silabs.com/documents/public/reference-manuals/Bluetooth_Smart_Software-BLE-1.5-API-RM.pdf)
- [Scripting guide](https://www.silabs.com/documents/public/user-guides/UG209.pdf)
- [Configuration guide](https://www.silabs.com/documents/public/user-guides/UG209.pdf)

Syntax highlighting is available in Atom by searching `language-bgscript` in the package manager.

---
## Usage

A BLE project folder should contain a `project.xml` file, which will link to a gatt file (`.xml`), a hardware file (`.xml`), and a script file (`.bgs`).

The `bgbuild.exe` executable provided in the SDK is used to build a project file into an image. A powershell function can make use of the bgbuild .exe more convenient. For example, `function bgbuild { C:\Bluegiga\ble-1.5.0-137\bin\bgbuild.exe $args }` may be used to run the program without entering the full path. Note that the install path for the SDK may differ. The project can be compiled using the syntax `bgbuild project.xml`, where project.xml is the target project file.

The image file can be flashed to the BLE113 using the [TI CC Debugger](https://www.digikey.com/product-detail/en/texas-instruments/CC-DEBUGGER/296-30207-ND/2231678) and the BLE SW Update Tool provided in the SDK. Select the `.hex` image file using the Browse button, and hit Update to flash the program to the BLE113. Note: No license key is needed.

---
## Projects

#### Bioreactor pH Sensor (`bioreactor`)

A low-cost pH sensor for use in benchtop bioreactors for cell manufacturing.

>Related Publications:
- [Nelson, B. D. (2018). A Bluetooth Low-Energy Wireless Sensor Platform for Continuous Monitoring of a Bioreactor Environment during Cell Manufacturing.](https://digitalcommons.mtu.edu/etdr/609/)

#### Georgia Tech Strain Gauge (`gt-strain`)

A telemetry platform for a strain gauge attached to a femoral fixation plate in a collaboration with Georgia Tech.

>Related Publications:
- Klosterhoff, B. S., Ghee Ong, K., Krishnan, L., Hetzendorfer, K. M., Chang, Y. H., Allen, M. G., ... & Willett, N. J. (2017). Wireless implantable sensor for noninvasive, longitudinal quantification of axial strain across rodent long bone defects. _Journal of biomechanical engineering, 139_(11), 111004.

#### Guidewire Sensor (`guidewire`)

An old project that used a pair of strain sensors to measure forces applied to a surgical guidewire.

#### Piezoelectic Fixation Plate (`piezo`)

An implantable piezoelectric fixation plate for providing strain actuation and load monitoring for fracture healing in rodents.

> Related Publications
- [Nelson, B. D. (2019). A Smart Implantable Bone Fixation Plate Providing Actuation and Load Monitoring for Orthopedic Fracture Healing.](https://digitalcommons.mtu.edu/etdr/898/)

---
## Contributors
- Brad Nelson (https://github.com/bradleydavidnelson)

---
## License
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
