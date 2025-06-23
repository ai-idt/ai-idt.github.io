---
layout: page
title: Projects
permalink: /projects/
---
# NOVA
![NOVA](/assets/NOVA.png)
Deployed models often encounter data that differs from training distributions, requiring robust out-of-distribution detection and open-world recognition capabilities. While foundation and vision-language models are expected to generalize broadly, current benchmarks with limited outlier types fail to capture real-world challenges, particularly in clinical settings.
We present NOVA, a challenging evaluation benchmark of ~900 brain MRI scans spanning 281 rare pathologies with heterogeneous acquisition protocols. Each case includes clinical narratives and expert bounding-box annotations, enabling joint assessment of anomaly localization, visual captioning, and diagnostic reasoning. As a training-free benchmark, NOVA provides an extreme stress-test of out-of-distribution generalization across both sample appearance and semantic domains, addressing critical gaps in evaluating model robustness for real-world medical applications.

[[Paper]](https://arxiv.org/abs/2505.14064) | [[Data]](https://huggingface.co/datasets/Ano-2090/Nova)

# GliODIL
![GliODIL](/assets/GliODIL.png)
Physical models, represented by partial differential equations, are crucial in addressing many under-constrained problems, such as tumor growth modeling. Deep learning methods often struggle to accurately estimate the complete distribution of tumor cells, primarily due to insufficient training data. As a result, most existing approaches rely on physics-based simulations to align with observed tumor characteristics, yielding anatomically and physiologically plausible estimates. However, these methods face challenges when dealing with complex and unknown initial conditions and are often constrained by rigid physical models. In this work, we introduce a novel method that balances data-driven and physics-based cost functions. Specifically, we propose a unique discretization scheme that quantifies how well our learned spatiotemporal distributions of tumors and brain tissue adhere to their respective growth and elasticity equations. This quantification acts as a regularization term rather than a strict constraint, allowing for greater flexibility and effectiveness in integrating patient data compared to existing models.

[[Paper]](https://neurips.cc/virtual/2024/poster/94680) | [[Code]](https://github.com/m1balcerak/PhysRegTumor)

# DL-Prior
![DL-Prior](/assets/DL-Prior.png)
Biophysical modeling, particularly involving partial differential equations (PDEs), offers significant potential for tailoring disease treatment protocols to individual patients. However, the inverse problem-solving aspect of these models presents a substantial challenge, either due to the high computational requirements of model-based approaches or the limited robustness of deep learning (DL) methods. We propose a novel framework that leverages the unique strengths of both approaches in a synergistic manner. Our method incorporates a DL ensemble for initial parameter estimation, facilitating efficient downstream evolutionary sampling initialized with this DL-based prior.

[[Paper]](https://ieeexplore.ieee.org/document/10748406) | [[Code]](https://github.com/jonasw247/a-learnable-prior-improves-inverse-tumor-growth-modeling)

# VariViT
![VariViT](/assets/VariViT.png)
Vision Transformers (ViTs) have emerged as the state-of-the-art architecture in representation learning, leveraging self-attention mechanisms to excel in various tasks. ViTs split images into fixed-size patches, constraining them to a predefined size and necessitating pre-processing steps like resizing, padding, or cropping. This poses challenges in medical imaging, particularly with irregularly shaped structures like tumors. To address this, we propose VariViT, an improved ViT model crafted to handle variable image sizes while maintaining a consistent patch size. VariViT employs a novel positional embedding resizing scheme for a variable number of patches. We also implement a new batching strategy within VariViT to reduce computational complexity, resulting in faster training and inference times.

[[Paper]](https://openreview.net/forum?id=uoRbMNoZ7w) | [[Code]](https://github.com/Aswathi-Varma/varivit)

# LST-AI
![LST-AI](/assets/lst-ai.png)
LST-AI is a publicly available UNet ensemble that segments inflammatory white matter MS lesions and classifies their location according to the 2017 McDonald criteria.

[[Paper]](https://doi.org/10.1016/j.nicl.2024.103611) | [[Code]](https://github.com/CompImg/LST-AI)

# INR for Multi-Contrast Super-Resolution
![NIF](/assets/NIF.png)
Combining different views of multi-contrast scans into high-resolution isotropic 3D scans is challenging due to the lack of a large training cohort, which calls for a subject-specific framework. This work proposes a novel solution to this problem leveraging Implicit Neural Representations (INR). Our proposed INR jointly learns two different contrasts of complementary views in a continuous spatial function and benefits from exchanging anatomical information between them.

[[Paper]](https://link.springer.com/chapter/10.1007/978-3-031-43993-3_17) | [[Code]](https://github.com/jqmcginnis/multi_contrast_inr/)

# GraphMS
![GraphMS](/assets/GraphMS.png)
Our work represents the first attempt to utilize graph neural networks (GNN) to aggregate imaging lesion-based biomarkers for a novel global representation. We propose a two-stage MS inflammatory disease activity prediction approach. First, a 3D segmentation network detects lesions, and a self-supervised algorithm extracts their image features. Second, the detected lesions are used to build a patient graph. The lesions act as nodes in the graph and are initialized with image features extracted in the first stage. Finally, the lesions are connected based on their spatial proximity and the inflammatory disease activity prediction is formulated as a graph classification task. Furthermore, we propose a self-pruning strategy to auto-select the most critical lesions for prediction. 

[[Paper]](https://link.springer.com/chapter/10.1007/978-3-031-43993-3_22) | [[Code]](https://github.com/chinmay5/ms_ida)
