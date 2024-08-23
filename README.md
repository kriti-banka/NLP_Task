# Representations for Words, Phrases, Sentences

NLP encompasses various tasks - Regression, Classification, Generation. A common denominator across all these tasks is the question of "how do we convert text into numbers/representations" so that machines can process them. One way to measure a machine's ability to “understand” text is Semantic Similarity, i.e., one should be able to tell how similar or dissimilar are a given pair of text inputs. This is the central theme of this task. You are expected to come up with solutions to the problems listed below. For all the tasks, you can assess how well your solution is working based on some quantitative measures. You are expected to choose a metric that is suitable and justify the same.

## a. Word Similarity Scores

Given a pair of words, predict their similarity score. The focus is on how to convert a word to its numerical representation, on which learning algorithms (like Regression, Classification, etc.) can be applied. Download the dataset from [this link](#). You have to come up with an unsupervised/semi-supervised method to achieve the task. Assume that you don't have any supervised training data at your disposal. The whole dataset will be used as a test set. Choose an appropriate metric that is suitable to assess the task and report the results. You have to come up with a solution for each of the following conditions:

- **i. Constraints on Data Resources:** You can only use the following resources (any one or all) to solve the problem (DON’T USE PRE-TRAINED MODELS!):
  - Any monolingual English corpus - Maximum 1 million tokens.
  - Any curated/structured knowledge bases / ontologies.

- **ii. Unconstrained:** Consider that the constraints above are removed and you are allowed to use any data or model.

Compare results/analysis across the two settings. What works, what doesn’t? And Why?

## b. Phrase and Sentence Similarity

In question (1), you would have come up with a method to get numerical/vector representation for a word. Now you have to come up with a mechanism to get representations for phrases and sentences. How do you aggregate individual word representations to get phrase or sentence embeddings?

- You can use any pre-trained static word embeddings like word2vec, GLOVE, FASTTEXT, etc., or create your own.
- You can use popular tools/libraries (e.g., NLTK, Stanza, SpaCy, etc.) to compute linguistic features (PoS, Constituency/Dependency Parse).

- **i. Phrase Similarity:** Given a pair of phrases, classify whether or not they are similar. The dataset can be found [here](#). The dataset has train/dev/test splits. You have to report results on the test set and use train/dev sets as needed.

- **ii. Sentence Similarity:** Given a pair of sentences, classify whether or not they are similar. The dataset can be found [here](#). The dataset has train/dev/test splits. You have to report results on the test set and use train/dev sets as needed.

You are encouraged to try multiple approaches to come up with phrase/sentence representations and models to solve the task, and do comparative analysis. What are the cases where your model fails - any patterns? Why so?

## c. BONUS TASK

- **i. Transformers:** Transformers are all the rage right now (backbone of most of the LLMs you might have used). Can you fine-tune a pre-trained transformer-based model (BERT, Roberta, etc.) to solve Phrase and Sentence Similarity Tasks described above? You are free to use any resource out there.

- **ii. LLMs:** Can you prompt LLMs (ChatGPT, LLAMA) to solve the phrase and sentence similarity scores?
  - Solve the task using:
    - Commercial LLM APIs (ChatGPT, BARD, etc.).
    - Open-source LLMs/APIs (LLAMA, Mistral, etc.).
  - Try with zero and few-shot settings. If querying LLMs is computational/commercially prohibitive, do it for only the test set / subset of the test set.
  - Analyze the results. Explain some analysis that you have done.

- **iii. Comparison:** Compare all the approaches that you tried - static word embeddings, fine-tuned transformers, LLMs. What are the improvements you notice across the three settings?

## d. Paper Reading Task

- **BERTSCORE:** EVALUATING TEXT GENERATION WITH BERT

# Repository Contents

This repository contains the following files:

## Notebooks

1. **Phrases and Sentence Similarity.ipynb (bonus task is in this file)**
2. **Word Similarity.ipynb**

## PDFs

1. **Report for the Programming Task**
2. **Report for the Paper Reading Task**

[Datasets Used](https://drive.google.com/drive/folders/10lWwY823myX0pPTpg1Ym4cKLImJNLpBp?usp=sharing)
