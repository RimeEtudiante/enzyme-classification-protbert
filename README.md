# Enzyme Classification using ProtBERT

This project focuses on classifying enzymes into their top-level EC classes using only protein amino acid sequences.
We fine-tune the ProtBERT transformer model on curated UniProt protein data.

## Objective
- Classify protein sequences into 7 EC enzyme classes
- Use a transformer-based model (ProtBERT)
- Evaluate performance using Accuracy, Precision, Recall, and F1-score

## Dataset
- Source: UniProtKB (reviewed entries)
- Input: Protein amino acid sequences
- Labels: Top-level EC classes (1–7)

## Methodology
1. Data preprocessing and cleaning
2. Extraction of EC classes
3. Train/validation/test split
4. Tokenization using ProtBERT tokenizer
5. Fine-tuning ProtBERT for sequence classification
6. Model evaluation and visualization

## Model
- Pretrained model: `Rostlab/prot_bert`
- Architecture: Transformer-based encoder
- Task: Multi-class classification (7 classes)

## Evaluation Metrics
- Accuracy
- Precision (weighted)
- Recall (weighted)
- F1-score (weighted)
- Confusion matrices (validation and test sets)

## Results
The model achieves strong performance with:
- ~89–91% accuracy
- Balanced precision and recall across EC classes
- No strong signs of overfitting

## Files
- `*.ipynb`: Main training and evaluation notebook
- `figures/`: Loss curves and confusion matrices

## References
- Elnaggar et al., *ProtTrans: Towards Cracking the Language of Life’s Code Through Self-Supervised Deep Learning*
- UniProt Consortium, *UniProt: the universal protein knowledgebase*
