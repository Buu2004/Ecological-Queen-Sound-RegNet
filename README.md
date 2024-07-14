# Detecting-Queenless-Beehives-with-Convolutional-Neural-Networks-A-Comparative-Analysis

Detecting the queenless state in beehives is crucial for effective hive management and maintaining colony health. This study aims to identify a robust and generalizable 2D convolutional network structure for this task by evaluating four CNN models: RegNet, EfficientNet, AlexNet, and ResNet-50. Using two distinct datasets with low-frequency STFT and MFCC spectrograms as input, we assessed the models' performance. RegNet achieved the highest accuracy, 96.4\% on one dataset and 92.46\% on the other, due to its optimized design and efficient training. EfficientNet also performed well, with accuracies of 96.33\% and 90.32\%, leveraging its compound scaling approach. In contrast, ResNet-50 and AlexNet struggled to generalize, with significant drops in accuracy between the datasets. Our findings suggest that RegNet is the most effective model for detecting the queenless state, offering a promising solution for beekeeping applications. Future research should focus on further optimization and exploring additional regularization techniques to enhance model performance.


\begin{table}[H]
\centering
\caption{Accuracy of deep learning models in detecting queenless state}
\begin{tabular}{|l|ll|ll|}
\hline
                        & \multicolumn{2}{l|}{Dataset 1}                        & \multicolumn{2}{l|}{Dataset 2}                                   \\ \cline{2-5} 
\multirow{-2}{*}{Model} & \multicolumn{1}{l|}{MFCC}           & STFT          & \multicolumn{1}{l|}{MFCC}                          & STFT           \\ \hline
RegNet\_x\_400mf        & \multicolumn{1}{l|}{97.43}          & \textbf{96.4} & \multicolumn{1}{l|}{89.53}                         & 80.46          \\ \hline
RegNet\_y\_400mf        & \multicolumn{1}{l|}{\textbf{97.48}} & 95.25         & \multicolumn{1}{l|}{\textbf{92.46}}                & \textbf{82.46} \\ \hline
EfficientNetB0          & \multicolumn{1}{l|}{95.75}          & 94.93         & \multicolumn{1}{l|}{90.07}                         & 80.07          \\ \hline
EfficientNetB5          & \multicolumn{1}{l|}{96.33}          & 95.3          & \multicolumn{1}{l|}{90.32}                         & 81.12          \\ \hline
AlexNet                 & \multicolumn{1}{l|}{50.00}          & 50.00         & \multicolumn{1}{l|}{82.09}                         & 78.62          \\ \hline
Resnet-50               & \multicolumn{1}{l|}{95.65}          & 93.75         & \multicolumn{1}{l|}{87.57}                         & 81.37          \\ \hline
\end{tabular}
\label{result}
\end{table}
