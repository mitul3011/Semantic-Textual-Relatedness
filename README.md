# Semantic Textual Relatedness
Two sentences are considered semantically similar when they have a paraphrasal or entailment relation. On the other hand, relatedness is a much broader concept that accounts for all the commonalities between two sentences: whether they are on the same topic, express the same view, originate from the same time period, one elaborates on (or follows from) the other, etc.

For example, the sentences:

>"There was a lemon tree next to the house."

>"The boy enjoyed reading under the lemon tree."

These two sentences are highly related.

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
```

## Dataset
Dataset can be found in the [`Semantic_Relatedness_SemEval2024`](https://github.com/mitul3011/Semantic-Textual-Relatedness/tree/main/Semantic_Relatedness_SemEval2024) folder.
