# Evaluating Supevised Contrastive Learning for noise-robust Speech Emotion Recognition (SER)

The objective is to compare the performance between a standard CNN trained with Cross-Entropy loss and a CNN trained using Supervised Contrastive Learning (SupCon) loss. We will evaluate the performance of each approach on the RAVDESS Emotional speech audio dataset, testing the robustiness by artificially injecting Gaussian noise on the test set.

## Implemementation

### Dataset pipeline

Needs to fetch and split the datasets. Also, needs to be able to extract Mel-spectrograms and perform data augmentation.


### Model A: baseline

- Network: CNN Encoder -> Linear Classifier
- Input: Mel-Spectrogram (Clean dataset)
- Loss: Cross-Entroopy Loss


### Model B: SupCon

**Stage 1**:

- Network: CNN Encoder -> Non-linear projection head (MLP)
- Input: Mel-Spectrogram (TODO: research augm)
- Loss: Supervised Contrastive Loss

**Stage 2**:

- Network: Fronzen CNN Encoder -> Linear Classifier
- Input: Mel-Spectrogram (Clean dataset)
- Loss: Cross-Entropy Loss

### Execution

1. Implement the datsaet pipeline (fetch, split, augment).
2. Establish Baseline performance (Model A) on clean and noisy test sets.
3. Train the SupCon Encoder (Model B - Stage 1).
4. Train the SupCon Linear Classifier (Model B - Stage 2).
5. Compare the performance of both models under noisy conditions.

## References:

- [Audio 02 - Audio Features](https://lefkippos.ds.unipi.gr/modules/document/file.php/AI_IIT107/AI%20-%20Multimodal%20AUDIO%20-%2002_%20Audio%20features.pdf)
- [DL - 03 - CNNs.pdf](https://lefkippos.ds.unipi.gr/modules/document/file.php/AI_IIT110/2025-2026/Deep%20Learning%20%28Giannakopoulos%20%26%20Kakogeorgiou%29/DL%20-%2003%20-%20CNNs.pdf)
- [DL - 06 - Practical DL Issues.pdf](https://lefkippos.ds.unipi.gr/modules/document/file.php/AI_IIT110/2025-2026/Deep%20Learning%20%28Giannakopoulos%20%26%20Kakogeorgiou%29/DL%20-%2006%20-%20Practical%20DL%20Issues.pdf)
- [Lecture 8 [Self-Supervised Learning].pdf](https://lefkippos.ds.unipi.gr/modules/document/file.php/AI_IIT110/2025-2026/Deep%20Learning%20%28Giannakopoulos%20%26%20Kakogeorgiou%29/Lecture%208%20%5BSelf-Supervised%20Learning%5D.pdf)
- [Supervised Contrastive Learning, Prannay Khosla et al.](https://arxiv.org/pdf/2004.11362) 



# Notes

- A spectrogram is a visual representation of the spectrum of frequencies in a signal as they change over time.
- Spectrograms are generated from sound signals using Fourier Transforms.
- A Fourier Transform decomposes the signal into its constituent frequencies and displays the amplitude of each frequency present in the signal.
- Mel spectrogram is a spectrogram that is converted to Mel scale.

 




## References
- https://ketanhdoshi.github.io/Audio-Mel/
- https://medium.com/analytics-vidhya/understanding-the-mel-spectrogram-fca2afa2ce53