
# ROCm with gfx803

This repo upload some archieves for ROCm with gfx803 after ROCm-4.0.

<https://github.com/xuhuisheng/rocm-build/tree/master/gfx803>

## ROCm-4.5.0

|OS            |linux|Python|ROCm |GPU  |
|--------------|-----|------|-----|-----|
|Ubuntu-20.04.3|5.11 |3.8.10|4.5.0|RX580|

<https://github.com/xuhuisheng/rocm-gfx803/releases/tag/rocm450>

Install ROCm First <https://rocmdocs.amd.com/en/latest/Installation_Guide/Installation-Guide.html#ubuntu>

|component  |version|size |link|
|-----------|-------|-----|----|
|rocblas    |2.41.0 |11.7M|<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm450/rocblas_2.41.0-337552f0~dirty_amd64.deb>|
|pytorch    |1.9.0  |206M |<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm43/torch-1.9.0a0+gitd69c22d-cp38-cp38-linux_x86_64.whl>|
|torchvision|0.10.0 |21M  |<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm43/torchvision-0.10.0a0+300a8a4-cp38-cp38-linux_x86_64.whl>|
|tensorflow |2.6.0  |284M |<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm43/tensorflow-2.6.0-cp38-cp38-linux_x86_64.whl>|

1. `sudo apt install rocm-dkms rocm-libs`
2. `sudo dpkg -i rocblas_2.41.0-337552f0~dirty_amd64.deb`
3. `pip3 install torch-1.9.0a0+gitd69c22d-cp38-cp38-linux_x86_64.whl`
4. `pip3 install torchvision-0.10.0a0+300a8a4-cp38-cp38-linux_x86_64.whl`
5. `pip3 install tensorflow-2.6.0-cp38-cp38-linux_x86_64.whl`

## ROCm-3.5.1

|OS            |linux|Python|ROCm |GPU  |
|--------------|-----|------|-----|-----|
|Ubuntu-20.04  |5.4  |3.8.5 |3.5.1|RX580|

<https://github.com/xuhuisheng/rocm-gfx803/releases/tag/rocm35>

Install ROCm-3.5.1 First <https://github.com/boriswinner/RX580-rocM-tensorflow-ubuntu20.4-guide>

|component  |version|size|link|
|-----------|-------|----|----|
|pytorch    |1.7.0  |173M|<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm35/torch-1.7.0a0-cp38-cp38-linux_x86_64.whl>|
|torchvision|0.8.0  |6.4M|<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm35/torchvision-0.8.0a0+2f40a48-cp38-cp38-linux_x86_64.whl>|

1. `sudo apt install rocm-dkms rocm-libs`
2. `export LB_LIBRARY_PATH=$LD_LIBRARY_PATH:/opt/rocm/hip/lib`
3. `pip3 install torch-1.7.0a0-cp38-cp38-linux_x86_64.whl`
4. `pip3 install torchvision-0.8.0a0+2f40a48-cp38-cp38-linux_x86_64.whl`

