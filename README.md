# YouTube Transcript Summarizer

This repository contains two Jupyter notebooks designed to fetch YouTube video transcripts using an API, preprocess the text, and summarize the content using different techniques.

---

## Features

### Notebook 1: `YouTube Transcript Fetch and Summarize`
1. **Transcript Fetching**: Retrieves YouTube video transcripts using the `YouTubeTranscriptApi`.
2. **Summarization with Transformers**: Uses the `T5` model from Hugging Face Transformers to summarize the fetched transcript.
3. **Chunking for Long Texts**: Splits long transcripts into smaller chunks to comply with the model’s input length limitations.
4. **Output**: Provides a concise summary of the video content.

#### Key Libraries Used:
- `youtube-transcript-api`
- `transformers` (Hugging Face)

---

### Notebook 2: `YouTube Transcript Preprocess and Summarize`
1. **Transcript Fetching**: Retrieves YouTube video transcripts using the `YouTubeTranscriptApi`.
2. **Text Preprocessing**:
   - Removes special characters, extra spaces, and numbers.
   - Tokenizes the transcript into sentences and words.
   - Filters out common stopwords.
3. **Word Frequency Analysis**: Computes word frequencies to score sentences based on importance.
4. **Sentence Scoring and Extraction**: Identifies and extracts the most relevant sentences to create a summary.
5. **Output**: Provides a summary using traditional NLP techniques.

#### Key Libraries Used:
- `youtube-transcript-api`
- `nltk`
- `re`

---

## Getting Started

### Prerequisites
- Python 3.x
- Jupyter Notebook
- Required libraries:
  ```bash
  pip install youtube-transcript-api transformers nltk
  ```

---

## Demo
- Sample Video ID: `aDG1T0kJnd4`
- Input this ID when prompted to test the functionality of the notebooks.

---

## Acknowledgments
- Hugging Face Transformers for the `T5` model.
- NLTK for natural language processing utilities.
- `YouTubeTranscriptApi` for easy access to YouTube video transcripts.

