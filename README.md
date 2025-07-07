# Sentiment‑Analysis‑on‑Textual‑Data‑using‑OCR

A pipeline that extracts text from images using OCR and performs sentiment analysis on the extracted content. Combines computer vision and NLP to evaluate the tone of visual documents.

## 🔍 Description

This project scans images (like posters, screenshots, handwritten notes) and uses OCR to extract embedded text. The text is then passed to a sentiment analysis model to classify it as positive, negative, or neutral. This is useful for analyzing content in image-heavy domains like social media or scanned documents.

## 🛠️ Techniques

- **Tesseract OCR** is used to extract text from image input. More on [Tesseract OCR](https://github.com/tesseract-ocr/tesseract).
- **Text Preprocessing** includes tokenization, punctuation removal, and lowercasing using regular expressions.
- **TF-IDF Vectorization** to convert raw text into numerical features. See [MDN on TF-IDF](https://developer.mozilla.org/en-US/docs/Glossary/TF-IDF).
- **Naive Bayes classifier** trained to categorize text sentiment.
- Integration of image reading, OCR, preprocessing, vectorization, and prediction in a streamlined pipeline.

## 📦 Technologies & Libraries

- [Pytesseract](https://pypi.org/project/pytesseract/) – Python wrapper for Google Tesseract.
- [OpenCV](https://opencv.org/) – used to preprocess image files before OCR.
- [scikit-learn](https://scikit-learn.org/) – for TF-IDF and model training.
- [NLTK](https://www.nltk.org/) – optional support for extended text preprocessing and stop word handling.

## 🗂️ Project Structure

```
/
├── data/
├── images/
├── models/
├── notebooks/
├── src/
└── README.md
```

- **data/** – stores sample text data or preprocessed outputs.
- **images/** – input image files for OCR.
- **models/** – stores trained sentiment classifiers and vectorizers.
- **notebooks/** – experiments and development logs.
- **src/** – Python scripts for OCR, preprocessing, training, and sentiment inference.
