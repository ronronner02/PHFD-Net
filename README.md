# PHFD-Net: A Locally Re-parameterized Hierarchical Spatial-Frequency Network for Single Image Dehazing

Project page for **PHFD-Net**. The paper is currently under review at IEEE TCSVT.

This repository shares paper-level information — method overview, results, figures,
and evaluation-protocol notes. **Source code, pretrained models, and evaluation
scripts will be released upon acceptance** (see [docs/release_plan.md](docs/release_plan.md)).

![PHFD-Net teaser](assets/teaser.png)

## Overview

PHFD-Net is a hierarchical single-image dehazing network that combines local
detail-enhanced restoration, deep-state residual routing, and a spatial-frequency
bottleneck. Local branches are re-parameterizable, so the deployed model runs as a
compact single-branch graph (4.74 M parameters) without changing its outputs.

## Method

- local detail-enhanced restoration;
- deep-state history residual routing (PreRoute-SF);
- spatial-frequency bottleneck refinement;
- local-branch re-parameterization for efficient deployment.

![PHFD-Net framework](assets/framework.png)

## Results

- Benchmark comparison: [results/quantitative_results.md](results/quantitative_results.md)
- Ablation study: [results/ablation_results.md](results/ablation_results.md)
- Complexity and speed: [results/complexity_profile.md](results/complexity_profile.md)

![Qualitative comparison](assets/qualitative_comparison.png)

## Datasets and evaluation protocol

- [docs/dataset_protocol.md](docs/dataset_protocol.md)
- [docs/evaluation_protocol.md](docs/evaluation_protocol.md)

Benchmarks: SOTS-Indoor, Haze4K, and SOTS-Outdoor. Fine-tuned results are reported
separately from matched/scratch comparisons. The SOTS-Outdoor row uses the
Pillow 8.3.2 JPEG decoding protocol.

## Release plan

See [docs/release_plan.md](docs/release_plan.md). Code and pretrained models will be
released after the paper is accepted.

## Citation

The bibliographic information will be updated once the paper is published. See
[CITATION.cff](CITATION.cff).

## License

Released under the [MIT License](LICENSE).
