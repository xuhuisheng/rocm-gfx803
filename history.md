
# history

## ROCm-5.1.0

|OS            |linux|Python|ROCm |GPU  |
|--------------|-----|------|-----|-----|
|Ubuntu-20.04.4|5.13 |3.8.10|5.1.0|RX580|

<https://github.com/xuhuisheng/rocm-gfx803/releases/tag/rocm510>

Install ROCm First <https://docs.amd.com/bundle/ROCm_Installation_Guide-v5.1/page/Overview_of_ROCm_Installation_Methods.html>

|component  |version   |size   |link|
|-----------|----------|-------|----|
|rocblas    |2.43.0    |9.8M   |<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm510/rocblas_2.43.0-490c4140.dirty_amd64.deb>|
|pytorch    |1.11.0-rc2|145.14M|<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm500/torch-1.11.0a0+git503a092-cp38-cp38-linux_x86_64.whl>
|torchvision|0.12.0-rc1|18.47M |<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm500/torchvision-0.12.0a0+2662797-cp38-cp38-linux_x86_64.whl>
|tensorflow |2.8.0     |300.22M|<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm500/tensorflow_rocm-2.8.0-cp38-cp38-linux_x86_64.whl>|

1. Install ROCm-5.1.0
2. `sudo dpkg -i rocblas_2.43.0-490c4140.dirty_amd64.deb`
3. `pip3 install torch-1.11.0a0+git503a092-cp38-cp38-linux_x86_64.whl`
4. `pip3 install torchvision-0.12.0a0+2662797-cp38-cp38-linux_x86_64.whl`
5. `pip3 install tensorflow_rocm-2.8.0-cp38-cp38-linux_x86_64.whl`

PS: You may need `export LD_LIBRARY_PATH=/opt/rocm/lib` to resolve cannot find libmiopen.so error.

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

## ROCm-4.5.2

|OS            |linux|Python|ROCm |GPU  |
|--------------|-----|------|-----|-----|
|Ubuntu-20.04.3|5.11 |3.8.10|4.5.2|RX580|

<https://github.com/xuhuisheng/rocm-gfx803/releases/tag/rocm452>

Install ROCm First <https://rocmdocs.amd.com/en/latest/Installation_Guide/Installation-Guide.html#ubuntu>

|component  |version|size |link|
|-----------|-------|-----|----|
|rocblas    |2.41.0 |11.7M|<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm452/rocblas_2.41.0-337552f0.dirty_amd64.deb>|
|pytorch    |1.9.0  |206M |<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm43/torch-1.9.0a0+gitd69c22d-cp38-cp38-linux_x86_64.whl>|
|torchvision|0.10.0 |21M  |<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm43/torchvision-0.10.0a0+300a8a4-cp38-cp38-linux_x86_64.whl>|
|tensorflow |2.6.0  |284M |<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm43/tensorflow-2.6.0-cp38-cp38-linux_x86_64.whl>|

1. `sudo apt install rocm-dkms rocm-libs`
2. `sudo dpkg -i rocblas_2.41.0-337552f0.dirty_amd64.deb`
3. `pip3 install torch-1.9.0a0+gitd69c22d-cp38-cp38-linux_x86_64.whl`
4. `pip3 install torchvision-0.10.0a0+300a8a4-cp38-cp38-linux_x86_64.whl`
5. `pip3 install tensorflow-2.6.0-cp38-cp38-linux_x86_64.whl`

## ROCm-4.5.0

|OS            |linux|Python|ROCm |GPU  |
|--------------|-----|------|-----|-----|
|Ubuntu-20.04.3|5.11 |3.8.10|4.5.0|RX580|

<https://github.com/xuhuisheng/rocm-gfx803/releases/tag/rocm450>

Install ROCm First <https://rocmdocs.amd.com/en/latest/Installation_Guide/Installation-Guide.html#ubuntu>

|component  |version|size |link|
|-----------|-------|-----|----|
|rocblas    |2.41.0 |11.7M|<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm450/rocblas_2.41.0-337552f0.dirty_amd64.deb>|
|pytorch    |1.9.0  |206M |<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm43/torch-1.9.0a0+gitd69c22d-cp38-cp38-linux_x86_64.whl>|
|torchvision|0.10.0 |21M  |<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm43/torchvision-0.10.0a0+300a8a4-cp38-cp38-linux_x86_64.whl>|
|tensorflow |2.6.0  |284M |<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm43/tensorflow-2.6.0-cp38-cp38-linux_x86_64.whl>|

1. `sudo apt install rocm-dkms rocm-libs`
2. `sudo dpkg -i rocblas_2.41.0-337552f0.dirty_amd64.deb`
3. `pip3 install torch-1.9.0a0+gitd69c22d-cp38-cp38-linux_x86_64.whl`
4. `pip3 install torchvision-0.10.0a0+300a8a4-cp38-cp38-linux_x86_64.whl`
5. `pip3 install tensorflow-2.6.0-cp38-cp38-linux_x86_64.whl`

