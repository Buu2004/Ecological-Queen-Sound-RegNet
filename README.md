# RegNet: A High-Performance Deep Learning Model for Queenless State Detection in Beehives
<h2>Abstract</h2>

Honey bees play a crucial role in pollination, supporting ecosystem balance and agricultural productivity. The queen bee is essential for hive cohesion, but her presence can often be inferred through the colony’s overall behavior and condition rather than direct monitoring. This study proposes a non-invasive approach using deep learning techniques to analyze spectrogram features obtained from Short-Time Fourier Transform (STFT) and Mel-Frequency Cepstral Coefficients (MFCCs), to detect the queenless condition in beehives. We evaluate five convolutional neural network (CNN) architectures—ResNet-50, EfficientNet, RegNet, ViT and CaiT—on two datasets from different beehives. A customized transfer learning strategy is employed to enhance model performance. Experimental results show that RegNetY consistently outperforms other models, achieving the highest accuracy and F1-score across both datasets and feature types, indicating its robustness and generalizability in detecting hive states.
<h2>Dataset description:</h2>
<ul>
<li>Dataset 1:</li>
  <span>
    <ul>
      <li>This is a real dataset of audio recordings collected from various beehives at the Research Center for Tropical Bees and Beekeeping, Vietnam National University of Agriculture. The audio data, after being collected, were segmented into 20,000 clips, each 2 seconds long with a 1 second overlap.  the dataset was split into a training set (70%), validation set (10%), and test set (20%) for model training and evaluation.</li> 
      <li>Link: <a href="https://drive.google.com/drive/folders/1cepNqlm2OMJFbytdiCKJBw22amkjNphI?usp=drive_link">here</a></li>
    </ul>
  </span>
<li>Dataset 2:</li>
  <span>
    <ul>
    <li>This dataset was originally presented in <a href="https://doi.org/10.1007/s11042-023-15192-5">this paper</a>. It comprises 13,792 sound recordings, distributed among three types of Beehive buzz anomalies: 5,473 Bee samples, 3,458 NoBee samples, and 4,861 NoQueen samples. The dataset is partitioned into subsets for training, testing, and validation, divided into ratios of 80%, 20%, and 10%, respectively.</li> 
    <li>Link: <a href="https://www.kaggle.com/datasets/yevheniiklymenko/beehive-buzz-anomaliess">here</a></li>
    </ul>
  </span>
</ul>
<h2>Methodology:</h2>
<ul>
  <li>
    Our goal is to leverage the strengths
of well-established deep learning models designed for image processing and
identify suitable models to apply to audio processing and queenless state
monitoring using audio data.
  </li>
  ![Methodology](https://github.com/user-attachments/assets/e3318a65-986e-43d1-873a-f584d50b090d)
  <li>
    In this study, we transform the raw audio data into the
frequency domain using the Short-Time Fourier Transform (STFT) and Mel
Spectrograms.
  </li>
  <li>
    Once the spectrograms are obtained as images, various CNN-based mod-
els are employed to extract more significant features and accurately detect
the beehive state. We explore five different CNN architectures, ranging from
simple to complex: ResNet, EfficientNet, RegNet, ViT and CaiT. These mod-
els are known for their ability to handle 2D image data and their effectiveness
in beehive state detection.
  </li>
</ul>
