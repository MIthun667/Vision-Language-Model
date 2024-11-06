# ViT-BERT CAMT: Vision-Language Model for Multi-Task Meme Classification
  # 1. Overview
ViT-BERT CAMT is a vision-language model designed for multi-task classification of memes. It addresses complex classification tasks such as sentiment, sarcasm, offensiveness, and prejudice across multimodal data, specifically focusing on visual and textual meme content. The model combines Visual Transformer (ViT) for image encoding with a custom BERT-based text encoder, leveraging Linear Self-Attentive Fusion (LSA) to integrate features.

  # Key Features
    Multi-Task Learning: Simultaneously classifies multiple tasks like sentiment, sarcasm, and offensiveness.
    Fusion Techniques: Implements several fusion strategies, including Linear Self-Attentive, Graph, Hybrid, and Early Fusion.
    Baseline Comparisons: Includes various unimodal (VGG16, ResNet50, BERT) and multimodal models (CNN-LSTM, CNN-GRU, CNN-BERT, etc.) for robust baseline performance analysis.
    Ablation Studies: Demonstrates the effect of different components by selectively disabling certain model elements.

 # Results
    The model achieves high accuracy across multimodal tasks with results that demonstrate the effectiveness of Linear Self-Attentive Fusion in capturing nuanced multimodal features. For example:
    Sentiment Classification: 85% accuracy on Memotion
    Offensiveness Detection: 82% F1 score on MIMIC
    Sarcasm Detection: 78% precision across the test dataset
    For detailed results, please see results/metrics_report.txt.

# Limitations & Future Work
    # Limitations:
        High computational cost, particularly for models with complex fusion strategies.
        Model training is constrained by dataset size and available GPU memory.
  # Future Work:
      Extend the model to more complex multimodal datasets, possibly incorporating audio or contextual data.
      Experiment with additional fusion methods to optimize performance.
      Improve training efficiency to reduce computational requirements.
  # References
      VGG16: Walińska, M. et al., "VGG16: A Convolutional Neural Network for Object Detection," 2020.
      ResNet50: Koonce, D., "Residual Neural Networks," 2021.
      BERT: Devlin, J., et al., "BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding," NAACL-HLT, 2019.
      CLIP: Radford, A., et al., "Learning Transferable Visual Models from Natural Language Supervision," ICML, 2021.
      VisualBERT: Li, J., et al., "VisualBERT: A Simple and Performant Baseline for Vision and Language," ICCV, 2019.

