# LiCSBASpatch_AIST_ALOS
Patch program for LiCSBAS to use AIST ALOS InSAR products (2006-2011)

- [ALOS frame map](https://yumorishita.github.io/gsimaps/#6/36.670180/139.284668/&base=blank&ls=blank%7Copenstreetmap%7Cgeojson_ALOSframeA343_group%7Cgeojson_ALOSframeAothers_group%7Cgeojson_ALOSframeD343_group%7Cgeojson_ALOSframeDothers_group&blend=0&disp=111000&lcd=openstreetmap&vs=c1g1j0h0k0l0u0t0z0r0s0m0f1&d=m)
- R. Sugimoto, M. Shimada, Y. Morishita, R. Natsuaki, C. Tsutsumi, R. Nakamura, and Y. Yamaguchi, “Interferometric SAR Processing Using Whole ALOS/PALSAR Data Archive for Measuring the Global Surface Deformation,” 2021 7th Asia-Pacific Conference on Synthetic Aperture Radar (APSAR). [https://doi.org/10.1109/APSAR52370.2021.9688342](https://doi.org/10.1109/APSAR52370.2021.9688342)
- Morishita, Y., Sugimoto, R., Nakamura, R. et al. Nationwide urban ground deformation in Japan for 15 years detected by ALOS and Sentinel-1. Prog Earth Planet Sci 10, 66 (2023). [https://doi.org/10.1186/s40645-023-00597-5](https://doi.org/10.1186/s40645-023-00597-5)
- [InSAR Browser](https://gsrt.digiarc.aist.go.jp/insarbrowser/index.html)
- [PALSAR InSAR Terms of use](https://gsrt.digiarc.aist.go.jp/insarbrowser/doc/terms_of_use_insar_EN.html)
- [AIST ALOS/PALSAR InSAR Product Format Description](https://gsrt.digiarc.aist.go.jp/insarbrowser/doc/AIST_PALSAR_INSAR_PFFD_EN.pdf)

## Installation

1. Install [LiCSBAS2](https://github.com/yumorishita/LiCSBAS2) (>=v1.9.0)
2. `git clone https://github.com/yumorishita/LiCSBASpatch_AIST_ALOS.git`
3. `source LiCSBASpatch_AIST_ALOS/bashrc_LiCSBAS_ALOS.sh`

* You can also use [LiCSBAS](https://github.com/yumorishita/LiCSBAS) instead of [LiCSBAS2](https://github.com/yumorishita/LiCSBAS2), but LiCSBAS2 is highly recommended because the DEM error correction which is important for ALOS (see [4.2 in Morishita et al., 2023](https://progearthplanetsci.springeropen.com/articles/10.1186/s40645-023-00597-5#Sec24)) is available in LiCSBAS2.

## How to run LiCSBAS using ALOS InSAR data

First, determine the frame ID of interest (e.g., `410_0690_343`), then
```
mkdir 410_0690_343
cd 410_0690_343
copy_batch_LiCSBAS2_ALOS.sh
# Edit batch_LiCSBAS2_ALOS.sh if you want
./batch_LiCSBAS2_ALOS.sh
```

## ALOS InSAR data coverage

- Japan
- Phillipines
- Indonesia (except Borneo island and New Guinea island)
- Nepal
- Turkey and NW of Iran
- East African Rift
- West coast of North America

![ALOSmap](https://github.com/yumorishita/LiCSBASpatch_AIST_ALOS/assets/37470321/32a86f13-6fda-4693-bac5-fbb423253863)


![ALOSmap](https://user-images.githubusercontent.com/37470321/182858953-6190cb41-e5d6-4cf5-ba27-ea46125fa8ae.png)
