# Quantitative Results

PSNR / SSIM are reported for each benchmark. Parameter counts are the deploy-time
(re-parameterized) inference model.

| Method | Params (M) | SOTS-Indoor | Haze4K | SOTS-Outdoor |
|---|---:|---:|---:|---:|
| DCP | - | 16.61 / 0.855 | - | 19.14 / 0.861 |
| AOD-Net | 0.002 | 20.51 / 0.816 | - | 24.14 / 0.920 |
| GridDehazeNet | 0.960 | 32.16 / 0.984 | 23.29 / 0.930 | 30.86 / 0.982 |
| FFA-Net | 4.456 | 36.59 / 0.989 | 26.96 / 0.950 | 33.57 / 0.984 |
| MSBDN | 31.35 | 32.77 / 0.981 | 22.99 / 0.850 | 34.81 / 0.986 |
| AECR-Net | 2.611 | 37.17 / 0.990 | - | - |
| DehazeFormer-M | 4.634 | 38.46 / 0.994 | - | 34.29 / 0.983 |
| DEA-Net-CR | 3.653 | 41.31 / 0.995 | 34.25 / 0.989 | 36.59 / 0.990 |
| MixDehazeNet | 12.417 | 42.62 / 0.997 | 35.64 / 0.992 | 36.50 / 0.986 |
| SFMN | 3.424 | 41.44 / 0.995 | - | 37.72 / 0.991 |
| SAD-Net | 3.15 | 41.71 / 0.993 | - | 37.78 / 0.990 |
| WDMamba | 11.25 | - | 35.88 / 0.991 | - |
| SEMN | 3.379 | 41.46 / 0.995 | - | 37.60 / 0.991 |
| PHFD-Net | 4.744 | 42.36 / 0.995 | 34.95 / 0.990 | 36.58 / 0.990 |
| PHFD-Net-FT | 4.744 | - | 38.54 / 0.994 | 38.36 / 0.991 |

- `PHFD-Net` denotes the standard matched / scratch setting.
- `PHFD-Net-FT` denotes target-domain fine-tuning initialized from the SOTS-Indoor
  checkpoint. Fine-tuning results should not be interpreted as scratch or matched
  baseline comparisons.
- The SOTS-Outdoor number follows the Pillow 8.3.2 JPEG decoding protocol; see
  [../docs/evaluation_protocol.md](../docs/evaluation_protocol.md).
