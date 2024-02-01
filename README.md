# OFDM Signal Detection in Cognitive Radio Networks

This project focuses on developing a machine learning-based approach for detecting OFDM (Orthogonal Frequency Division Multiplexing) signals in cognitive radio networks. The goal is to differentiate between primary and secondary user signals, enabling efficient spectrum utilization and dynamic spectrum access.

## Project Overview

Cognitive radio networks are advanced wireless communication systems that intelligently adapt to changing radio frequency (RF) environments. OFDM is a popular modulation technique used in modern wireless systems due to its robustness to frequency-selective fading and high spectral efficiency.

### Key Components
1. **Dataset Generation**: Synthetic datasets containing IQ samples of OFDM signals for primary and secondary users are generated. These datasets simulate various channel conditions and user behaviors.
2. **Data Preprocessing**: Feature extraction and normalization techniques are applied to preprocess the dataset, preparing it for model training.
3. **Model Training**: An SVM (Support Vector Machine) classifier is trained on the preprocessed dataset to classify primary and secondary user signals.
4. **Model Evaluation**: The performance of the trained SVM classifier is evaluated using metrics such as accuracy, confusion matrix, and ROC curve.
5. **Deployment**: The trained model can be deployed in cognitive radio networks for real-time signal detection, facilitating dynamic spectrum access and efficient spectrum utilization.

## Usage

### Prerequisites
- Python (>=3.6)
- NumPy
- scikit-learn
- matplotlib

### Installation
1. Clone the repository:
   ```
   git clone https://github.com/yourusername/OFDM-Signal-Detection.git
   cd OFDM-Signal-Detection
   ```
2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

### Project Structure
- `generate_datasets.py`: Script to generate synthetic datasets of OFDM signals.
- `train_and_evaluate.py`: Script to train an SVM classifier and evaluate its performance.
- `plots.py`: Script to generate relevant plots for model evaluation.
- `datasets/`: Directory to store generated datasets (IQ samples and labels).
- `README.md`: Project documentation and usage instructions.

### Execution
1. Generate datasets:
   ```
   python generate_datasets.py
   ```
2. Train and evaluate the model:
   ```
   python train_and_evaluate.py
   ```
3. Plot evaluation graphs:
   ```
   python plots.py
   ```
