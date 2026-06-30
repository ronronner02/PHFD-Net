# Evaluation Protocol

PSNR and SSIM are full-reference metrics computed between the restored image and
the corresponding ground-truth clear image.

PHFD-Net-FT denotes target-domain fine-tuning. It should not be mixed with
scratch or matched baseline comparisons, because the initialization protocol is
different.

Real-haze visualization only supports qualitative inspection. Real-haze images
without paired ground truth are not used for PSNR or SSIM comparison.

Outdoor evaluation can be sensitive to JPEG decoding and image-loading details.
When comparing against protocol-specific outdoor results, the evaluation
environment and preprocessing rules should be matched.
