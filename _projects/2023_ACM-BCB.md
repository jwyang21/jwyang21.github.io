---
layout: page
title: Deep learning-based survival prediction using DNA methylation-derived 3D genomic information
description: "[Oral Presentation] ACM Conference on Bioinformatics, Computational Biology, and Health Informatics (ACM-BCB) 2023"
img: assets/img/project/2023_ACM-BCB.png
importance: 3
category: work
---

Three-dimensional (3D) genome states are closely related to cancer development. Nonetheless, the 3D genome information has not been clinically utilized to the best of our knowledge, due to the costly production of Hi-C data which is a manifest source of 3D genome information. Therefore, there is a need for a novel metric computable from a 3D genome-related data which is more easily accessible for the clinical utilization of 3D genome information. We here propose a method to extract 3D genome-aware epigenetic features from DNA methylation data and use these features for a deep learning-based survival prediction. These features are derived from the 3D genome structures which are rebuilt from the DNA methylation data at an individual level. The results showed that usage of 3D genome-aware features contributed to more accurate risk prediction across seven cancer types, suggesting the effectiveness of the knowledge about 3D genome structure embedded in these features. The deeper biological investigation revealed that altered DNA methylation level in risk-high group could be related to the anomalously activated genes involved in cancer-related pathways. Altogether, the risks predicted from 3D genome-aware epigenetic features showed its significance as a survival predictor in seven cancer types, along with its biological importance.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/project/2023_ACM-BCB.png" title="Overview" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 1. Overview of the whole pipeline. (A) Single-sample inference of 3D genome structure. The binned difference matrix(BDM) is constructed from the 450K DNA methylation data, and the PC1 of BDM is extracted. The BDM PC1s are reflective ofthe 3D genome structures. (B) Reference 3D genome states are constructed by averaging the BDM PC1s from multiple normalcells of the same tissue type or the stem cells. The resulting vectors are used as normal/stem references, representing thetissue type-specific normalness or stemness, respectively. (C) Each reconstructed 3D genome state is represented into a space.Distances from individual states to stem/normal references are measured. The blue and red arrows represent normal and stemdistances, respectively. Between two depicted samples 𝑗 and 𝑘, sample 𝑗 has shorter stem distance and longer normal distance.Therefore, sample 𝑗 has higher stem closeness. The more detailed procedures for quantifying stem closeness is explained in thesupplementary information section B-C. (D) The 3D genome-aware epigenetic features and survival-related features (age andgender) are concatenated for each sample. The feedforward neural network predicts risk of failures using this input feature.
</div>
