# Evaluation Protocol

PSNR and SSIM are full-reference metrics computed between the restored image and the
corresponding ground-truth clear image.

`PHFD-Net-FT` denotes target-domain fine-tuning initialized from the SOTS-Indoor
checkpoint. It should not be mixed with scratch or matched baseline comparisons,
because the initialization protocol is different.

Real-haze visualization only supports qualitative inspection. Real-haze images
without paired ground truth are not used for PSNR or SSIM comparison.

SOTS-Outdoor evaluation can be sensitive to JPEG decoding and image-loading details
because the hazy inputs are JPEG images. The reported matched SOTS-Outdoor result
uses the Pillow 8.3.2 decoding protocol (`36.58 / 0.990`).
