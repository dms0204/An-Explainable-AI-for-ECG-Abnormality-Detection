# ECG Anomaly Detection
## Abstract
Electrocardiogram (ECG) anomaly detection is critical for early cardiovascular diagnosis, b8t precise localization of anomalous segments in multi-lead signals remains challenging. This study presents a weakly-supervised deep learning framework for 12-lead ECG anomaly detection and visual localization. Using a 1D ResNet architecture, the model automatically extracts complex spatiotemporal features from preprocessed 12-lead signals for binary and multi-label classification. To address the black-box nature of deep networks and facilitate clinical review, 1D Grad-CAM is integrated to generate activation maps that pinpoint specific anomalous waveform regions. This approach eliminates the need for expensive segment-level annotations while offering high diagnostic accuracy and spatial interpretability for continuous clinical monitoring.

## License
This project uses the PTB-XL dataset licensed under **[CC BY 4.0](https://physionet.org/content/ptb-xl/view-license/1.0.3/)**.

## References
- Wagner, P., Strodthoff, N., Bousseljot, R., Samek, W., & Schaeffter, T. (2022). PTB-XL, a large publicly available electrocardiography dataset [Dataset]. PhysioNet. https://doi.org/10.13026/kfzx-aw45
- Strodthoff, N., Wagner, P., Schaeffter, T., & Samek, W. (2020, April 28). Deep Learning for ECG Analysis: Benchmarks and Insights from PTB-XL. arXiv.org. https://arxiv.org/abs/2004.13701
- Ruiz-Barroso, P., Castro, F. M., Miranda, J., Constantinescu, D.-A., Atienza, D., & Guil, N. (2025). FADE: Forecasting for Anomaly Detection on ECG. arXiv.org. https://arxiv.org/abs/2502.07389