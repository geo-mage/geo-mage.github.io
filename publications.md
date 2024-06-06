# Publications

## Cross-sensor self-supervised training and alignment for remote sensing

Authors: Valerio Marsocci, Nicolas Audebert

🔗 [arXiv](https://arxiv.org/abs/2405.09922) 🔗 [HAL](https://hal.science/hal-04576064)

**Preprint**

Large-scale "foundation models" have gained traction as a way to leverage the vast amounts of unlabeled remote sensing data collected every day. However, due to the multiplicity of Earth Observation satellites, these models should learn "sensor agnostic" representations, that generalize across sensor characteristics with minimal fine-tuning. This is complicated by data availability, as low-resolution imagery, such as Sentinel-2 and Landsat-8 data, are available in large amounts, while very high-resolution aerial or satellite data is less common. To tackle these challenges, we introduce cross-sensor self-supervised training and alignment for remote sensing (X-STARS). We design a self-supervised training loss, the Multi-Sensor Alignment Dense loss (MSAD), to align representations across sensors, even with vastly different resolutions. Our X-STARS can be applied to train models from scratch, or to adapt large models pretrained on e.g low-resolution EO data to new high-resolution sensors, in a continual pretraining framework. We collect and release MSC-France, a new multi-sensor dataset, on which we train our X-STARS models, then evaluated on seven downstream classification and segmentation tasks. We demonstrate that X-STARS outperforms the state-of-the-art by a significant margin with less data across various conditions of data availability and resolutions. 


##  Detecting Out-Of-Distribution Earth Observation Images with Diffusion Models

Authors: Georges Le Bellier, Nicolas Audebert

🔗 [arXiv](https://arxiv.org/abs/2404.12667) 🔗 [HAL](https://hal.science/hal-04551408/)

**EarthVision 2024** (CVPR workshop)
https://www.grss-ieee.org/events/earthvision-2024/

Earth Observation imagery can capture rare and unusual events, such as disasters and major landscape changes, whose visual appearance contrasts with the usual observations. Deep models trained on common remote sensing data will output drastically different features for these out-of-distribution samples, compared to those closer to their training dataset.
Detecting them could therefore help anticipate changes in the observations, either geographical or environmental.
In this work, we show that the reconstruction error of diffusion models can effectively serve as unsupervised out-of-distribution detectors for remote sensing images., using as a plausibility score.
Moreover, we introduce ODEED, a novel reconstruction-based scorer using the probability-flow ODE of diffusion models. We validate it experimentally on SpaceNet 8 with various scenarios, such as classical OOD detection with geographical shift and near-OOD setups: pre/post-flood and non-flooded/flooded image recognition.
We show that our ODEED scorer significantly outperforms other diffusion-based and discriminative baselines on the more challenging near-OOD scenarios of flood image detection, where OOD images are close to the distribution tail.
We aim to pave the way towards better use of generative models for anomaly detection in remote sensing.
