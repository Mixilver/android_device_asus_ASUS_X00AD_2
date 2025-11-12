## Device configuration for Asus Zenfone Go ZB500KL (ASUS_X00AD_2)

### Build Instructions
```bash
# Initialize repo
mkdir lineage-13.0 && cd lineage-13.0
repo init -u https://github.com/LineageOS/android.git -b cm-13.0

# Create local manifests folder
mkdir -p .repo/local_manifests

# Download roomservice.xml
curl https://raw.githubusercontent.com/Mixilver/android_device_asus_ASUS_X00AD_2/cm-13.0/roomservice.xml \
    -o .repo/local_manifests/roomservice.xml

# Sync source
repo sync
# or
# repo sync -c -j$(nproc) --force-sync --no-clone-bundle --no-tags --prune --optimized-fetch

# Start build
. build/envsetup.sh  
breakfast ASUS_X00AD_2 && brunch ASUS_X00AD_2
```
### Spec Sheet
| Feature                 | Specification                       |
| :---------------------- | :--------------------------------   |
| CPU                     | Quad-core 1/1.2 GHz ARM® Cortex™ A53|
| Chipset                 | Qualcomm Snapdragon 410 (MSM8916)   |
| GPU                     | Adreno 306                          |
| Memory                  | 2 GB                                |
| Shipped Android Version | 6.0.1                               |
| Storage                 | 16/32 GB                            |
| MicroSD                 | Up to 128 GB                        |
| Battery                 | 2660 (2600) mAh (removable)         |
| Dimensions              | 143.7 x 70.85 x 11.25 mm            |
| Display                 | 720 x 1280 pixels, 5.0" IPS LCD     |
| Rear Camera             | 13 MP, LED flash                    |
| Front Camera            | 5 MP                                |

### Device Picture
![Zenfone Go](https://mcgrp.ru/images/1288969/3134746.png "Zenfone Go")
