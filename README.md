# Tennis Shots Recognition through Human-Pose Estimation and Deep LSTM-based Neural Network

The developed algorithm classifies tennis strokes from video input using a Deep LSTM-based Neural Network with human pose estimation. Key steps include:
- **Preprocessing**: Extracts keypoints from videos using **OpenPose**, normalizes the coordinates, and structures them into a dataset. Padding ensures consistency;
- **Feature Representation**: Frames are represented as sequences of 18 joints with (x, y) coordinates, reshaped into (N, 36) tensors;
- **Model Architecture**: A **Bidirectional 3-layer LSTM** processes frame sequences, capturing temporal dependencies;
- **Attention Mechanism**: Enhances classification by focusing on relevant time steps, applied via a dot-product attention layer;
- **Output & Training**: The final fully connected layer predicts one of 10 tennis shot classes (two excluded), using Adagrad optimization and dropout for regularization.

The model achieves 47% average accuracy, benchmarking against other deep learning approaches for tennis action recognition.

To execute the notebook, use there resources:
https://drive.google.com/drive/folders/17zVb39IatBCqojtsUTMkXGLcvK2uGiM4?usp=share_link
