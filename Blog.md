# The Inclusivity Challenge in Automatic Speech Recognition for Indian Accents: Bridging the Gap

Imagine a world where your voice assistant understands you perfectly, regardless of your accent. For millions of Indian English speakers, this dream remains elusive. Let's dive into the fascinating world of Automatic Speech Recognition (ASR) and explore how we are working to make this technology truly inclusive.

## Introduction

ASR has become an integral part of our daily lives, powering virtual assistants, live captioning, and audio transcription services. However, a significant challenge persists: the accurate recognition of diverse accents and dialects, particularly Indian English accents. In this blog we will explore the aspects, key features and complexities of Indian accented english, the current state of research, why we need new datasets and how to use the new datasets to potentially improve inclusivity of Indian accents in speech recognition technology.

## The Colorful Tapestry of Indian English

India's linguistic landscape is extraordinarily diverse, with 22 officially recognized languages and hundreds of dialects. This diversity has given birth to a unique variety of English, characterized by a wide range of accents and pronunciation patterns. Indian English speakers exhibit a wide range of phonetic and phonological features that distinguish their speech from other English varieties.

<p align="center"> <img src="https://github.com/Aryaan03/Independent-Study/blob/main/Indian%20Lang%20Dist.png" alt="Most Commonly Spoken Native Languages in India" style="width: 80%;"> </p> <p align="center"><em>Source: statsofIndia.in by @PratapVardhan</em></p> 

### Key Features of Indian English Accents

#### 1. Consonant Variations

i) **"Curled Tongue" Sounds**:

- Indian English speakers often use sounds made with the tongue curled back (called retroflex consonants) in place of regular "t" and "d" sounds [1].<br>
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
  - Some double vowel sounds (diphthongs) are simplified to single vowels [2].
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

## Regional Variations
Apart form the above distinctions, Indian Accents also vary considerably based on the speaker's primary language and region, such as Bengali English, Southern Indian English, and Punjabi English. [Link](https://en.wikipedia.org/wiki/Regional_differences_and_dialects_in_Indian_English)

#### I. Tamil-influenced English

- Strong "r" sound and distinct vowel qualities
- Example: "Very" might sound more like "wery"
- Tendency to add an "a" sound at the end of questions
- Clear pronunciation of "r" sounds throughout words
- Stress on syllables, giving a rhythmic quality to speech

#### II. Bengali-influenced English

- Softer "v" sound and distinct vowel qualities
- Example: "Love" might sound more like "lobe"
- Tendency to replace "z" sounds with "j" sounds (e.g., "jero" for "zero")
- Emphasis often placed on the second syllable of words (e.g., "tea-CHER" instead of "TEA-cher")
- Melodic and soft-spoken quality compared to other Indian accents

#### III. Punjabi-influenced English

- Loud and boisterous accent, common in northern India
- Clear pronunciation of "r" sounds
- Tendency to use retroflex "t" and "d" sounds (tongue curled back)
- Example: "Tea" pronounced with the tongue curled back for the "t" sound
- Often emphasize syllables like "ji" instead of "jee"

#### IV. Marathi-influenced English

- Non-aspirated "p" and "b" sounds
- Clear distinction between "v" and "w" sounds
- Tendency to drop the final consonant in many words
- Example: The "th" in words like "thigh" often pronounced as "d"
- Generally more relaxed and laid-back tone of speech

#### V. Telugu-influenced English

- Words often end in vowel sounds
- No contrastive stress, but emphasis usually on the final syllable
- Pronounced "sh" sounds influenced by Telugu
- Less aspirated "p" and "b" sounds
- Distinct intonation patterns different from other Indian English varieties

#### VI. Hindi-influenced English

- Intonation pattern influenced by Hindi phonetics
- Difficulty pronouncing certain English sounds, like "th" in "thought"
- Clear pronunciation of "r" and "i" sounds
- Less nasalization compared to some other Indian English varieties
- Tendency to use Hindi sentence structures in English

These variations make Indian English a rich and diverse dialect, reflecting India's linguistic diversity.

## The ASR Inclusivity Dilemma

Despite the advancements in ASR technology, models often struggle with accurately transcribing Indian English accents. This challenge stems from several factors:

1. **Data Bias**: Most commercial ASR systems are trained primarily on American and British English datasets, leading to poor performance on Indian accents. This bias results in higher error rates and frustration for Indian English speakers.
2. **Linguistic Complexity**: The phonetic and phonological features of Indian English, influenced by the country's diverse languages, create a complex landscape for ASR systems to navigate. Features like retroflex consonants, vowel peculiarities, unique stress patterns and regional variations are often misinterpreted.
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

## Improving ASR Inclusivity: From SVARAH to UFIND Accent Dataset

The journey to create an inclusive Automatic Speech Recognition (ASR) system for Indian English speakers has led us through multiple iterations and improvements. Initially, we worked with the Svarah dataset, but analysis revealed a significant limitation: an overabundance of single-word recordings that made it difficult to extract meaningful accent features.

### The Need for a New Approach

<p align="center"> <img src="https://github.com/Aryaan03/Independent-Study/blob/main/Distribution_Plot.png" alt="Distribution of Speaker Audio Durations" style="width: 80%; max-width: 800px;"> </p> <p align="center"><em>Distribution of Speaker Audio Durations</em></p> 

This distribution graph above shows a clear spike in very short audio durations (0-5 seconds), which is a significant limitation in the dataset. The overabundance of very short recordings makes it challenging to capture the natural rhythm, intonation, and connected speech patterns that are crucial for understanding and modeling Indian-accented English. Longer recordings would be more valuable for capturing these prosodic features and natural speech variations.

