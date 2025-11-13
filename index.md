# 🛰 MAGE: Mapping Aerial imagery with Game Engine data

*Mapping Aerial imagery with Game Engine data* (MAGE, 2022-2026) is a deep learning and Earth Observation research project funded by the JCJC program of the [Agence Nationale de la Recherche](https://anr.fr/) (ANR).

## News

* **November 10, 2025:** [New paper](publications.md) on unsupervised domain adaptation for remote sensing imagery. We introduce FlowEO, a flow matching based image translation models that outperform existing approaches in many scenarios, including SAR-to-optical translation and temporal domain adaptation.
* **June 27, 2025:** The alpha release of WorldWeaver, our procedural generator of low-fidelity digital twins based on Blender, has been released on [GitHub](https://github.com/geo-mage/worldweaver).
* **April 28, 2025:** X-STARS has been accepted for publication into the *IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing*.
* **December 5, 2024:** Several MAGE project members were involved into the design of PANGAEA, a new benchmark to evaluate large pretrained models for Earth Observation, now released on [GitHub](https://github.com/VMarsocci/pangaea-bench).
* **May 16, 2024:** New [preprint](publications.md) on self-supervised adaptation of pretrained labels to new sensors. We introduce X-STARS, a continual self-training strategy that shows better representations of optical imagery with less data than existing SSL methods.
* **April 20, 2024:** Our [first paper](publications.md) on detecting out-of-distribution remote sensing images with diffusion models has been accepted at EarthVision 2024 (CVPR workshop)!
* **March 1st, 2023:** Valerio Marsocci joines the project as a postdoctoral fellow. His work will focus on self-supervised learning for Earth Observation data.
* **February 13, 2023:** Héloïse Verstraete joins the project as a research engineer. She will work on developing the simulation and rendering tool to produce synthetic aerial images of urban environments.
* **January 27, 2023:** scientific kick-off at Cnam/Cédric.
* **January 16, 2023:** Georges Le Bellier joins the team as a PhD student on domain adaptation and self-supervised learning on remote sensing data. He will be advised by Nicolas Audebert, Nicolas Thome and Marin Ferecatu.

## About the project

International satellite constellations such as Sentinel-2 and national high resolution imaging programs such as SPOT or BDORTHO in France have made Earth Observation (EO) data abundant. However, this data is unlabeled, i.e. misses semantic information useful to train machine learning (ML) models for downstream applications.

While the fast response time of AI models would strongly benefit rapid mapping applications, the Copernicus Emergency Management Service mostly rely on expert interpretation of remote sensing imagery to quickly deliver geo-data for disaster management (flooding, seismic events, refugee camps…). Since disasters are rare events, datasets are even scarcer than usual. When faced with this issue, autonomous driving introduced learning on simulations and games, especially to generate simulations of rare events that are expensive to acquire in real life. As tools such as CityEngine now produce plausible digital twins of cities, simulating EO data with various environmental conditions becomes feasible.

![The MAGE project aims to design a sim2real workflow for Earth Observation. We collect large-scale unlabeled remote sensing datasets from open sources. We generate synthetic data by simulating disasters on 3D models using state-of-the-art engines such as Unreal or Blender. This mixed training set is used to train deep neural networks in semi-supervised fashion, using domain adaptation to reduce the gap between real and synthetic images. Then, we leverage the trained models on real use cases for disaster mapping.](images/MAGE_workflow.png)

This research project aims to bring all of those tools together to unlock the power of simulated data and deep learning for rapid disaster mapping based on EO imagery. We will leverage game engines to produce simulated aerial views of cities before and after a disaster (flood, earthquake or fire). These images will act as supervised training data, in addition to the existing big real unlabeled EO data. To improve the realism of simulated images, we will design domain adaptation techniques based on generative models to bridge the perceptual gap between synthetic and real EO images. We will then conceive semi-supervised training algorithms for semantic segmentation based on self-supervised learning with pretext tasks suitable for EO data. This will allow us to train deep models with high generalization ability to perform post-disaster high-precision mapping to detect damaged buildings, find the most affected areas and help navigation of emergency services.

## 🏦 Funding

This project is funded through the ANR Young Researchers (*Jeunes Chercheurs/Jeunes Chercheuses*) program.

![Logo of the ANR](images/anr_logo.png){:height="40px"}
![Logo of the Cnam/Cédric laboratory](images/cedric_cnam.png){:height="40px"}
