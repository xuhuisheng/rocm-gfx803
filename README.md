
# ROCm with gfx803

This repo upload some archieves for ROCm with gfx803 after ROCm-4.0.

<https://github.com/xuhuisheng/rocm-build/tree/master/gfx803>

## ROCm-5.0.0

|OS            |linux|Python|ROCm |GPU  |
|--------------|-----|------|-----|-----|
|Ubuntu-20.04.3|5.11 |3.8.10|5.0.0|RX580|

<https://github.com/xuhuisheng/rocm-gfx803/releases/tag/rocm500>

Install ROCm First <https://docs.amd.com/bundle/ROCm_Installation_Guide-v5.0/page/Overview_of_ROCm_Installation_Methods.html>

|component  |version   |size   |link|
|-----------|----------|-------|----|
|rocblas    |2.42.0    |9.71M  |<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm500/rocblas_2.42.0-60c5f03d.dirty_amd64.deb>|
|pytorch    |1.11.0-rc2|145.14M|<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm500/torch-1.11.0a0+git503a092-cp38-cp38-linux_x86_64.whl>
|torchvision|0.12.0-rc1|18.47M |<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm500/torchvision-0.12.0a0+2662797-cp38-cp38-linux_x86_64.whl>
|tensorflow |2.8.0     |300.22M|<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm500/tensorflow_rocm-2.8.0-cp38-cp38-linux_x86_64.whl>|

1. Install ROCm-5.0.0
2. `sudo dpkg -i rocblas_2.42.0-60c5f03d.dirty_amd64.deb`
3. `pip3 install torch-1.11.0a0+git503a092-cp38-cp38-linux_x86_64.whl`
4. `pip3 install torchvision-0.12.0a0+2662797-cp38-cp38-linux_x86_64.whl`
5. `pip3 install tensorflow_rocm-2.8.0-cp38-cp38-linux_x86_64.whl`

PS: I tried pytorch-1.8.2 and pytorch-1.10.2, there is a compiling error for cannot resolve chain iterator in rocPRIM. There latest pytorch-1.11.0-rc2 seems resolved this problem.

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

