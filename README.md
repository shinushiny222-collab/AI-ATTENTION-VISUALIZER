# AI Attention Visualizer

## Project Overview

AI Attention Visualizer is a Streamlit-based application that extracts text from an uploaded image and visualizes word-level attention scores.

The project demonstrates the basic workflow of text processing, word embeddings, and attention calculation.

## Demo
https://ai-attention-visualizer-wgdudt3jhwhplptsva28rd.streamlit.app/

## Features

- Upload JPG, JPEG, and PNG images
- Extract text from images using OCR
- Process extracted text into individual words
- Remove punctuation and short words
- Generate word embeddings
- Calculate attention scores
- Display attention scores for each word
- Visualize attention using progress bars
- Identify the word with the highest attention score

## Technologies Used

- Python
- Streamlit
- NumPy
- Pillow
- Pytesseract
- Sentence Transformers

## Project Structure

```text
AI Attention Visualizer/
│
├── app.py
├── ocr.py
├── embedding.py
├── attention.py
├── requirements.txt
└── README.md

## How It Works

The application follows these steps:

Image Upload
     |
     v
OCR Text Extraction
     |
     v
Text Processing
     |
     v
Word Embeddings
     |
     v
Attention Calculation
     |
     v
Attention Score Visualization
     |
     v
Highest Attention Word

## Step 1: Upload Image

The user uploads an image containing text.

Supported image formats:

JPG
JPEG
PNG

## Step 2: Text Extraction

The application uses Optical Character Recognition to extract text from the uploaded image.

The extracted text is displayed in the application.

## Step 3: Word Processing

The extracted text is split into individual words.

Punctuation marks are removed, and words with two or fewer characters are filtered out.

The application processes a maximum of 20 words.

## Step 4: Word Embeddings

Each word is converted into a numerical vector representation called an embedding.

Embeddings allow words to be represented mathematically so that they can be used for further processing.

## Step 5: Attention Calculation

The generated embeddings are passed to the attention calculation function.

An attention score is calculated for each word.

A higher score indicates a higher relative attention value according to the implemented attention calculation.

## Step 6: Attention Visualization

The attention scores are normalized between 0 and 1.

Streamlit progress bars are used to visually represent the relative attention of each word.

## Example:

computer - 92.45%
██████████████████

artificial - 75.30%
███████████████

intelligence - 61.20%
████████████

## Step 7: Highest Attention Word

NumPy is used to find the word with the highest attention score.

## The application displays:

Highest Attention Word
Attention Score
Total Number of Words
Installation

## Clone the repository:

git clone https://github.com/your-username/AI-Attention-Visualizer.git

## Move into the project directory:

cd "AI Attention Visualizer"

Install the required Python packages:

python -m pip install -r requirements.txt
Requirements

## Run the Streamlit application using:

python -m streamlit run app.py

## Example Input

An image containing text such as:

Artificial Intelligence
Machine Learning
Data Science

can be uploaded to the application.

## Example Output

The application displays:

## Extracted Text

Artificial Intelligence
Machine Learning
Data Science

Then it generates embeddings and attention scores for the processed words.

The word with the highest attention score is displayed in the Attention Summary section.

## Applications

This project can be used for:

Learning OCR
Understanding word embeddings
Learning the basic concept of attention
Visualizing NLP concepts
Demonstrating AI and NLP concepts
Educational projects and presentations
Future Enhancements

## Possible improvements include:

Interactive attention heatmaps
Transformer-based attention visualization
Multi-language OCR support
Sentence-level attention visualization
Downloadable attention reports
Visualization using charts
Support for PDF documents

## Conclusion

AI Attention Visualizer provides a simple way to understand how text extracted from an image can be converted into word embeddings and processed to calculate and visualize attention scores.

The project combines OCR, natural language processing, embeddings, and Streamlit into a single interactive application.
