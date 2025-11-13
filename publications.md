# Publications

## FlowEO: Generative Unsupervised Domain Adaptation for Earth Observation

Authors: Georges Le Bellier, Nicolas Audebert

🔗 [arXiv](https://arxiv.org/abs/) 🔗 [HAL](https://hal.science/hal-)

**WACV 2026**

The increasing availability of Earth observation data offers unprecedented opportunities for large-scale environmental monitoring and analysis. However, these datasets are inherently heterogeneous, stemming from diverse sensors, geographical regions, acquisition times, and atmospheric conditions. Distribution shifts between training and deployment domains severely limit the generalization of pretrained remote sensing models, making unsupervised domain adaptation (UDA) crucial for real-world applications. We introduce FlowEO, a novel framework that leverages generative models for image-space UDA in Earth observation. We leverage flow matching to learn a semantically preserving mapping that transports from the source to the target image distribution. This allows us to tackle challenging domain adaptation configurations for classification and semantic segmentation of Earth observation images. We conduct extensive experiments across four datasets covering adaptation scenarios such as SAR to optical translation and temporal and semantic shifts caused by natural disasters. Experimental results demonstrate that FlowEO outperforms existing image translation approaches for domain adaptation while achieving on-par or better perceptual image quality, highlighting the potential of flow-matching-based UDA for remote sensing.

## Cross-sensor self-supervised training and alignment for remote sensing

Authors: Valerio Marsocci, Nicolas Audebert

🔗 [arXiv](https://arxiv.org/abs/2405.09922) 🔗 [HAL](https://hal.science/hal-04576064)

**IEEE JSTARS**

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

## PANGAEA: A Global and Inclusive Benchmark for Geospatial Foundation Models

Authors: Valerio Marsocci, Yuru Jia, Georges Le Bellier, David Kerekes, Liang Zeng, Sebastian Hafner, Sebastian Gerard, Eric Brune, Ritu Yadav, Ali Shibli, Heng Fang, Yifang Ban, Maarten Vergauwen, Nicolas Audebert, Andrea Nascetti

(in collaboration with KTH, ESA and KU Leuven)

🔗 [arXiv](https://arxiv.org/abs/2412.04204) 🔗 [HAL](https://hal.science/hal-)

🧮 [Benchmark on GitHub](https://github.com/VMarsocci/pangaea-bench)

**IEEE GRSM**

Geospatial Foundation Models (GFMs) have emerged as powerful tools for extracting representations from Earth observation data, but their evaluation remains inconsistent and narrow. Existing works often evaluate on suboptimal downstream datasets and tasks, that are often too easy or too narrow, limiting the usefulness of the evaluations to assess the real-world applicability of GFMs. Additionally, there is a distinct lack of diversity in current evaluation protocols, which fail to account for the multiplicity of image resolutions, sensor types, and temporalities, which further complicates the assessment of GFM performance. In particular, most existing benchmarks are geographically biased towards North America and Europe, questioning the global applicability of GFMs. To overcome these challenges, we introduce PANGAEA, a standardized evaluation protocol that covers a diverse set of datasets, tasks, resolutions, sensor modalities, and temporalities. It establishes a robust and widely applicable benchmark for GFMs. We evaluate the most popular GFMs openly available on this benchmark and analyze their performance across several domains. In particular, we compare these models to supervised baselines (e.g. UNet and vanilla ViT), and assess their effectiveness when faced with limited labeled data. Our findings highlight the limitations of GFMs, under different scenarios, showing that they do not consistently outperform supervised models. PANGAEA is designed to be highly extensible, allowing for the seamless inclusion of new datasets, models, and tasks in future research. By releasing the evaluation code and benchmark, we aim to enable other researchers to replicate our experiments and build upon our work, fostering a more principled evaluation protocol for large pre-trained geospatial models.
