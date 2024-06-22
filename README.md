
# English to Kinyarwanda Translation using RNNs

## Project Overview
This project aims to build a model that translates text from English to Kinyarwanda using Recurrent Neural Networks (RNNs). The model utilizes an encoder-decoder architecture with LSTM cells for sequence-to-sequence translation.

## Dataset
The dataset used for training and testing consists of English-Kinyarwanda translation pairs. Each entry contains a phrase in English and its corresponding translation in Kinyarwanda.

### Dataset Creation
The dataset was created and curated specifically for this project. Entries are stored in JSON format, ensuring easy accessibility and compatibility with the model training pipeline.

### Data Preprocessing
Text data underwent the following preprocessing steps:
- Tokenization using the `Tokenizer` from Keras.
- Padding sequences to ensure uniform input length.
- Special tokens `<start>` and `<end>` were added to mark the beginning and end of sequences.

## Model Architecture
The translation model employs an encoder-decoder architecture tailored for sequence-to-sequence translation:
- **Encoder**: Embedding layer followed by LSTM layers.
- **Decoder**: Embedding layer and LSTM layers with attention mechanism for enhanced performance.
- Bidirectional layers were considered to capture bidirectional context.

### Design Choices
The architecture was designed to balance complexity and performance, with attention mechanisms implemented to improve translation accuracy.

## Training
The model was trained using the curated dataset:
- **Epochs**: 50
- **Batch Size**: 64
- **Optimizer**: Adam with default learning rate
- **Loss Function**: Categorical Cross-Entropy

### Hyperparameters
Hyperparameters were chosen based on empirical testing to optimize training efficiency and model performance.

## Evaluation
The model's performance was evaluated using the following metrics:
- **BLEU Score**: 6.66832382604621e-232

### Results
The BLEU score suggests a significant gap in n-gram overlaps, indicating areas for improvement in translation quality.

## Insights and Potential Improvements
Insights gained from the project include the need for:
- Further data augmentation to enhance dataset diversity.
- Experimentation with advanced model architectures such as Transformer-based models.
- Fine-tuning hyperparameters to optimize translation accuracy.



## Conclusion
In conclusion, this project laid the foundation for English to Kinyarwanda translation using RNNs, highlighting key steps in dataset creation, model architecture design, training, and evaluation. Future iterations will focus on addressing identified limitations to achieve higher translation accuracy.



