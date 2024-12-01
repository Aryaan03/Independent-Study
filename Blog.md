# The Inclusivity Challenge in Automatic Speech Recognition for Indian Accents: Bridging the Gap

Imagine a world where your voice assistant understands you perfectly, regardless of your accent. For millions of Indian English speakers, this dream remains elusive. Let's dive into the fascinating world of Automatic Speech Recognition (ASR) and explore how we are working to make this technology truly inclusive.

## Introduction

ASR has become an integral part of our daily lives, powering virtual assistants, live captioning, and audio transcription services. However, a significant challenge persists: the accurate recognition of diverse accents and dialects, particularly Indian English accents. In this blog we will explore the aspects, key features and complexities of Indian accented english, the current state of research, why we need new datasets and how to use the new datasets to potentially improve inclusivity of Indian accents in speech recognition technology.

## The Colorful Tapestry of Indian English

India's linguistic landscape is extraordinarily diverse, with 22 officially recognized languages and hundreds of dialects. This diversity has given birth to a unique variety of English, characterized by a wide range of accents and pronunciation patterns. Indian English speakers exhibit a wide range of phonetic and phonological features that distinguish their speech from other English varieties.

![Most Commonly Spoken Native Languages in India](https://github.com/Aryaan03/Independent-Study/blob/main/Indian%20Lang%20Dist.png)
*Source: statsofIndia.in by @PratapVardhan*

### Key Features of Indian English Accents

#### 1. Consonant Variations

i) **"Curled Tongue" Sounds**:

- Indian English speakers often use sounds made with the tongue curled back (called retroflex consonants) in place of regular "t" and "d" sounds.<br>
- Example: The word "tea" might sound like "tea" but with the tongue curled back for the "t" sound.<br>
- To understand this, try saying "tea" while curling your tongue tip backwards and touching the roof of your mouth.<br>

ii) **'V/W' Confusion**:

- The difference between "v" and "w" sounds is often unclear.<br>
- Example: "Vine" might sound like "wine" and vice versa.<br>
- Think of saying "very well" as "wery vell".<br>

#### 2. Vowel Peculiarities
The central vowels [ə] (schwa) and [ʌ] are often not distinguished in traditional Indian English pronunciation

  i) **Full Vowel Sounds**:
  - Short, unstressed vowels (like the "a" in "about") are often pronounced as full, clear vowels.
  - Example: "About" might be pronounced as "a-bout" with both vowels clearly heard.
  - Imagine saying "a-bout" with equal stress on both parts.

  ii) **Simplified Double Vowels**:
  - Some double vowel sounds (diphthongs) are simplified to single vowels.
  - Example: "Go" might be pronounced more like "goh" without the subtle "uh" sound at the end.

#### 3. Stress and Intonation

  i) **Equal Syllable Stress**:
  - Each syllable tends to receive equal stres
  - Example: "Computer" might be pronounced as "com-pu-ter" with equal emphasis on each part.
   
  ii) **Different Word Stress**:
  - The emphasized part of longer words may differ from standard English.
  - Example: "DEvelop" might be pronounced as "deveLOP".

#### 4. Breath Distinctions
Indian English often makes a clear difference between sounds pronounced with or without a puff of air (aspiration), which isn't common in other English varieties. 

  i) **Sounds Without Puffs**:
  - The "p", "t", and "k" sounds are often said without a puff of air.
  - Example: "Pin" might sound more like "bin" to non-Indian ears.
  - Try saying "pin" without blowing air at the start.
  
  ii) **Sounds With Strong Puffs:**
  - Some Indian languages have versions of sounds with extra strong puffs of air.
  - Example: Imagine saying "pin" with an extra strong puff of air after the "p".

#### 5. Regional Variations
Accents vary considerably based on the speaker's primary language and region, such as Bengali English, Southern Indian English, and Punjabi English.

 i) **Tamil-influenced English**:
  - Often has a strong "r" sound and certain vowel changes.
  - Example: "Very" might sound more like "wery".
 
 ii) **Bengali-influenced English**:
  - Often has a softer "v" sound and distinct vowel qualities.
  - Example: "Love" might sound more like "lobe".

These variations make Indian English a rich and diverse dialect, reflecting India's linguistic diversity.

1. **Consonants**: Indian English often uses retroflex plosives [ʈ] and [ɖ] instead of the alveolar plosives [t] and [d] found in American English
2. **Aspirated vs. Unaspirated Plosives**: Unlike American English, Indian English makes a clear distinction between aspirated and unaspirated sounds, which can change the meaning of words
3. **Vowels**: The central vowels [ə] (schwa) and [ʌ] are often not distinguished in traditional Indian English pronunciation
4. **Non-rhoticity**: Indian English is generally non-rhotic, meaning the 'r' at the end of words or before consonants is not pronounced, similar to British English
5. **Regional Variations**: Accents vary considerably based on the speaker's primary language and region, such as Bengali English, Southern Indian English, and Punjabi English

## The ASR Inclusivity Dilemma

Despite the advancements in ASR technology, models often struggle with accurately transcribing Indian English accents. This challenge stems from several factors:

1. **Data Bias**: Most commercial ASR systems are trained primarily on American and British English datasets, leading to poor performance on Indian accents. This bias results in higher error rates and frustration for Indian English speakers.
2. **Linguistic Complexity**: The phonetic and phonological features of Indian English, influenced by the country's diverse languages, create a complex landscape for ASR systems to navigate. Features like retroflex consonants and unique stress patterns are often misinterpreted.
3. **Limited Resources**: There is a scarcity of large-scale, high-quality datasets that represent the full spectrum of Indian English accents. This lack of training data hampers the development of more inclusive ASR models.

## Current Research and Solutions
Researchers and organizations are actively working to address these challenges through various approaches:

### 1. The SVARAH Dataset

The SVARAH dataset represents a significant step towards improving ASR for Indian English accents. Key features include::

- 9.6 hours of transcribed English audio
- 117 speakers from 65 districts across 19 states in India
- Diverse range of accents reflecting 19 of 22 constitutionally recognized languages
- Both read speech and spontaneous conversational data
- Coverage of various domains and common use case scenarios

While Svarah is a valuable resource, it has limitations, particularly an overabundance of single-word recordings that don't fully capture the nuances of connected speech.

### 2. Advanced ASR Models

Researchers are exploring advanced ASR models that can better handle accent variations:

- **Whisper**: OpenAI's Whisper model, trained on 680,000 hours of multilingual data, shows promise in handling diverse accents
- **Wav2vec 2.0**: This self-supervised learning model has shown potential in adapting to various accents with limited labeled data

## Improving ASR Inclusivity: From Svarah to UF Indian Accent Dataset

The journey to create an inclusive Automatic Speech Recognition (ASR) system for Indian English speakers has led us through multiple iterations and improvements. Initially, we worked with the Svarah dataset, but analysis revealed a significant limitation: an overabundance of single-word recordings that made it difficult to extract meaningful accent features.

![Distribution of Speaker Audio Durations](https://github.com/Aryaan03/Independent-Study/blob/main/Distribution.png)

The distribution graph above shows a clear spike in very short audio durations (0-5 seconds), indicating a predominance of single-word utterances that don't capture the natural flow and prosody of Indian-accented English speech.

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
