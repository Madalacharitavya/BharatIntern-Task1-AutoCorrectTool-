Explanation the code and how to use the Auto Correct Tool:

# Auto Correct Tool using NLTK

This Python script implements a simple Auto Correct Tool using the NLTK (Natural Language Toolkit) library. The tool takes an input sentence, identifies misspelled words, and suggests corrections based on the nearest word found in an English word list.

## Requirements

- Python 3.x
- NLTK (Natural Language Toolkit) library

## Setup

1. Install Python 3.x on your system if you haven't already.
2. Install the required NLTK library by running the following command in your terminal or command prompt:

```
pip install nltk
```

## Usage

1. Download the NLTK resources by running the following code snippet in your Python environment:

```python
import nltk
nltk.download('words')
nltk.download('punkt')
nltk.download('stopwords')
```

2. Import the necessary functions from the script:

```python
from auto_correct_tool import auto_correct_sentence
```

3. Prepare your input sentence as a string:

```python
input_sentence = "I am happpy to be here andd learrn neew things"
```

4. Use the `auto_correct_sentence` function to correct the sentence:

```python
corrected_sentence = auto_correct_sentence(input_sentence)
```

5. Print the original and corrected sentences:

```python
print(f"Original Sentence: {input_sentence}")
print(f"Corrected Sentence: {corrected_sentence}")
```

6. You should see the output displaying the original and corrected sentences.

## Customization

The script uses the NLTK English word list to find the nearest word for correction. If you have specific domain or jargon-related words, you can add them to the word list to improve the accuracy of the auto-correct tool.

To add custom words, you can extend the `english_words` set in the script:

```python
english_words.update({"customword1", "customword2", "customword3"})
```

By adding custom words, the auto-correct tool will consider them as valid words during the correction process.

## Note

This implementation is a simple demonstration of an auto-correct tool using edit distance and Jaccard similarity. The accuracy of the tool depends on the quality of the English word list and the methods used for similarity calculation. In practical applications, more sophisticated language models and context-aware techniques can be employed for better auto-correction performance.

Feel free to experiment and extend the code as needed for your specific use case.

## Author

This Auto Correct Tool was created by [NagaCharitavya Madala].

Output(DEMO)

https://github.com/Madalacharitavya/BharatIntern-Task1-AutoCorrectTool-/assets/102969979/a980bdd2-f296-45a4-8070-07e53c0cf746

## Contributing

Contributions are welcome! Feel free to open issues or pull requests.

## License

This project is licensed under the [MIT License](LICENSE).

