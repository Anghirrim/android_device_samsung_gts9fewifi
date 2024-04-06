# TWRP Device Tree for Samsung Galaxy Tab S9 FE Wifi (SM-X510)

The Galaxy Tab S9 FE Wifi (codenamed _"gts9fewifi"_) is an upper-mid-range tablet from Samsung.

It was announced and released in October 2023.

## Device specifications

| Feature                      | Specification                                                                  |
| ---------------------------: | :----------------------------------------------------------------------------- |
| Chipset                      | Exynos 1380                                                                    |
| CPU                          | Octa-core (4x2.4 GHz Cortex-A78 & 4x2.0 GHz Cortex-A55)                        |
| GPU                          | Mali-G68 MP5                                                                   |
| Memory                       | 6GB / 8GB RAM (LPDDR4X)                                                        |
| Shipped OS                   | Android 13 (One UI 5.1)                                                        |
| Storage                      | 128GB / 256GB (UFS 2.2)                                                        |
| MicroSD                      | microSDXC                                                                      |
| Battery                      | Li-Po 8000 mAh (non-removable), 45W wired, QC2.0                               |
| Dimensions                   | 254.3 x 165.8 x 6.5 mm (10.01 x 6.53 x 0.26 in)                                |
| Display                      | 10.9", 1440 x 2304 pixels, 16:10 ratio, IPS LCD, 90Hz (~249 ppi density)       |
| Rear Camera                  | 8 MP, (wide), Video 	4K@30fps, 1080p@30fps                                     |
| Front Camera                 | 12 MP, (ultrawide)                                                             |
| Fingerprint                  | Yes, side mounted                                                              |
| Sensors                      | Accelerometer, gyro, compass, proximity (accessories only)                     |
| Positioning                  | GPS, GALILEO, GLONASS, BDS, QZSS                                               |
| Extras                       | IP68 dust/water resistant, Stereo speakers tuned by AKG, USB-C 2.0             |

## Kernel source 

Available at [https://github.com/BlackMesa123/android_kernel_samsung_s5e8835/tree/sep-15/twrp-12.1](https://github.com/BlackMesa123/android_kernel_samsung_s5e8835/tree/sep-15/twrp-12.1)

## How to build

This device tree was tested and is fully compatible with [minimal-manifest-twrp](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp).

1. Set up the build environment following the instructions [here](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp/blob/twrp-12.1/README.md#getting-started)

2. In the root folder of the fetched repo, clone the device tree:

```bash
git clone https://github.com/TeamWin/android_device_samsung_a54x.git -b android-12.1 device/samsung/gts9fewifi
```

3. To build:

```bash
export ALLOW_MISSING_DEPENDENCIES=true
. build/envsetup.sh
lunch twrp_gts9fewifi-eng
mka recoveryimage
```

## Copyright

```
#
# Copyright (C) 2024 The TWRP Open Source Project
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#
```
