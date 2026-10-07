# ECG Anomaly Detection
## Abstract
Electrocardiogram (ECG) anomaly detection is critical for early cardiovascular diagnosis, b8t precise localization of anomalous segments in multi-lead signals remains challenging. This study presents a weakly-supervised deep learning framework for 12-lead ECG anomaly detection and visual localization. Using a 1D ResNet architecture, the model automatically extracts complex spatiotemporal features from preprocessed 12-lead signals for binary and multi-label classification. To address the black-box nature of deep networks and facilitate clinical review, 1D Grad-CAM is integrated to generate activation maps that pinpoint specific anomalous waveform regions. This approach eliminates the need for expensive segment-level annotations while offering high diagnostic accuracy and spatial interpretability for continuous clinical monitoring.

## License
This project uses the PTB-XL dataset licensed under **[CC BY 4.0](https://physionet.org/content/ptb-xl/view-license/1.0.3/)**.

## References
[1] N. Strodthoff, P. Wagner, T. Schaeffter, and W. Samek, “Deep learning for ECG analysis: Benchmarks and insights from PTB-XL,” arXiv preprint arXiv:2004.13701, 2020. arXiv:2004.

[2] A. E. M. Atwa, E.-S. Atlam, A. Ahmed, M. A. Atwa, E. M. Abdelrahim, and A. I. Siam, “Interpretable deep learning models for arrhythmia classification based on ECG signals using PTB-X dataset,” Diagnostics, vol. 15, no. 15, p. 1950, 2025, doi: 10.3390/diagnostics15151950.

[3] J.-H. Jang and Y.-y. Jo, “ExECG: An Explainable AI Framework for ECG models,” arXiv preprint arXiv:2605.19258, 2026. doi: 10.48550/arXiv.2605.19258.

[4] Y. Song, W. Zheng, T. Chen, Z. Wang, J. Shi, and Y. Chen, “Deep neural network architectures for electrocardiogram classification: A comprehensive evaluation,” arXiv preprint arXiv:2602.17701, 2026, doi: 10.48550/arXiv.2602.17701.

[5] Hsd1503, “Resnet1d: PyTorch implementations of several SOTA backbone deep neural networks on one-dimensional (1D) signal/time-series data,” GitHub, [Computer software]. Accessed: Oct. 3, 2026. https://github.com/hsd1503/resnet1d

[6] Liguge, “1D-Grad-CAM for interpretable intelligent fault diagnosis,” GitHub, [Computer software]. Accessed: Oct. 3, 2026. https://github.com/liguge/1D-Grad-CAM-for-interpretable-intelligent-fault-diagnosis

[7] P. Helme, N. Strodthoff, M. Kampffmeyer, W. Samek, and K. R. Müller, “ecg_ptbxl_benchmarking: Benchmarking deep learning models for ECG classification,” GitHub, [Computer software]. Accessed: Oct. 4, 2026. https://github.com/helme/ecg_ptbxl_benchmarking