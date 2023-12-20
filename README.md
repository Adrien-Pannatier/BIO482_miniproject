# BIO-482 Miniproject - Neuronal Cell Type Classification

Neurons play a crucial role in cognitive function, and understanding and categorizing the diversity of different cell types are essential for comprehending key aspects of brain function. 
This project aims to develop a robust classifier for neuronal cell types, enhancing our ability to characterize and differentiate various neurons. 
The focus is on four cell classes: Excitatory cells, Vasoactive Intestinal Peptide (VIP) inhibitory cells, Parvalbumin (PV) inhibitory cells, and Somatostatin (SST) inhibitory cells.

## Dataset and Features

The dataset used in this project exhibits interesting features for classifying different cell types, particularly from two experimental data sources: active touch and free whisking. 
The hypothesis is that these data sources can contribute to the development of a reliable classifier. The selected features for classification are outlined in Table 1.

| Feature              | Description         |
|----------------------|---------------------|
| ap_threshold         | Action potential threshold |
| ap_duration          | Action potential duration  |
| mean_vm              | Mean membrane potential   |
| std_vm               | Standard deviation of membrane potential |
| fft_low              | Low-frequency Fast Fourier Transform component |
| fft_high             | High-frequency Fast Fourier Transform component |
| numb_events         | Number of events          |
| wp_amplitude_pre    | Whisking pre-amplitude    |
| wp_amplitude_post   | Whisking post-amplitude   |
| vm_amplitude_pre    | Membrane potential pre-amplitude |
| vm_amplitude_post   | Membrane potential post-amplitude |
| ap_fr_pre           | Action potential firing rate pre |
| ap_fr_post          | Action potential firing rate post |

## Classification Methodology

The chosen methodology involves the following steps:
1. **Feature Selection:** Identify and select relevant features for classification.
2. **Classification Methods:** Test and assess multiple classification algorithms to determine the most effective one.
3. **Algorithms Investigated:**
    - Multiple Logistic Regression
    - Random Forest
    - K-nearest Neighbours
    - Support Vector Machine

4. **Dataset Splitting:** Split the dataset into training and testing subsets. The ratio of test to train sizes is 1/5.
5. **Performance Metrics:** Compute accuracy scores and generate confusion matrices for performance quantification.

## Classification Scenarios

1. **All Cell Types Classification:**
   - Investigate classification among all cell types for both free whisking and active touch.

2. **Excitatory vs. Inhibitory Cells Classification:**
   - Examine the classification between excitatory and inhibitory cells.

3. **Inhibitory Cell Type Classification:**
   - Explore the classification within inhibitory cell types.
