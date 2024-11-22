# The Inclusivity Challenge in Automatic Speech Recognition for Indian Accents

## Introduction

Automatic Speech Recognition (ASR) has become an integral part of our daily lives, powering virtual assistants, live captioning, and audio transcription services. However, a significant challenge persists: the accurate recognition of diverse accents and dialects, particularly Indian English accents. This project explores the complexities of Indian English accents in ASR, the current state of research, and potential solutions to improve inclusivity in speech recognition technology.

## Understanding Indian English Accents

Indian English is characterized by a rich tapestry of accents influenced by the country's linguistic diversity. With 22 constitutionally recognized languages and numerous dialects, Indian English speakers exhibit a wide range of phonetic and phonological features that distinguish their speech from other English varieties.

### Key Features of Indian English Accents

1. **Consonants**: Indian English often uses retroflex plosives [ʈ] and [ɖ] instead of the alveolar plosives [t] and [d] found in American English
2. **Aspirated vs. Unaspirated Plosives**: Unlike American English, Indian English makes a clear distinction between aspirated and unaspirated sounds, which can change the meaning of words
3. **Vowels**: The central vowels [ə] (schwa) and [ʌ] are often not distinguished in traditional Indian English pronunciation
4. **Non-rhoticity**: Indian English is generally non-rhotic, meaning the 'r' at the end of words or before consonants is not pronounced, similar to British English
5. **Regional Variations**: Accents vary considerably based on the speaker's primary language and region, such as Bengali English, Southern Indian English, and Punjabi English

## The ASR Inclusivity Dilemma

Despite the advancements in ASR technology, models often struggle with accurately transcribing Indian English accents. This challenge stems from several factors:

1. **Data Bias**: Many ASR models are trained primarily on standard American or British English, leading to poor performance on Indian accents
2. **Linguistic Complexity**: The diverse phonetic and phonological features of Indian English pose a significant challenge for ASR systems
3. **Limited Resources**: There is a scarcity of large-scale, high-quality datasets representing the full spectrum of Indian English accents

## Current Research and Solutions

To address these challenges, researchers and organizations are working on various approaches:

### 1. The Svarah Dataset

The Svarah dataset is a significant step towards improving ASR for Indian English accents. Key features of this dataset include:

- 9.6 hours of transcribed English audio
- 117 speakers from 65 districts across 19 states in India
- Diverse range of accents reflecting 19 of 22 constitutionally recognized languages
- Both read speech and spontaneous conversational data
- Coverage of various domains and common use case scenarios

### 2. Advanced ASR Models

Researchers are exploring advanced ASR models that can better handle accent variations:

- **Whisper**: OpenAI's Whisper model, trained on 680,000 hours of multilingual data, shows promise in handling diverse accents
- **Wav2vec 2.0**: This self-supervised learning model has shown potential in adapting to various accents with limited labeled data

## Improving ASR Inclusivity: From Svarah to UF Indian Accent Dataset

The journey to create an inclusive Automatic Speech Recognition (ASR) system for Indian English speakers has led us through multiple iterations and improvements. Initially, we worked with the Svarah dataset, but analysis revealed a significant limitation: an overabundance of single-word recordings that made it difficult to extract meaningful accent features.

![Distribution of Speaker Audio Durations](Distribution.jpg)

The distribution graph above shows a clear spike in very short audio durations (0-2 seconds), indicating a predominance of single-word utterances that don't capture the natural flow and prosody of Indian-accented English speech.

### The Need for a New Approach

The limitations of the Svarah dataset prompted us to develop a more focused and structured data collection methodology. We're now gathering data from Indian students at the University of Florida using Qualtrics, ensuring longer, more natural speech samples that better capture accent characteristics.

### New Data Collection Framework

#### Survey Structure

Our new approach implements a comprehensive survey designed to collect:

- Detailed demographic information
- Educational background
- Linguistic history
- High-quality audio recordings

#### Recording Categories

The survey incorporates three distinct speech tasks:

- **Read Speech**: Carefully selected texts covering various domains
- **Extempore Speech**: Natural responses to familiar topics
- **Use Case Scenarios**: Real-world situation simulations

#### Participant Demographics

The new dataset focuses specifically on Indian students at UF, collecting detailed information about:

- Age and gender
- Educational qualifications
- Professional background
- Geographic origin within India
- Language background
- English acquisition history

#### Data Quality Controls

To ensure high-quality recordings, we've implemented strict guidelines:

- Quiet environment requirements
- Consistent microphone positioning
- Clear speaking instructions
- Quality verification through playback
- WAV format recordings for optimal audio quality

#### Privacy and Ethics

The new data collection process emphasizes:

- Voluntary participation
- Explicit consent requirements
- Data confidentiality
- Anonymous data aggregation
- Educational use restrictions

### Future Directions

This refined approach to data collection will enable:

- Better accent feature extraction
- More accurate ASR model training
- Improved understanding of Indian English variations
- Development of more inclusive speech recognition technology

The transition from Svarah to our new UF-focused dataset represents a significant step toward creating more accurate and inclusive ASR systems for Indian English speakers. By addressing the limitations of previous datasets and implementing a more structured collection methodology, we're building a foundation for better speech recognition technology.
