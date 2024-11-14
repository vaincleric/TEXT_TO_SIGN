
# Gest-Lingual: Sign Language Translation Model

## Abstract
Gest-Lingual is a Machine Learning (ML) model that translates input sentences into American Sign Language (ASL) representations. This model leverages Google’s T5 transformer to gloss input sentences by identifying key terms and filtering out unnecessary words. The glossed output is mapped to corresponding ASL gestures through a video library, utilizing the WLASL dataset for ASL gestures and Mediapipe for pose extraction. This approach optimizes the mapping process, providing efficient and accurate text-to-sign translations.

## Table of Contents
- [Introduction](#introduction)
- [Proposal](#proposal)
- [Key Features](#key-features)
- [Engines Used](#engines-used)
- [Architecture](#architecture)
- [Technical Challenges](#technical-challenges)
- [Future Enhancements](#future-enhancements)
- [Acknowledgments](#acknowledgments)

## Introduction
Sign language translation is crucial for accessibility, as over 466 million people worldwide rely on it for communication. Gest-Lingual aims to bridge the gap between spoken language and sign language by automating the translation process, creating an accessible solution for various sectors such as education, healthcare, and social interactions. The system combines Natural Language Processing (NLP) techniques, pose estimation algorithms, and a well-curated ASL dataset to output accurate ASL representations.

## Proposal
Current sign language translation tools either rely on human interpreters or automated systems that lack precision. Gest-Lingual proposes an ML-driven approach to translate English text into ASL by:
1. **Gloss-based Translation**: Glossing filters out non-essential words for clearer, more accurate translations.
2. **Pose-Based Gesture Recognition**: Mediapipe enables precise gesture recognition for fluid, natural sign language output.
3. **Comprehensive Dataset**: The WLASL dataset, enriched with Mediapipe pose points, ensures a broad vocabulary for accurate translations.

## Key Features
- **Efficient Text-to-ASL Translation**: Transforms glossed English text into ASL using a pre-existing video library.
- **Pose Estimation Integration**: Mediapipe pose data enhances gesture accuracy and fluidity.
- **Optimized Mapping**: Glossing reduces computational complexity and improves translation speed.

## Engines Used
- **T5 Model**: Used for glossing input sentences by identifying essential words, improving translation efficiency.
- **Mediapipe**: Extracts pose points from ASL videos, capturing precise body and hand movements for accurate sign language gestures.
- **WLASL Dataset**: A rich collection of over 2,000 ASL signs, forming the basis of the project’s sign language library.

## Architecture
1. **Input Processing**: Sentences are glossed using the T5 model.
2. **Gesture Mapping**: Glossed words are mapped to ASL gestures from a video library using WLASL and Mediapipe data.
3. **Output Generation**: Video clips are sequenced to form a coherent ASL representation of the input sentence.

## Technical Challenges
- Ensuring the glossing process preserves the semantic meaning of complex sentences.
- Achieving smooth transitions between video clips, requiring fine-tuning of sequence generation.

## Future Enhancements
- **Improved Natural Language Understanding**: Incorporate advanced models like GPT-4 for better glossing accuracy.
- **Support for Dialects**: Introduce personalization features to adapt gestures based on regional variations.
- **Integration with Assistive Technologies**: Compatibility with smart glasses or hearing aids for real-time ASL translation.

## Acknowledgments
Thanks to our mentor for guidance on WLASL and Mediapipe integration, and the Google Research team for the open-source T5 model and Mediapipe framework.

---
