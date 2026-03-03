# ConvIR-Based-Structure-Oriented-Restoration-for-Small-AreaWet-Fingerprint-Recognition
⚠ This repository only provides pretrained weights.
The full implementation is available at the official CycleGAN repository.

# CycleGAN Models for Small Area Wet Fingerprint Generation

This repository provides the pretrained CycleGAN models used in our CVPR Workshop paper:

"Structure-Oriented ConvIR and CycleGAN Benchmarking for Small-Area Wet Fingerprints"

---

## Overview

We adopt the official PyTorch implementation of CycleGAN:

👉 https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix

We do **not modify the architecture** or training framework.
The original implementation is used directly.

This repository only contains two pretrained models used for public wet fingerprint benchmark generation.

---

## Provided Models

Two CycleGAN checkpoints are provided:

1. origin2clear  
   - Transforms original fingerprint patches into sensor-style dry fingerprints.
   - Used to unify sensor appearance.

2. clear2hazy  
   - Transforms clear fingerprints into simulated wet fingerprints.
   - Used to generate wet degradation patterns.

These models are trained on the private training split of n9395_1023_v1 only.

---

## How to Use

To use the models, please clone the official CycleGAN repository:

https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix

Then place the provided checkpoints under:

    checkpoints/{model_name}/

and follow the standard testing procedure from the official implementation.

---

## Acknowledgement

We sincerely thank the authors of CycleGAN for making their implementation publicly available.

If you use these models, please also cite:

@inproceedings{CycleGAN2017,
  title={Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks},
  author={Zhu, Jun-Yan and Park, Taesung and Isola, Phillip and Efros, Alexei A},
  booktitle={Computer Vision (ICCV), 2017 IEEE International Conference on},
  year={2017}
}

@inproceedings{isola2017image,
  title={Image-to-Image Translation with Conditional Adversarial Networks},
  author={Isola, Phillip and Zhu, Jun-Yan and Zhou, Tinghui and Efros, Alexei A},
  booktitle={Computer Vision and Pattern Recognition (CVPR), 2017 IEEE Conference on},
  year={2017}
}

CycleGAN code: https://drive.google.com/drive/folders/1hnB0tfAXoUJmXm9OzTD33nlLZU2GqJio
code: https://drive.google.com/drive/folders/1ub9c9KTLWB_Jz0Wc0nLUGnmdydyySbe4?usp=drive_link
Dataset: https://drive.google.com/file/d/1uH6NoXNtZZ7AyBSgPOBN3kjk8SQl6mIn/view?usp=drivesdk
