Image Integrity: Evaluating Caption-Image Consistency

📝 Overview

ImageIntegrity is an NLP and vision project that evaluates how well a caption matches the content of a given image. Our approach combines image captioning, object and action recognition, and multiple evaluation metrics to compute an integrity score between an image and its caption.

This project was developed as part of the coursework for CSCI 544: Applied Natural Language Processing at USC.

📌 Motivation

Textual descriptions of images can be incomplete, misleading, or outright false. Our goal is to automate the verification of image-caption pairs and determine if a caption accurately reflects the image content.

🎯 Objectives

Automatically generate captions from images using pretrained models.
Detect objects and actions in the image using visual recognition models.
Evaluate the semantic and factual consistency between the image and the provided caption.
Output a comprehensive integrity score using multiple NLP and vision metrics.

🧩 Pipeline

Input: Image and caption pair.
Image Captioning: Generate reference captions using [BLIP/BLIP-2].
Object Detection: Detect entities in the image using [BLIP/BLIP-2].
Action Recognition: Identify actions using [BLIP/BLIP-2].
Evaluation:
Rule-based consistency checks.
Metric-based scores: CLIPScore, BLEU, ROUGE-L, GPT-2 Perplexity.
QA-based evaluation via [TIFA].
Output: Integrity score and visual indicators.


📊 Evaluation Metrics

CLIPScore: Measures alignment between image and caption.
BLEU & ROUGE-L: Compare user caption to generated captions.
GPT-2 Perplexity: Language model coherence score.
Rule-based Evaluation: Checks object/action consistency.
TIFA Score: QA-based factual correctness evaluation.

🧠 Contributors

Jake Treska
Atharva Bhide
Cheryl Khau
Jeannie Jiang
Rahul Sura
