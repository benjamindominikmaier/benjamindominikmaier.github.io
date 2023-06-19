---
title: "Entropy predicts sensitivity of pseudo-random seeds (RECOMB 2023)"
collection: talks
type: "Talk"
permalink: /talks/2023-RECOMB
venue: "RECOMB 2023 - 27th International Conference on Research in Computational Molecular Biology"
date: 2023-04-16
location: "Istanbul, Turkey"
---

Benjamin Maier & Kristoffer Sahlin (2022): Entropy predicts sensitivity of pseudo-random seeds
[Preprint](https://www.biorxiv.org/content/10.1101/2022.10.13.512198v2) | [Proceedings]{https://link.springer.com/book/10.1007/978-3-031-29119-7 } | [Paper]{https://doi.org/10.1101/gr.277645.123}

In sequence similarity search applications such as read mapping, it is desired that seeds match between a read and reference in regions with mutations or read errors (seed sensitivity). K-mers are likely the most well-known and used seed construct in bioinformatics, and many studies on, e.g., spaced k-mers aim to improve sensitivity over k-mers. Spaced k-mers are highly sensitive when substitutions largely dominate the mutation rate but quickly deteriorate when indels are present. Recently, we developed a pseudo-random seeding construct, strobemers, which were empirically demonstrated to have high sensitivity also at high indel rates. However, the study lacked a deeper understanding of why. In this study, we demonstrate that a seed’s entropy (randomness) is a good predictor for seed sensitivity. We propose a model to estimate the entropy of a seed and find that seeds with high entropy, according to our model, in most cases have high match sensitivity. We also present three new strobemer seed constructs, mixedstrobes, altstrobes, and multistrobes. We use both simulated and biological data to demonstrate that our new seed constructs improve sequence-matching sensitivity to other strobemers. We implement strobemers into minimap2 and observe slightly faster alignment time and higher accuracy than using k-mers at various error rates.

Our discovered seed randomness-sensitivity relationship explains why some seeds perform better than others, and the relationship provides a framework for designing even more sensitive seeds. In addition, we show that the three new seed constructs are practically useful. Finally, in cases where our entropy model does not predict the observed sensitivity well, we explain why and how to improve the model in future work.