This limitation of the Svarah dataset prompted us to develop a more focused and structured data collection methodology. We're now gathering data from Indian students at the University of Florida using Qualtrics, ensuring longer, more natural speech samples that better capture accent characteristics.

## New Data Collection Framework

### Survey Structure

Our new approach implements a comprehensive survey designed to collect:

- Detailed demographic information
  - Age and gender
  - Educational qualifications
  - Professional background
  - Geographic origin within India
  - Language background
- English acquisition history
- Educational background
- Linguistic history
- Primary Langauges
- High-quality audio recordings

### Recording Categories

The survey incorporates three distinct speech tasks:

- **Read Speech**: Carefully selected texts covering various domains
- **Extempore Speech**: Natural responses to familiar topics
- **Use Case Scenarios**: Real-world situation simulations

### Data Quality Controls

To ensure high-quality recordings, we've implemented strict guidelines:

- Quiet environment requirements
- Clear speaking instructions
- Quality verification through playback
- WAV format recordings for optimal audio quality

### Privacy and Ethics

The new data collection process emphasizes:

- Voluntary participation
- Explicit consent requirements
- Data confidentiality
- Anonymous data aggregation
- Educational use restrictions

## Future Directions

Our journey from SVARAH to UFIND (UF Indian Dataset) marks a pivotal shift in ASR development for Indian English. The distribution analysis clearly shows why this transition is crucial - while SVARAH was dominated by short 0-2 second utterances, our new methodology ensures longer, more natural speech samples.

#### Current Progress

- Collected approximately 100 responses
- On track to reach our target of 250 responses
- Projected raw audio data: 10.5 hours

#### Immediate Goals

- Data Collection Enhancement
  - Targeting 150 additional responses
  - Focus on extracting features of Indian English Accents
  - Ensuring diverse regional representation

- Model Development
  - Fine-tuning Whisper model with collected data
  - Optimizing for Indian English variations
  - Implementing accent-specific adaptations

## Join Our Research: Help Improve Speech Recognition for Indian Accents
As our distribution analysis shows, we need more diverse and natural speech samples to build better ASR systems. If you are of Indian origin and would like to contribute to making speech technology more inclusive, we welcome your participation in our research.

### How You Can Help
You can participate in our data collection by taking a brief survey that includes:

- Recording natural speech samples
- Providing demographic information
- Sharing your linguistic background

The survey takes approximately 7-10 minutes to complete, and your contribution will help develop more accurate speech recognition systems for Indian English speakers.

### Participation Requirements

- Must be of Indian origin
- Comfortable speaking English
- Access to a quiet environment and a working microphone
- Willing to provide anonymous demographic information

To participate in this research and help make speech technology more inclusive, please visit: [Survey Link](https://ufl.qualtrics.com/jfe/form/SV_bsypey1tUeqAic6) 
<br> Your participation will be completely voluntary and confidential, contributing to the development of more accurate and inclusive speech recognition technology.



## References 

[1] Sirsa, H., & Redford, M. A. (2013). The effects of native language on Indian English sounds and timing patterns. Journal of Phonetics, 41(6), 393-406. https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4028080/<br>
[2] Jain, S., Pal, P., Vuppala, A. K., Ghosh, P. K., & Yarra, C. (2023). An Investigation of Indian Native Language Phonemic Influences on English Pronunciations. ISCA Archive. https://www.isca-archive.org/interspeech_2023/jain23b_interspeech.pdf<br>
[3] Grolman, M. B., Biktagirova, Z. A., & Kasimov, O. H. (2021). Phonetic Peculiarities of the English Language in India. International Journal of Society, Culture & Language. https://www.ijscl.com/article_241951_a15237d176e59f6236b49c3389015f63.pdf<br>
[4] Jiang, Y. (2023). A Study on the Influence of Mother Tongue Transfer on English Pronunciation of Primary Students. Open Journal of Modern Linguistics, 13(1), 49-59. https://www.scirp.org/journal/paperinformation?paperid=128933<br>
[5] Jain, M., & Yadav, D. (2023). An investigation of Indian native language phonemic influences on Indian English pronunciation. Interspeech 2023. Retrieved from https://www.isca-archive.org/interspeech_2023/jain23b_interspeech.pdf<br>
[6] Grolman, M. B., Biktagirova, Z. A., & Kasimov, O. H. (2022). Phonetic peculiarities of the English language in India. International Journal of Society, Culture & Language. Retrieved from https://www.ijscl.com/article_241951_a15237d176e59f6236b49c3389015f63.pdf<br>
[7] Tarun, M., Israr, A., & Gajwal, D. (2022). Analysis of the factors influencing Indian English accents, and how pronunciation and articulation fill the accent gap. EPRA International Journal of Environmental Economics, Commerce and Educational Management. Retrieved from https://eprajournals.com/IJCM/article/6876/download<br>
[8] Propósitos y Representaciones. (2021). Peculiarities of Indian English as a separate language. ERIC. https://files.eric.ed.gov/fulltext/EJ1298339.pdf<br>
[9] Reppen, R. (n.d.). Teaching Children to Unlearn the Sounds of English. Northern Arizona University. https://jan.ucc.nau.edu/~jar/TIL_4.html 3<br>
[10] Wikipedia. (n.d.). Non-native pronunciations of English. https://en.wikipedia.org/wiki/Non-native_pronunciations_of_English

