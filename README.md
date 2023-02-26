# Text Summarization using TextRank Algorithm

This is a Python program that summarizes a text file by extracting the most important sentences using the TextRank algorithm. The program uses natural language processing techniques such as sentence tokenization, stop word removal, and word embeddings to create a similarity matrix of sentences. The program then calculates the importance of each sentence using TextRank and returns a summary of the most important sentences.

## Requirements
- Python 3.6 or later
- NumPy
- pandas
- NLTK
- Gensim
- SciPy
- NetworkX

## Installation
1. Install Python from the official website
2. Open a terminal or command prompt and install the required packages using the following command:
```
pip install numpy pandas nltk gensim scipy networkx
```

## Usage
1. Clone the repository or download the script `text_summarization.py`.
2. Place the text file you want to summarize in the same directory as the script.
3. Open the script in a code editor and modify the file name in the following lines to match the name of your text file:
```
file = open("example.txt", "r")
text = file.read()
```
4. Run the script using the following command:
```
python text_summarization.py
```
5. The program will output the total number of sentences and the summary length (number of sentences in the summary).
6. The program will then print the summary of the most important sentences.

## Customization
1. The program uses a default summary length of 20% of the total number of sentences. You can change this by modifying the following line:
```
summary_length = int(length/5)
```

2. The program uses a default epoch iteration of 2000 rounds in Word2Vec training model. You can change this value for more accurate summarization by modifying the following lines:
```
model = Word2Vec(sentence_tokens, vector_size=1, min_count=1, epochs=2000)
```
