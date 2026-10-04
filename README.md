# ECG Anomaly Detection
## Abstract
Electrocardiogram (ECG) anomaly detection is critical for early cardiovascular diagnosis, b8t precise localization of anomalous segments in multi-lead signals remains challenging. This study presents a weakly-supervised deep learning framework for 12-lead ECG anomaly detection and visual localization. Using a 1D ResNet architecture, the model automatically extracts complex spatiotemporal features from preprocessed 12-lead signals for binary and multi-label classification. To address the black-box nature of deep networks and facilitate clinical review, 1D Grad-CAM is integrated to generate activation maps that pinpoint specific anomalous waveform regions. This approach eliminates the need for expensive segment-level annotations while offering high diagnostic accuracy and spatial interpretability for continuous clinical monitoring.

## License
This project uses the PTB-XL dataset licensed under **[CC BY 4.0](https://physionet.org/content/ptb-xl/view-license/1.0.3/)**.

## References
- Ruiz-Barroso, P., Castro, F. M., Miranda, J., Constantinescu, D.-A., Atienza, D., & Guil, N. (2025). FADE: Forecasting for anomaly detection on ECG. arXiv. https://arxiv.org/abs/2502.07389
- Strodthoff, N., Wagner, P., Schaeffter, T., & Samek, W. (2020). Deep learning for ECG analysis: Benchmarks and insights from PTB-XL. arXiv. https://arxiv.org/abs/2004.13701
- Wagner, P., Strodthoff, N., Bousseljot, R., Samek, W., & Schaeffter, T. (2022). PTB-XL, a large publicly available electrocardiography dataset [Dataset]. PhysioNet. https://doi.org/10.13026/kfzx-aw45
- Hsd1503. (n.d.). Resnet1d: PyTorch implementations of several SOTA backbone deep neural networks on one-dimensional (1D) signal/time-series data [Computer software]. GitHub. Retrieved October 3, 2026, from https://github.com/hsd1503/resnet1d
- Liguge. (n.d.). 1D-Grad-CAM for interpretable intelligent fault diagnosis [Computer software]. GitHub. Retrieved October 3, 2026, from https://github.com/liguge/1D-Grad-CAM-for-interpretable-intelligent-fault-
- Helme, P., Strodthoff, N., Kampffmeyer, M., Samek, W., & Müller, K. R. (2020). ecg_ptbxl_benchmarking: Benchmarking deep learning models for ECG classification [Computer software]. GitHub. Retrieved October 4, 2026, from https://github.com/helme/ecg_ptbxl_benchmarking