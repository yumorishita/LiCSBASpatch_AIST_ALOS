# LiCSBASpatch_AIST_ALOS
Patch program for LiCSBAS to use AIST ALOS InSAR products (2006-2011)

- [InSAR Browser](https://gsrt.digiarc.aist.go.jp/insarbrowser/index.html)
- [PALSAR InSAR Terms of use](https://gsrt.digiarc.aist.go.jp/insarbrowser/doc/terms_of_use_insar_EN.html)
- [AIST ALOS/PALSAR InSAR Product Format Description](https://gsrt.digiarc.aist.go.jp/insarbrowser/doc/AIST_PALSAR_INSAR_PFFD_EN.pdf)
- [ALOS frame map](https://yumorishita.github.io/gsimaps/#6/36.670180/139.284668/&base=blank&ls=blank%7Copenstreetmap%7Cgeojson_ALOSframeA343_group%7Cgeojson_ALOSframeAothers_group%7Cgeojson_ALOSframeD343_group%7Cgeojson_ALOSframeDothers_group&blend=0&disp=111000&lcd=openstreetmap&vs=c1g1j0h0k0l0u0t0z0r0s0m0f1&d=m)

## Installation

1. [Install LiCSBAS](https://github.com/yumorishita/LiCSBAS/wiki/1_Installation)
2. `git clone https://github.com/yumorishita/LiCSBASpatch_AIST_ALOS.git`
3. `source LiCSBASpatch_AIST_ALOS/bashrc_LiCSBAS_ALOS.sh`

## How to run LiCSBAS using ALOS InSAR data

First, determine the frame ID of interest (e.g., `410_0690_343`), then
```
mkdir 410_0690_343
cd 410_0690_343
copy_batch_LiCSBAS_ALOS.sh
# Edit batch_LiCSBAS_ALOS.sh if you want
./batch_LiCSBAS_ALOS.sh
```

## ALOS InSAR data coverage

- Japan
- Phillipines
- Indonesia (except Borneo island and New Guinea island)
- Turkey
- East African Rift
- West coast of North America

![ALOSmap](https://user-images.githubusercontent.com/37470321/182858953-6190cb41-e5d6-4cf5-ba27-ea46125fa8ae.png)
