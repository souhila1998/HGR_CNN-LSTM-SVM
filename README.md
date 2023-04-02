# Enhancing Dynamic Hand Gesture Recognition using Feature Concatenation via Multi-Input Hybrid Model
## Three-Input CNN-LSTM-SVM
The proposed approach is designed to classify dynamic hand gestures, which are formed by a consecutive sequence of poses where their characteristics vary over time. Therefore, the recognition process of dynamic gestures takes into account both spatial and temporal information. To enable the analysis of spatial and temporal features of gestures, we propose using a three-input CNN in conjunction with an LSTM to process the input data and perform feature extraction. First, the three-input CNN is used to extract the spatial features corresponding to the low-level representation of the images. Each representation is processed separately in a CNN branch. To fully represent the gesture, the output features of the three CNN branches are merged. The concatenated features are reshaped and provided as input to the LSTM for temporal feature extraction. The LSTM captures and memorizes how the features extracted by the CNN layers change over time. The output of the LSTM that provides the spatiotemporal features is put into vector form and fed into the multiclass SVM. The SVM acts as the final classifier of the architecture and gives the prediction result.

![three_input_cnn_lstm_svm](https://user-images.githubusercontent.com/127494864/229339601-8c5f53a4-6f67-4ba0-a3ab-0a3ca5ef0c21.PNG)

The noteworthy characteristics of the three-input CNN-LSTM-SVM are:

*	Increasing the amount of input data to prevent overfitting and improve the generalization performance of the model.
*	Adopting a more efficient feature extractor.
*	Using both spatial and temporal information to describe a gesture.
*	Providing the final classifier with more information to make a decision.

## Dataset
The dataset and labels are available on the following [link](https://drive.google.com/drive/folders/1RMtVFkmEy9848MaO5boX_l0xhk-zSszA?usp=sharing)