## ROCm-4.3.1

|OS            |linux|Python|ROCm |GPU  |
|--------------|-----|------|-----|-----|
|Ubuntu-20.04.2|5.11 |3.8.10|4.3.1|RX580|

<https://github.com/xuhuisheng/rocm-gfx803/releases/tag/rocm43>

Install ROCm First <https://rocmdocs.amd.com/en/latest/Installation_Guide/Installation-Guide.html#ubuntu>

|component  |version|size|link|
|-----------|-------|----|----|
|rocblas    |2.39.0 |7.4M|<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm43/rocblas_2.39.0-8328dcce.dirty_amd64.deb>|
|pytorch    |1.9.0  |206M|<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm43/torch-1.9.0a0+gitd69c22d-cp38-cp38-linux_x86_64.whl>|
|torchvision|0.10.0 |21M |<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm43/torchvision-0.10.0a0+300a8a4-cp38-cp38-linux_x86_64.whl>|
|tensorflow |2.6.0  |284M|<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm43/tensorflow-2.6.0-cp38-cp38-linux_x86_64.whl>|

1. `sudo apt install rocm-dkms rocm-libs`
2. `sudo dpkg -i rocblas_2.39.0-8328dcce.dirty_amd64.deb`
3. `pip3 install torch-1.9.0a0+gitd69c22d-cp38-cp38-linux_x86_64.whl`
4. `pip3 install torchvision-0.10.0a0+300a8a4-cp38-cp38-linux_x86_64.whl`
5. `pip3 install tensorflow-2.6.0-cp38-cp38-linux_x86_64.whl`

## ROCm-4.2.0

|OS            |linux|Python|ROCm |GPU  |
|--------------|-----|------|-----|-----|
|Ubuntu-20.04.2|5.4  |3.8.5 |4.2.0|RX580|

<https://github.com/xuhuisheng/rocm-gfx803/releases/tag/rocm42>

Install ROCm First <https://rocmdocs.amd.com/en/latest/Installation_Guide/Installation-Guide.html#ubuntu>

|component  |version|size|link|
|-----------|-------|----|----|
|pytorch    |1.8.1  |189M|<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm41/torch-1.8.0a0+56b43f4-cp38-cp38-linux_x86_64.whl>|
|torchvision|0.9.1  |19M |<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm41/torchvision-0.9.0a0+8fb5838-cp38-cp38-linux_x86_64.whl>|
|rocblas    |2.38.0 |7.3M|<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm42/rocblas_2.38.0-1d398335.dirty_amd64.deb>|
|rocrand    |2.10.9 |5.1M|<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm42/rocrand_2.10.9-220a6ff_amd64.deb>|
|miopen     |2.11.0 |73M |<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm42/miopen-hip_2.11.0-dd38ed4f7.dirty_amd64.deb>|

1. `sudo apt install rocm-dkms rocm-libs`
2. `sudo dpkg -i rocblas_2.38.0-1d398335.dirty_amd64.deb`
3. `sudo dpkg -i rocrand_2.10.9-220a6ff_amd64.deb`
3. `sudo dpkg -i miopen-hip_2.11.0-dd38ed4f7.dirty_amd64.deb`
4. `pip3 install torch-1.8.0a0+56b43f4-cp38-cp38-linux_x86_64.whl`
5. `pip3 install torchvision-0.9.0a0+8fb5838-cp38-cp38-linux_x86_64.whl`

## ROCm-4.1.1

|OS            |linux|Python|ROCm |GPU  |
|--------------|-----|------|-----|-----|
|Ubuntu-20.04.2|5.4  |3.8.5 |4.1.1|RX580|

<https://github.com/xuhuisheng/rocm-gfx803/releases/tag/rocm41>

Install ROCm First <https://rocmdocs.amd.com/en/latest/Installation_Guide/Installation-Guide.html#ubuntu>

|component  |version|size|link|
|-----------|-------|----|----|
|pytorch    |1.8.1  |189M|<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm41/torch-1.8.0a0+56b43f4-cp38-cp38-linux_x86_64.whl>|
|torchvision|0.9.1  |19M |<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm41/torchvision-0.9.0a0+8fb5838-cp38-cp38-linux_x86_64.whl>|
|rocblas    |2.36.0 |7M  |<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm41/rocblas_2.36.0-93c82939_amd64.deb>|
|rocrand    |2.10.7 |5.1M|<https://github.com/xuhuisheng/rocm-gfx803/releases/download/rocm41/rocrand_2.10.7-c73b16d_amd64.deb>|

1. `sudo apt install rocm-dkms rocm-libs`
2. `sudo dpkg -i rocblas_2.36.0-93c82939_amd64.deb`
3. `sudo dpkg -i rocrand_2.10.7-c73b16d_amd64.deb`
4. `pip3 install torch-1.8.0a0+56b43f4-cp38-cp38-linux_x86_64.whl`
5. `pip3 install torchvision-0.9.0a0+8fb5838-cp38-cp38-linux_x86_64.whl`

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

