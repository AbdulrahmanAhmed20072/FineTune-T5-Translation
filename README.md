# Fine-Tuning T5 for English-to-French Translation

This repository fine-tunes T5-small for English-to-French translation using Parameter-Efficient Fine-Tuning (PEFT) with LoRA and BitsAndBytes quantization.

## Features

- **T5 Fine-Tuning**: Adapts T5-small for sequence-to-sequence translation.
- **LoRA & BitsAndBytes**: Efficient training with low-rank adaptation and 4-bit quantization.
- **Dataset Preparation**: Uses the OPUS Books dataset for training.
- **Training Pipeline**: Utilizes Hugging Face `Trainer` for efficient model training.
- **Evaluation**: Computes BLEU score and translation accuracy.

## Files

1. **`LoRA_BnB_T5_Translation.ipynb`**: Python script implementing the training pipeline.
2. **Dataset**: OPUS Books dataset for English-to-French translation.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/AbdulrahmanAhmed20072/FineTune-T5-Translation.git
   ```
2. Install the required dependencies:
   ```bash
   pip install datasets bitsandbytes accelerate evaluate transformers torch peft sacrebleu numpy
   ```

## Usage

1. Load and preprocess the dataset.
2. Fine-tune T5-small with LoRA and quantization.
3. Evaluate model performance.
4. Translate English text to French.

Run the script:
```bash
python LoRA_BnB_T5_Translation.ipynb
```

## Outputs

- Fine-tuned T5-small model for English-to-French translation.
- BLEU score evaluation on test data.
- Translations for input English sentences.

## Example

Input Sentence:
```
Hello, how are you?
```

Translated Output:
```
Bonjour, comment ça va ?
```
