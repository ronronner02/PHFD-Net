# Quantitative Results

PSNR / SSIM are reported for each benchmark.

| Method | Params (M) | SOTS-Indoor | Haze4K | SOTS-Outdoor |
|---|---:|---:|---:|---:|
| DCP | - | 16.61 / 0.855 | - | 19.14 / 0.861 |
| AOD-Net | - | 20.51 / 0.816 | - | 24.14 / 0.920 |
| GridDehazeNet | - | 32.16 / 0.984 | 23.29 / 0.930 | 30.86 / 0.982 |
| FFA-Net | - | 36.59 / 0.989 | 26.96 / 0.950 | 33.57 / 0.984 |
| MSBDN | - | 32.77 / 0.981 | 22.99 / 0.850 | 34.81 / 0.986 |
| AECR-Net | - | 37.17 / 0.990 | - | - |
| DehazeFormer-M | - | 38.46 / 0.994 | - | 34.29 / 0.983 |
| DEA-Net-CR | - | 41.31 / 0.995 | 34.25 / 0.989 | 36.59 / 0.990 |
| MixDehazeNet | - | 42.62 / 0.997 | 35.64 / 0.992 | 36.50 / 0.986 |
| SFMN | - | 41.44 / 0.995 | - | 37.72 / 0.991 |
| SAD-Net | - | 41.71 / 0.993 | - | 37.78 / 0.990 |
| WDMamba | - | - | 35.88 / 0.991 | - |
| SEMN | - | 41.46 / 0.995 | - | 37.60 / 0.991 |
| PHFD-Net | 4.744 | 42.35 / 0.995 | 34.94 / 0.990 | 36.58 / 0.990 |
| PHFD-Net-FT | 4.744 | - | 38.537 / 0.99371 | 38.364 / 0.99095 |

PHFD-Net denotes the standard matched/scratch setting.
PHFD-Net-FT denotes target-domain fine-tuning initialized from the SOTS-Indoor checkpoint.
Fine-tuning results should not be interpreted as scratch or matched baseline comparisons.
