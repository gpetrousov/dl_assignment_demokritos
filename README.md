# Evaluating Supervised Contrastive Learning for noise-robust Speech Emotion Recognition (SER)

Speech Emotion Recognition (SER) on limited datasets such as RAVDESS often leads to model overfitting. This study investigates a Supervised Contrastive Learning (SupCon) pipeline combined with multi-view SpecAugment to extract stable emotional representations rather than memorizing specific acoustic frequencies. The experimental results demonstrate that the SupCon architecture increases the clean test accuracy from a 53% baseline to 60% compared to a standard Cross-Entropy approach. Furthermore, the proposed methodology exhibits improved classification stability under heavy Gaussian noise degradation.

## References:

- [Audio 02 - Audio Features](https://lefkippos.ds.unipi.gr/modules/document/file.php/AI_IIT107/AI%20-%20Multimodal%20AUDIO%20-%2002_%20Audio%20features.pdf)
- [DL - 03 - CNNs.pdf](https://lefkippos.ds.unipi.gr/modules/document/file.php/AI_IIT110/2025-2026/Deep%20Learning%20%28Giannakopoulos%20%26%20Kakogeorgiou%29/DL%20-%2003%20-%20CNNs.pdf)
- [DL - 06 - Practical DL Issues.pdf](https://lefkippos.ds.unipi.gr/modules/document/file.php/AI_IIT110/2025-2026/Deep%20Learning%20%28Giannakopoulos%20%26%20Kakogeorgiou%29/DL%20-%2006%20-%20Practical%20DL%20Issues.pdf)
- [Lecture 8 [Self-Supervised Learning].pdf](https://lefkippos.ds.unipi.gr/modules/document/file.php/AI_IIT110/2025-2026/Deep%20Learning%20%28Giannakopoulos%20%26%20Kakogeorgiou%29/Lecture%208%20%5BSelf-Supervised%20Learning%5D.pdf)
- [Supervised Contrastive Learning, Prannay Khosla et al.](https://arxiv.org/pdf/2004.11362)


# Repository Structure
```text
├── notebooks/
│   ├── notebook.ipynb      # Main notebook
│   └── notebook.py         # Source only version
├── report_src/             # Latex report source
├── requirements.txt        # Dependencies
└── README.md               # Repository documentation
```

# Replicating the results

```shell
pip install -r requirements.txt
```

Run main notebook in `notebooks/notebook.ipynb`.
