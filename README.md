# Continued self-supervised pretraining of DINO and DINOv2 on endoscopic data for anatomical site classification of the upper gastrointestinal tract

Diploma thesis, Department of Electrical and Computer Engineering, Aristotle University of Thessaloniki (AUTh), November 2026.

- **Author:** Βασιλική Μανούση
- **Supervisor:** Λεόντιος Χατζηλεοντιάδης
- **Supervising PhD candidate:** Γιώργος Αποστολίδης

## Contents

| File | Description |
| --- | --- |
| [`thesis.pdf`](thesis.pdf) | Full thesis text (in Greek, with an English abstract) |
| [`presentation.pdf`](presentation.pdf) | Defence presentation slides (in Greek) |

## Abstract

Accurate recognition of the anatomical site in endoscopic images of the upper gastrointestinal tract is a key building block of computer-aided gastroscopy systems, yet annotated data remain scarce. The self-supervised models DINO and DINOv2 are pretrained on large, general-purpose collections of unlabeled images and have shown strong representations across many domains, but it remains unclear whether further adapting them to endoscopic data improves their performance on a specific medical task.

This thesis addresses this question on the GastroHUN anatomical site classification benchmark. First, the benchmark was reproduced for 16 reference architectures and extended with eight generic DINO/DINOv2 backbones. Then, three models (DINOv2 ViT-S/14, DINO ViT-S/16 and DINOv2 ViT-B/14) were further pretrained on 108,321 unlabeled HyperKvasir images and compared with their generic checkpoints under a fixed downstream protocol, using both a frozen backbone and partial fine-tuning, with three seeds and bootstrap confidence intervals.

In all three experiments, the domain-adapted checkpoint significantly outperforms its generic counterpart, both with a frozen backbone and after partial fine-tuning. After continued pretraining, all three models rank among the top positions of the architecture ranking, alongside the top ConvNeXt models. The results suggest that adapting to in-domain data is a practical and consistent way of improving self-supervised models in endoscopic imaging.

**Keywords:** DINO, DINOv2, self-supervised learning, continued pretraining, gastroscopy, GastroHUN, Vision Transformers, anatomical site classification

## Note

This repository contains the thesis text and presentation only. No code or datasets are included. The datasets used (GastroHUN, HyperKvasir) are distributed by their respective authors under their own terms.
