# Awesome Finnish NLP [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of awesome resources for Natural Language Processing in Finnish. This repository gathers tools, models, datasets, papers, and organizations working on Finnish NLP. Contributions are welcome!

## Contents

- [Corpora, datasets, word lists and lexicons](#corpora-datasets-word-lists-and-lexicons)
  - [Finnish corpus listings and repositories](#finnish-corpus-listings-and-repositories)
  - [Manually annotated Finnish corpora](#manually-annotated-finnish-corpora)
  - [Popular Finnish corpora](#popular-finnish-corpora)
  - [Other Finnish datasets](#other-finnish-datasets)
  - [Evaluation datasets](#evaluation-datasets)
  - [Multilingual datasets with a notable Finnish subset](#multilingual-datasets-with-a-notable-finnish-subset)
  - [Wordlists and lexicons](#wordlists-and-lexicons)
  - [Finnish speech corpora](#finnish-speech-corpora)
- [Pre-trained Models](#pre-trained-models)
  - [General Language Models](#general-language-models)
  - [Sentiment Analysis](#sentiment-analysis)
  - [Named Entity Recognition (NER)](#named-entity-recognition-ner)
- [Tools](#tools)
  - [Morphology and Parsers](#morphology-and-parsers)
  - [Universal Dependencies](#universal-dependencies)
  - [Sentiment and Semantic Similarity](#sentiment-and-semantic-similarity)
- [Speech Technologies](#speech-technologies)
  - [Text-to-Speech (TTS)](#text-to-speech-tts)
  - [Speech-to-Text (STT)](#speech-to-text-stt)
- [Machine Translation](#machine-translation)
  - [Open-Source Models and Tools](#open-source-models-and-tools)
  - [Pipelines and Frameworks](#pipelines-and-frameworks)
  - [Commercial Machine Translation APIs](#commercial-machine-translation-apis)
- [LLMs for Finnish](#llms-for-finnish)
- [Organizations and notable users](#organizations-and-notable-users)
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
- [Finnish corpora at Leipzig Corpora Collection](https://wortschatz.uni-leipzig.de/en/download/Finnish)

### Manually annotated Finnish corpora

- Treebanks ([See the comparison table](https://github.com/JousiaPiha/awesome-finnish-nlp/blob/main/treebank-comparison.md))
  - [Turku Dependency Treebank](https://github.com/UniversalDependencies/UD_Finnish-TDT)
    - A high-quality, manually annotated treebank of diverse real-world Finnish texts, designed for NLP applications and closely aligned with Universal Dependencies guidelines.
  - [FinnTreeBank 1](https://github.com/UniversalDependencies/UD_Finnish-FTB)
    - A treebank of grammatical example sentences adapted from the VISK grammar, automatically converted to Universal Dependencies with partial manual revision.
- NER corpora ([See the comparison table](https://github.com/JousiaPiha/awesome-finnish-nlp/blob/main/ner-comparison.md))
  - [Turku NER corpus](https://github.com/TurkuNLP/turku-ner-corpus)
    - A broad-coverage Finnish NER corpus with six entity types, built on top of the Turku Dependency Treebank, aiming to improve domain-general NER performance.
  - [TurkuONE](https://github.com/TurkuNLP/turku-one)
    - An extended, fine-grained NER corpus for Finnish using the OntoNotes entity schema, designed for bilingual and cross-lingual modeling by combining and refining Turku NER and FiNER annotations.
  - [Finer](https://github.com/mpsilfve/finer-data)
    - A manually annotated NER corpus of Finnish technology news articles with six entity types and support for nested annotation, developed alongside the rule-based FINER tool.

### Monolingual Finnish corpora

- [Suomi24 Corpus](https://www.kielipankki.fi/corpora/suomi24/)
- [Yle News Archive](https://www.kielipankki.fi/corpora/ylenews/)
- [Finnish subreddits available here](https://the-eye.eu/redarcs/)
  - Notably r/suomi submissions and comments
- [Newspaper and Periodical Corpus of the National Library of Finland](https://www.kielipankki.fi/corpora/klk/)
- [Finnish News Agency Archive](https://www.kielipankki.fi/corpora/stt-fi/)
- [The Finnish Web Corpus (fiTenTen)](https://www.sketchengine.eu/fitenten-finnish-corpus/)
- [Finnish news and web crawls, and Wikipedia](https://wortschatz.uni-leipzig.de/en/download/Finnish)

### Parallel and Multilingual Corpora (Finnish–Other Languages)

- todo


### Other Finnish datasets

- [SemFi](https://zenodo.org/records/1463685)


### Evaluation datasets

- todo


### Multilingual datasets with a notable Finnish subset

| Dataset   | Description                                                                                                                                                     | Size   | Size, FI | Documents    | Documents, FI | Source                                                  |
|-----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|--------|----------|--------------|---------------|---------------------------------------------------------|
| C4        | A colossal, cleaned version of Common Crawl's web crawl corpus. Based on Common Crawl dataset                                                                   | 9.7 TB | 65 GB    | 10.3 billion | 26.8 million  | https://huggingface.co/datasets/allenai/c4              |
| CulturaX  | CulturaX is a multilingual dataset containing 6.3 trillion tokens across 167 languages, tailored for large language model development.                          | 27 TB  | 124 GB   | 7.2 billion  | 30.47 million | https://huggingface.co/datasets/uonlp/CulturaX          |
| Fineweb 2 | Fineweb 2 is the second iteration of the popular FineWeb dataset, bringing high quality pretraining data to over 1000 languages.                                | 7.9 TB | 56.8 GB  | 4.57 billion | 33.1 million  | https://huggingface.co/datasets/HuggingFaceFW/fineweb-2 |
| HPLT 2.0  | Web-crawled multilingual corpora. The High-Performance Language Technologies (HPLT) project has released large-scale web-crawled corpora in multiple languages. | 15 TB  | 150 GB   | 10.6 billion | 34.8 million  | https://hplt-project.org/datasets/v2.0                  |
| Oscar     | The OSCAR project is an open-source initiative offering multilingual unannotated web resources and datasets for Machine Learning. | - | 41.1 GB | - | 14.5 million | https://oscar-project.github.io/documentation |


### Wordlists and lexicons

- [Kotus Modern Finnish Word List](https://kotus.fi/sanakirjat/kielitoimiston-sanakirja/nykysuomen-sana-aineistot/nykysuomen-sanalista/)
- [Finnish Parsebank's Word Frequency List](http://dl.turkunlp.org/finnish-parsebank/)
  - Frequency list derived from the Finnish Internet Parsebank corpus, covering a wide range of Finnish word forms and lemmas.
- [Frequency List of Written Finnish Word Forms](https://kaino.kotus.fi/sanat/taajuuslista/parole.php)
  - Word frequency lists compiled by Kotus from the Finnish PAROLE corpus — includes lemmas and part-of-speech information.
- [Frequencies of Early Modern Finnish Words](https://kaino.kotus.fi/sanat/taajuuslista/vns.php)
- [Frequencies of Old Literary Finnish Words](https://kaino.kotus.fi/sanat/taajuuslista/vks.php)
- [Joukahainen corpus](https://joukahainen.puimula.org/)
- [Finnish names](https://www.avoindata.fi/data/fi/dataset/none)
- [fi-words](https://github.com/akx/fi-words)
- [Sanat-wiki (CSC)](https://sanat.csc.fi/)


### Finnish speech corpora

- Parliament Plenary Speech Corpus
- Aalto Finnish Parliament ASR Corpus
- Lahjoita puhetta
- [Mozzilla Common Voice](https://commonvoice.mozilla.org/en/datasets)
- VoxPopuli Finnish
- [CSS10](https://github.com/Kyubyong/css10)
  - A Collection of Single Speaker Speech Datasets for 10 Languages
- [Fleurs](https://huggingface.co/datasets/google/fleurs)

#### Commercial speech corpora
- Finnish Speecon
- SpeechDat-Car Finnish

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
- [UralicNLP](https://github.com/mikahama/uralicNLP)
  - A Python toolkit for NLP tasks in Uralic languages, including Finnish, with support for morphological analysis, disambiguation, and lemmatization using Omorfi and Giellatekno resources.
- [Turku Neural Parser Pipeline](https://turkunlp.org/Turku-neural-parser-pipeline/)
  - A neural parsing pipeline for Finnish and other languages, providing tokenization, lemmatization, POS tagging, dependency parsing, and NER.
- [SpaCy Finnish Model](https://spacy.io/models/fi) - Finnish language model for SpaCy.
  - A statistical pipeline for Finnish NLP in SpaCy, supporting tokenization, POS tagging, dependency parsing, lemmatization, and named entity recognition.
- [Murre](https://github.com/mikahama/murre)
  - Normalize non-standard Finnish to standard Finnish.
- [FinnPos](https://github.com/mpsilfve/FinnPos)


### Universal Dependencies

- [Finnish TDT](https://universaldependencies.org/treebanks/fi_tdt/index.html) - Universal Dependencies treebank for Finnish.
  - The Finnish Turku Dependency Treebank (TDT), a manually annotated treebank following the Universal Dependencies framework.
-  [Finnish data from the FTB treebank](https://github.com/UniversalDependencies/UD_Finnish-FTB)


### Sentiment and Semantic Similarity

- [Semantic Similarity of Words](http://epsilon-it.utu.fi/wv_demo/)
  - A demo tool from University of Turku to explore cosine similarity between Finnish words using pre-trained word vector embeddings.
- [FinMeter](https://github.com/mikahama/finmeter)
  - [FinMeter models](https://zenodo.org/records/3473456)
  - [Finnish Semantic Relatedness Model](https://b2share.eudat.eu/records/5f1a5add29094d85800e5d4d2b852cdc)


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

A list of general LLMs capable of Finnish.

| Name    | Openess      | Links |
|---------|------------- |-------|
| ChatGPT | Closed       | [ChatGPT](https://chatgpt.com/) |
| Gemma 3 | Open weights | [Hugging Face](https://huggingface.co/collections/google/gemma-3-release-67c6c6f89c4f76621268bb6d), [Ollama](https://ollama.com/library/gemma3) |
| Gemini  | Closed       | [Gemini](https://gemini.google.com) |
| Poro    | Open         | [Poro collection](https://huggingface.co/collections/LumiOpen/poro-34b-66506aaedb8d705069ad7ecb) |
| Viking  | Open         | [Viking collection](https://huggingface.co/collections/LumiOpen/viking-660fa4c659d8544c00f77d9b) |
| Ahma    | Open         | [Ahma collection](https://huggingface.co/collections/Finnish-NLP/ahma-models-66ee9459e9c6e64c66f452f7)


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

- [Mika Hämäläinen](https://github.com/mikahama)


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
- [UralicNLP](https://www.uralicnlp.com/)


## Papers

A collection of interesting research papers related to Finnish NLP.

### 2025
- [An Expanded Massive Multilingual Dataset for High-Performance Language Technologies](https://arxiv.org/abs/2503.10267)

### 2021
- [Fine-grained Named Entity Annotation for Finnish](https://aclanthology.org/2021.nodalida-main.14.pdf)
- [The Current State of Finnish NLP](https://arxiv.org/abs/2109.11326)

### 2020
- [A Broad-coverage Corpus for Finnish Named Entity Recognition](http://www.lrec-conf.org/proceedings/lrec2020/pdf/2020.lrec-1.567.pdf)

### 2019
- [A Finnish News Corpus for Named Entity Recognition](https://arxiv.org/abs/1908.04212)


## Future Directions

- todo

---

This list aims to highlight the growing ecosystem of Finnish NLP tools and models. 
Maintained by [Jousia Piha](https://www.linkedin.com/in/jousia-piha/)

Contributions welcome! See [CONTRIBUTING.md](CONTRIBUTING.md) for details.

- todo

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
