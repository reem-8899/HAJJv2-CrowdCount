# HAJJv2-CrowdCount Annotation Protocol

## Overview

This document describes the annotation protocol used to generate the frame level crowd count annotations released with the HAJJv2-CrowdCount benchmark.

The objective of the annotation process is to provide reliable and reproducible ground truth crowd counts for evaluating crowd counting algorithms under challenging Hajj surveillance conditions.

Frames were extracted from each video at a fixed sampling rate of **1 frame per second (1 FPS)** and manually annotated by human annotators.

---

# Annotation Protocols

The dataset contains annotations generated using two protocols.

## Protocol A – Independent Manual Annotation

Independent manual annotation was adopted as the primary annotation protocol.

For each sampled frame:

1. The frame was opened independently.
2. No detector predictions or model outputs were shown to the annotator.
3. The annotator manually counted all valid individuals.
4. The final count was recorded as the ground truth.

Every frame was counted twice by the same annotator.

If the two counting passes produced different totals, the frame was manually reexamined until a final verified count was obtained.

---

## Protocol B – Model-Assisted Annotation

TBC

---

# Frame Sampling

Videos were sampled uniformly at:

- Sampling rate: **1 FPS**

Each sampled frame corresponds to a single annotation.

---

# Ground Truth Definition

Ground truth represents the total number of valid people visible in the image according to the annotation guidelines.

Only verified human counts are released.

---

# Quality Assurance

Each frame underwent a verification process before publication.

Quality assurance consisted of:

- Double manual counting
- Manual verification of disagreements
- Consistent application of annotation rules
- Protocol tracking for every annotated video

---

# Public Release

The released dataset contains only the verified crowd count annotations.

Intermediate detector predictions, correction values, and annotation drafts are intentionally excluded from the public release.