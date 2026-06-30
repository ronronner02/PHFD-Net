# Complexity Profile

| Method | Params (M) | MACs (G) | FLOPs (G) | FPS | Latency (ms) |
|---|---:|---:|---:|---:|---:|
| AOD-Net | 0.002 | 0.11 | 0.23 | 3608.88 | 0.28 |
| FFA-Net | 4.456 | 287.28 | 574.56 | 38.83 | 25.75 |
| MSBDN-DFF | 31.353 | 24.43 | 48.87 | 100.72 | 9.93 |
| DehazeFormer-S | 1.285 | 11.92 | 23.83 | 69.43 | 14.40 |
| DehazeFormer-B | 2.518 | 23.36 | 46.71 | 39.66 | 25.21 |
| MixDehazeNet-S | 3.165 | 28.46 | 56.92 | 98.54 | 10.15 |
| MixDehazeNet-L | 12.417 | 111.85 | 223.71 | 28.51 | 35.07 |
| ConvIR-base | 8.631 | 67.71 | 135.42 | 57.21 | 17.48 |
| SFMN | 3.428 | 17.31 | 34.61 | 39.62 | 25.24 |
| DEA-Net | 3.653 | 32.22 | 64.45 | 164.81 | 6.07 |
| PHFD-Net | 4.744 | 35.87 | 71.74 | 65.42 | 15.29 |

MACs are counted using lightweight forward hooks over Conv2d, ConvTranspose2d, and Linear layers.
Attention matrix multiplication, FFT, interpolation, normalization, activations, and some functional/custom operations may not be fully counted.
Latency and FPS are therefore the primary runtime indicators.
