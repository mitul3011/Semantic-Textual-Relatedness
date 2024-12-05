# Semantic Textual Relatedness
Semantic Textual Similarity (STS) refers to the degree to which two pieces of text (usually sentences or short passages) share the same meaning or convey similar information. The goal is to measure how semantically similar two texts are, regardless of their surface-level differences (like word choice or sentence structure).

For example, the sentences:

>"The dog is running in the park."

>"A dog is jogging in the park."

These two sentences might use different words ("running" vs. "jogging") but convey essentially the same meaning, so they would be considered highly semantically similar.

## Commands to Run the Code:
1. Download the code by running command:
   ```bash
   git clone https://github.com/mitul3011/Semantic-Textual-Relatedness.git
2. Change working directory to `pair_encoder` folder and install all pipeline dependencies:
   ```bash
   cd ../pair_encoder/
   pip install .
3. Change working directory again to `src` folder and install all the dependencies and libraries:
   ```bash
   cd ../src/
   pip install -r requirements.txt
4. Command to train the model with default parameters:
   ```bash
   python pairencoder_train.py 
5. Command to optimize the hyperparameters:
   ```bash
   python pairencoder_optimize.py

## Key Parameters
```
1.lang: Language code (eng, esp, etc.)
2.model_name: Pre-trained model name from HuggingFace
3.device: cpu or cuda
4.k: Number of nearest neighbors for augmentation (0-3)
5.epochs: Number of training epochs
6.learning_rate: Learning rate for training
