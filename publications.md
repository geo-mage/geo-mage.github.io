# Publications

##  Detecting Out-Of-Distribution Earth Observation Images with Diffusion Models

Authors: Georges Le Bellier, Nicolas Audebert

🔗 [arXiv](https://arxiv.org/abs/2404.12667) [HAL](https://hal.science/hal-04551408/)

**EarthVision 2024** (CVPR workshop)

Earth Observation imagery can capture rare and unusual events, such as disasters and major landscape changes, whose visual appearance contrasts with the usual observations. Deep models trained on common remote sensing data will output drastically different features for these out-of-distribution samples, compared to those closer to their training dataset.
Detecting them could therefore help anticipate changes in the observations, either geographical or environmental.
In this work, we show that the reconstruction error of diffusion models can effectively serve as unsupervised out-of-distribution detectors for remote sensing images., using as a plausibility score.
Moreover, we introduce ODEED, a novel reconstruction-based scorer using the probability-flow ODE of diffusion models. We validate it experimentally on SpaceNet 8 with various scenarios, such as classical OOD detection with geographical shift and near-OOD setups: pre/post-flood and non-flooded/flooded image recognition.
We show that our ODEED scorer significantly outperforms other diffusion-based and discriminative baselines on the more challenging near-OOD scenarios of flood image detection, where OOD images are close to the distribution tail.
We aim to pave the way towards better use of generative models for anomaly detection in remote sensing.
