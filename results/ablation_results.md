# Ablation Results

| Variant | Routing | SFBlock | PSNR | SSIM |
|---|:---:|:---:|---:|---:|
| Baseline | x | x | 40.7928 | 0.9940 |
| +PreRoute-Spatial | yes | x | 40.9346 | 0.9940 |
| +SFBlock | x | yes | 41.0962 | 0.9941 |
| PHFD-Net | yes | yes | 41.1259 | 0.9941 |

These are controlled 100-epoch ablation runs on ITS, evaluated on the SOTS-Indoor
validation protocol. They are reported separately from the fully trained main
comparison and should not be mixed with it.
