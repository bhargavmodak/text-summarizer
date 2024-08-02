<h1 align="center">Syntactic Text Summarizer</h1>

<!-- Languages -->
<p align="center">
    <img src="https://img.shields.io/badge/Language-Python-blue?style=for-the-badge&logo=python" alt="Language">
</p>

<p align="center">
A simple syntactic text summarizer that uses cosine similarity to find the most important sentences in a text.
</p>
<hr style="width:100px; margin: 1rem auto;">

![alt text](image.png)

**Note that it does not rephrase the sentences, but rather extracts the most important ones.** The summarizer uses the `nltk`, `numpy`, and `networkx` libraries to tokenize the text, remove stopwords, and create a graph of the sentences, respectively. The graph is then used to calculate the importance of each sentence based on the cosine similarity between the sentences. The sentences with the highest importance are then extracted and concatenated to form the summary.

## Table of Contents
- [Table of Contents](#table-of-contents)
- [Libraries](#libraries)
- [How to Run the Summarizer locally](#how-to-run-the-summarizer-locally)
    - [1. Clone the repository:](#1-clone-the-repository)
    - [2. Create a virtual environment (optional):](#2-create-a-virtual-environment-optional)
    - [3. Install the required libraries:](#3-install-the-required-libraries)
    - [4. Run the summarizer:](#4-run-the-summarizer)
- [Contributing](#contributing)

## Libraries
The following python libraries are used in this project:


| Library                                                   | Use in this Project                                                                                                                          |
| --------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| [numpy](https://numpy.org/)                               | Used for numerical operations and calculations.                                                                                              |
| [nltk](https://www.nltk.org/)                             | Used for natural language processing tasks such as tokenization and stopwords removal, and for deducing cosine similarity between sentences. |
| [networkx](https://networkx.org/)                         | Used for creating and manipulating graphs. And for Pagerank scores.                                                                          |
| [tkinter](https://docs.python.org/3/library/tkinter.html) | Used for creating the GUI.                                                                                                                   |


## How to Run the Summarizer locally

#### 1. Clone the repository:
```bash
git clone https://github.com/bhargavmodak/text-summarizer
```

#### 2. Create a virtual environment (optional):
```bash
cd text-summarizer
python3 -m venv venv
source venv/bin/activate
```

You can also use `conda` to create a virtual environment.

#### 3. Install the required libraries:
```bash
pip install -r requirements.txt
```

#### 4. Run the summarizer:
```bash
python text_summarizer.py
```

## Contributing

There is no dedicated support for this project. However, if you have any suggestions or find any bugs, feel free to open an issue or create a pull request. Alternatively, you can fork the repository and make changes as you see fit.