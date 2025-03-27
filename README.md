# Awesome Finnish NLP [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of awesome resources for Natural Language Processing in Finnish. This repository gathers tools, models, datasets, papers, and organizations working on Finnish NLP. Contributions are welcome!

## Contents

- [Corpora, datasets, word lists and lexicons](#corpora-datasets-word-lists-and-lexicons)
  - [Finnish corpus listings and repositories](#finnish-corpus-listings-and-repositories)
  - [Wordlists and lexicons](#wordlists-and-lexicons)
- [Pre-trained Models](#pre-trained-models)
  - [General Language Models](#general-language-models)
  - [Sentiment Analysis](#sentiment-analysis)
  - [Named Entity Recognition (NER)](#named-entity-recognition-ner)
- [Tools](#tools)
  - [Morphology & Parsers](#morphology-and-parsers)
  - [Universal Dependencies](#universal-dependencies)
  - [Semantic Similarity](#semantic-similarity)
- [Speech Technologies](#speech-technologies)
  - [Text-to-Speech (TTS)](#text-to-speech-tts)
  - [Speech-to-Text (STT)](#speech-to-text-stt)
- [Machine Translation](#machine-translation)
  - [Open-Source Models and Tools](#open-source-models-and-tools)
  - [Pipelines and Frameworks](#pipelines-and-frameworks)
  - [Commercial Machine Translation APIs](#commercial-machine-translation-apis)
- [LLMs for Finnish](#llms-for-finnish)
- [Organizations and notable users](#organizations-and-notable-users)
  - [Hugging Face](#hugging-face)
  - [Github](#github)
  - [Organizations](#organizations)
- [Papers](#papers)
- [Future Directions](#future-directions)
- [License](#license)


## Corpora, datasets, word lists and lexicons

### Finnish corpus listings and repositories

- [Kielipankki - The Language Bank of Finland](https://www.kielipankki.fi/aineistot/)
  - A national infrastructure providing access to Finnish and multilingual corpora for research.
- [European Language Grid: Finnish corpora](https://live.european-language-grid.eu/catalogue/?&language__term=Finnish&resource_type__term=Corpus)
  - A listing of Finnish corpora search results on ELG.
- [Kotus Aineistot Verkossa](https://kotus.fi/kotus/kieliaineistot/aineistot-verkossa/)
  - A collection of publicly available corpora and lexical resources from the Institute for the Languages of Finland (Kotus), including news, spoken language, dialects, and more.


### Multilingual datasets with a notable Finnish subset

| Dataset   | Description                                                                                                                                                     | Size   | Size, FI | Documents    | Documents, FI | Source                                                  |
|-----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|--------|----------|--------------|---------------|---------------------------------------------------------|
| CulturaX  | CulturaX is a multilingual dataset containing 6.3 trillion tokens across 167 languages, tailored for large language model development.                          | 27 TB  | 124 GB   | 7.2 billion  | 30.47 million | https://huggingface.co/datasets/uonlp/CulturaX          |
| C4        | A colossal, cleaned version of Common Crawl's web crawl corpus. Based on Common Crawl dataset                                                                   | 9.7 TB | 65 GB    | 10.3 billion | 26.8 million  | https://huggingface.co/datasets/allenai/c4              |
| HPLT 2.0  | Web-crawled multilingual corpora. The High-Performance Language Technologies (HPLT) project has released large-scale web-crawled corpora in multiple languages. | 15 TB  | 150 GB   | 10.6 billion | 34.8 million  | https://hplt-project.org/datasets/v2.0                  |
| Fineweb 2 | Fineweb 2 is the second iteration of the popular FineWeb dataset, bringing high quality pretraining data to over 1000 languages.                                | 7.9 TB | 56.8 GB  | 4.57 billion | 33.1 million  | https://huggingface.co/datasets/HuggingFaceFW/fineweb-2 |



### Wordlists and lexicons

- [Finnish Parsebank's Word Frequency List](http://dl.turkunlp.org/finnish-parsebank/)
  - Frequency list derived from the Finnish Internet Parsebank corpus, covering a wide range of Finnish word forms and lemmas.
- [Parole Corpus Frequency Lists](https://kaino.kotus.fi/sanat/taajuuslista/parole.php)
  - Word frequency lists compiled by Kotus from the Finnish PAROLE corpus — includes lemmas and part-of-speech information.


## Pre-trained Models

### General Language Models
- [FinBERT](https://github.com/TurkuNLP/FinBERT)
  - A BERT-based model pre-trained on Finnish corpora.

### Sentiment Analysis
- [FinBERT Finnish Sentiment](https://huggingface.co/fergusq/finbert-finnsentiment)
  - A FinBERT variant fine-tuned for sentiment analysis on Finnish texts, such as news or social media.

### Named Entity Recognition (NER)
- [FinBERT NER (Kansallisarkisto)](https://huggingface.co/Kansallisarkisto/finbert-ner)
  - Named entity recognition model trained on Finnish historical text for recognizing people, places, and dates.

- [Finnish NER by TurkuNLP](https://turkunlp.org/fin-ner.html)
  - NER pipeline developed using modern neural parsing tools for high-accuracy named entity recognition on contemporary Finnish.


## Tools

### Morphology and Parsers

- [Omorfi](https://flammie.github.io/omorfi/)
  - Omorfi is a free and open source project containing various tools and data for natural language processing of Finnish based on a knowledge driven paradigm.
- [UralicNLP](https://www.uralicnlp.com/)
  - A Python toolkit for NLP tasks in Uralic languages, including Finnish, with support for morphological analysis, disambiguation, and lemmatization using Omorfi and Giellatekno resources.
- [Turku Neural Parser Pipeline](https://turkunlp.org/Turku-neural-parser-pipeline/)
  - A neural parsing pipeline for Finnish and other languages, providing tokenization, lemmatization, POS tagging, dependency parsing, and NER.
- [SpaCy Finnish Model](https://spacy.io/models/fi) - Finnish language model for SpaCy.
  - A statistical pipeline for Finnish NLP in SpaCy, supporting tokenization, POS tagging, dependency parsing, lemmatization, and named entity recognition.


### Universal Dependencies

- [Finnish TDT](https://universaldependencies.org/treebanks/fi_tdt/index.html) - Universal Dependencies treebank for Finnish.
  - The Finnish Turku Dependency Treebank (TDT), a manually annotated treebank following the Universal Dependencies framework.


### Semantic Similarity

- [Semantic Similarity of Words](http://epsilon-it.utu.fi/wv_demo/)
  - A demo tool from University of Turku to explore cosine similarity between Finnish words using pre-trained word vector embeddings.


## Speech Technologies

### Text-to-Speech (TTS)

- [Piper](https://github.com/rhasspy/piper)
  - A fast, lightweight neural TTS engine with Finnish voice support, designed for offline use on CPUs and embedded devices.


### Speech-to-Text (STT)

- todo


## Machine Translation

### Open-Source Models and Tools

- [Opus-MT](https://github.com/Helsinki-NLP/Opus-MT)  
  Open-source neural machine translation models developed by Helsinki-NLP, covering a wide range of language pairs including Finnish.  
  → Models available at [Hugging Face: Helsinki-NLP](https://huggingface.co/Helsinki-NLP)

- [Facebook NLLB-200](https://ai.meta.com/research/no-language-left-behind/)  
  No Language Left Behind (NLLB-200) is a multilingual MT model supporting 200 languages, including Finnish. Designed to improve translation quality for low-resource languages.  
  → [Hugging Face: facebook/nllb-200-distilled-1.3B](https://huggingface.co/facebook/nllb-200-distilled-1.3B)

- [Apertium](https://apertium.org/)  
  A rule-based machine translation platform supporting Finnish–Estonian and other low-resource pairs. Lightweight, linguistically motivated, and fully open-source.


### Pipelines and Frameworks

- [OpenNMT](https://opennmt.net/)  
  A general-purpose neural machine translation framework. Finnish support depends on available training data (can be combined with OPUS datasets).

- [MarianNMT](https://marian-nmt.github.io/)  
  High-performance NMT framework used to train many Opus-MT models. Supports custom training for Finnish models using OPUS corpora.


### Commercial Machine Translation APIs

These are proprietary services that support Finnish, often used in production environments:

- [Google Cloud Translation](https://cloud.google.com/translate)
- [DeepL Translator](https://www.deepl.com/translator)
- [Microsoft Translator (Azure)](https://www.microsoft.com/en-us/translator/)  
- [Amazon Translate](https://aws.amazon.com/translate/)
- [Lingsoft MT Services](https://www.lingsoft.fi/en/solutions/language-services/translation)


## LLMs for Finnish

| Name    | Open-source | Available locally | Links |
|---------|-------------|-------------------|-------|
| ChatGPT | No          | No                | [ChatGPT](https://chatgpt.com/) |
| Gemma 3 | Yes         | Yes               | [Hugging Face](https://huggingface.co/collections/google/gemma-3-release-67c6c6f89c4f76621268bb6d), [Ollama](https://ollama.com/library/gemma3) |
| Gemini  | No          | No                | [Gemini](https://gemini.google.com) |
| Poro    | Yes         | Yes               | [Poro](https://huggingface.co/collections/LumiOpen/poro-34b-66506aaedb8d705069ad7ecb) |
| Viking  | Yes         | Yes               | [Viking](https://huggingface.co/collections/LumiOpen/viking-660fa4c659d8544c00f77d9b) |


## Organizations and notable users

### Hugging Face

- [TurkuNLP](https://huggingface.co/TurkuNLP)
  - Research group at the University of Turku specializing in Finnish NLP, creators of FinBERT, Turku parser, and other foundational tools.
- [Finnish-NLP](https://huggingface.co/Finnish-NLP)
  - A community-maintained collection of Finnish language models and datasets.
- [Kansallisarkisto](https://huggingface.co/Kansallisarkisto)
  - The Finnish National Archives’ repository for NER and NLP models trained on historical Finnish text.
- [Helsinki-NLP](https://huggingface.co/Helsinki-NLP)
  - Known for the OPUS project and multilingual machine translation models, including models supporting Finnish.
- [LumiOpen](https://huggingface.co/LumiOpen)
  - A collection of Finnish-capable open LLMs and evaluation tools trained and deployed on the LUMI supercomputer.


### Github

- todo


### Organizations

- [Kotus](https://kotus.fi/)
  - The Institute for the Languages of Finland — maintains official Finnish corpora, word lists, grammar guidelines, and other language resources.
- [Kielipankki](https://www.kielipankki.fi/)
  - The Language Bank of Finland — a national infrastructure providing access to Finnish and multilingual corpora for research.
- [TurkuNLP](https://turkunlp.org/)
  - Research group producing high-quality Finnish NLP tools, corpora, and pre-trained models.
- [HPLT Project](https://hplt-project.org/)
  - High-Performance Language Technologies project — aims to build open LLMs in European languages, including Finnish, using supercomputing resources.
- [ELG – European Language Grid](https://live.european-language-grid.eu/)
  - ELG contains tools and services, language resources and information on European LT companies and research organisations as well as their projects.


## Papers

A collection of interesting research papers related to Finnish NLP.

- [A Broad-coverage Corpus for Finnish Named Entity Recognition](http://www.lrec-conf.org/proceedings/lrec2020/pdf/2020.lrec-1.567.pdf)
- [An Expanded Massive Multilingual Dataset for High-Performance Language Technologies](https://arxiv.org/abs/2503.10267)

## Future Directions

- todo

---

This list aims to highlight the growing ecosystem of Finnish NLP tools and models. 
Maintained by [Jousia Piha](https://www.linkedin.com/in/jousia-piha/)

Contributions welcome! See [CONTRIBUTING.md](CONTRIBUTING.md) for details.

- todo

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
