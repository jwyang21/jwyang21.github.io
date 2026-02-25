---
layout: page
title: Deep learning-based survival prediction using DNA methylation-derived 3D genomic information
description: "[Oral Presentation] ACM Conference on Bioinformatics, Computational Biology, and Health Informatics (ACM-BCB) 2023"
img: assets/img/project/2023_ACM-BCB.png
importance: 3
category: work
---

Three-dimensional (3D) genome states are closely related to cancerdevelopment. Nonetheless, the 3D genome information has notbeen clinically utilized to the best of our knowledge, due to thecostly production of Hi-C data which is a manifest source of 3Dgenome information. Therefore, there is a need for a novel metriccomputable from a 3D genome-related data which is more easilyaccessible for the clinical utilization of 3D genome information.We here propose a method to extract 3D genome-aware epigeneticfeatures from DNA methylation data and use these features for adeep learning-based survival prediction. These features are derivedfrom the 3D genome structures which are rebuilt from the DNAmethylation data in an individual level. The results showed that us-age of 3D genome-aware features contributed to more accurate riskprediction across seven cancer types, suggesting the effectivenessof the knowledge about 3D genome structure embedded in thesefeatures. The deeper biological investigation revealed that alteredDNA methylation level in risk-high group could be related to the anomalously activated genes involved in cancer-related pathways.Altogether, the risks predicted from 3D genome-aware epigeneticfeatures showed its significance as a survival predictor in sevencancer types, along with its biological importance.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/project/2023_ACM-BCB.png" title="Overview" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure 1. Overview of the whole pipeline. (A) Single-sample inference of 3D genome structure. The binned difference matrix(BDM) is constructed from the 450K DNA methylation data, and the PC1 of BDM is extracted. The BDM PC1s are reflective ofthe 3D genome structures. (B) Reference 3D genome states are constructed by averaging the BDM PC1s from multiple normalcells of the same tissue type or the stem cells. The resulting vectors are used as normal/stem references, representing thetissue type-specific normalness or stemness, respectively. (C) Each reconstructed 3D genome state is represented into a space.Distances from individual states to stem/normal references are measured. The blue and red arrows represent normal and stemdistances, respectively. Between two depicted samples 𝑗 and 𝑘, sample 𝑗 has shorter stem distance and longer normal distance.Therefore, sample 𝑗 has higher stem closeness. The more detailed procedures for quantifying stem closeness is explained in thesupplementary information section B-C. (D) The 3D genome-aware epigenetic features and survival-related features (age andgender) are concatenated for each sample. The feedforward neural network predicts risk of failures using this input feature.
</div>
