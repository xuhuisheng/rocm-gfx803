
# history

## ROCm-4.2.0

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

