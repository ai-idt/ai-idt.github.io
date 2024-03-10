---
layout: page
title: Projects
permalink: /projects/
---

# LST-AI
![LST-AI](/assets/lst-ai.png)
LST-AI is a publicly available UNet ensemble that segments inflammatory white matter MS lesions and classifies their location according to the 2017 McDonald criteria.

[[Paper]](https://www.medrxiv.org/content/10.1101/2023.11.23.23298966v1) | [[Code]](https://github.com/CompImg/LST-AI)


# NIF
![NIF](/assets/NIF.png)
Combining different views of multi-contrast scans into high-resolution isotropic 3D scans is challenging due to the lack of a large training cohort, which calls for a subject-specific framework. This work proposes a novel solution to this problem leveraging Implicit Neural Representations (INR). Our proposed INR jointly learns two different contrasts of complementary views in a continuous spatial function and benefits from exchanging anatomical information between them.

[[Paper]](https://link.springer.com/chapter/10.1007/978-3-031-43993-3_17) | [[Code]](https://github.com/jqmcginnis/multi_contrast_inr/)


# GraphMS
![GraphMS](/assets/GraphMS.png)
Our work represents the first attempt to utilize graph neural networks (GNN) to aggregate imaging lesion-based biomarkers for a novel global representation. We propose a two-stage MS inflammatory disease activity prediction approach. First, a 3D segmentation network detects lesions, and a self-supervised algorithm extracts their image features. Second, the detected lesions are used to build a patient graph. The lesions act as nodes in the graph and are initialized with image features extracted in the first stage. Finally, the lesions are connected based on their spatial proximity and the inflammatory disease activity prediction is formulated as a graph classification task. Furthermore, we propose a self-pruning strategy to auto-select the most critical lesions for prediction. 

[[Paper]](https://link.springer.com/chapter/10.1007/978-3-031-43993-3_22) | [[Code]](https://github.com/chinmay5/ms_ida)
