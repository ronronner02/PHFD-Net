# Dataset Protocol

PHFD-Net is evaluated on SOTS-Indoor, Haze4K, and SOTS-Outdoor.

## SOTS-Indoor

SOTS-Indoor is used for indoor dehazing evaluation under the RESIDE indoor
protocol. The matched setting trains on the corresponding indoor training split and
evaluates on the SOTS-Indoor test/validation protocol used in the paper.

## Haze4K

Haze4K is used for synthetic dehazing evaluation. The standard PHFD-Net row reports
the matched/scratch Haze4K setting. The PHFD-Net-FT row reports target-domain
fine-tuning initialized from the SOTS-Indoor checkpoint.

## SOTS-Outdoor

SOTS-Outdoor is used for outdoor dehazing evaluation under the outdoor RESIDE
protocol. Outdoor results are reported separately from indoor and Haze4K results
because data generation, haze density, and image-compression properties differ. The
matched SOTS-Outdoor number follows the Pillow 8.3.2 JPEG decoding protocol used for
the paper table.

## Protocol Types

- **Matched**: training and evaluation follow the same target benchmark protocol.
- **Scratch**: the target benchmark is trained without using another target-domain
  checkpoint as initialization.
- **Fine-tuning**: target-domain training is initialized from a checkpoint trained
  on another dataset.
- **Zero-shot qualitative**: real-haze examples are used only for visual inspection,
  not for full-reference quantitative comparison.

The public datasets above are available from their original sources; local dataset
paths are not part of this repository.
