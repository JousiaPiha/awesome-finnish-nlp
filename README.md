# Awesome Finnish NLP [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of awesome resources for Natural Language Processing in Finnish. This repository gathers tools, models, datasets, papers, and organizations working on Finnish NLP. Contributions are welcome!

## Contents

- [LLMs for Finnish](#llms-for-finnish)
- [Spacy & Finnish Pipeline](#spacy--finnish-pipeline)
- [Hugging Face Organizations and Users](#hugging-face-organizations-and-users)
- [Morphology & Parsers](#morphology--parsers)
- [Universal Dependencies](#universal-dependencies)
- [Organizations](#organizations)
- [Sentiment Analysis](#sentiment-analysis)
- [Named Entity Recognition](#named-entity-recognition)
- [Semantic Similarity](#semantic-similarity)
- [Word Lists](#word-lists)
- [Pre-trained Models](#pre-trained-models)
  - [General Language Models](#general-language-models)
  - [Sentiment Analysis](#sentiment-analysis)
  - [Named Entity Recognition (NER)](#named-entity-recognition-ner)
- [Datasets and Corpora](#datasets-and-corpora)
- [Speech technologies](#speech-technologies)
  - [Text-to-Speech (TTS)](#text-to-speech-tts)
  - [Speech-to-Text (STT)](#speech-to-text-stt)
- [Machine translation](#machine-translation)
- [Papers](#papers)
- [Future Directions](#future-directions)
- [Contributing](#contributing)
- [License](#license)

## LLMs for Finnish

| Name    | Open-source | Available locally | Links |
|---------|-------------|-------------------|-------|
| ChatGPT | No          | No                | [ChatGPT](https://chatgpt.com/) |
| Gemma 3 | Yes         | Yes               | [Hugging Face](https://huggingface.co/collections/google/gemma-3-release-67c6c6f89c4f76621268bb6d), [Ollama](https://ollama.com/library/gemma3) |
| Gemini  | No          | No                | [Gemini](https://gemini.google.com) |
| Poro    | Yes         | Yes               | [Poro](https://huggingface.co/collections/LumiOpen/poro-34b-66506aaedb8d705069ad7ecb) |
| Viking  | Yes         | Yes               | [Viking](https://huggingface.co/collections/LumiOpen/viking-660fa4c659d8544c00f77d9b) |

## Spacy & Finnish Pipeline

- [SpaCy Finnish Model](https://spacy.io/models/fi) - Finnish language model for SpaCy.
  - A statistical pipeline for Finnish NLP in SpaCy, supporting tokenization, POS tagging, dependency parsing, lemmatization, and named entity recognition.

## Hugging Face Organizations and Users

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

## Morphology & Parsers

- [Omorfi](https://flammie.github.io/omorfi/)
  - Omorfi is a free and open source project containing various tools and data for natural language processing of Finnish based on a knowledge driven paradigm.
- [UralicNLP](https://www.uralicnlp.com/)
  - A Python toolkit for NLP tasks in Uralic languages, including Finnish, with support for morphological analysis, disambiguation, and lemmatization using Omorfi and Giellatekno resources.
- [Turku Neural Parser Pipeline](https://turkunlp.org/Turku-neural-parser-pipeline/)
  - A neural parsing pipeline for Finnish and other languages, providing tokenization, lemmatization, POS tagging, dependency parsing, and NER.

## Universal Dependencies

- [Finnish TDT](https://universaldependencies.org/treebanks/fi_tdt/index.html) - Universal Dependencies treebank for Finnish.
  - The Finnish Turku Dependency Treebank (TDT), a manually annotated treebank following the Universal Dependencies framework.

## Organizations

- [Kotus](https://kotus.fi/)
  - The Institute for the Languages of Finland — maintains official Finnish corpora, word lists, grammar guidelines, and other language resources.
- [Kielipankki](https://www.kielipankki.fi/)
  - The Language Bank of Finland — a national infrastructure providing access to Finnish and multilingual corpora for research.
- [TurkuNLP](https://turkunlp.org/)
  - Research group producing high-quality Finnish NLP tools, corpora, and pre-trained models.
- [HPLT Project](https://hplt-project.org/)
  - High-Performance Language Technologies project — aims to build open LLMs in European languages, including Finnish, using supercomputing resources.

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

## Semantic Similarity

- [Semantic Similarity of Words](http://epsilon-it.utu.fi/wv_demo/)
  - A demo tool from University of Turku to explore cosine similarity between Finnish words using pre-trained word vector embeddings.

## Word Lists

- [Finnish Parsebank's Word Frequency List](http://dl.turkunlp.org/finnish-parsebank/)
  - Frequency list derived from the Finnish Internet Parsebank corpus, covering a wide range of Finnish word forms and lemmas.
- [Parole Corpus Frequency Lists](https://kaino.kotus.fi/sanat/taajuuslista/parole.php)
  - Word frequency lists compiled by Kotus from the Finnish PAROLE corpus — includes lemmas and part-of-speech information.

## Datasets and Corpora

- [Kotus Aineistot Verkossa](https://kotus.fi/kotus/kieliaineistot/aineistot-verkossa/)
  - A collection of publicly available corpora and lexical resources from the Institute for the Languages of Finland (Kotus), including news, spoken language, dialects, and more.

## Speech Technologies

### Text-to-Speech (TTS)
- [Piper](https://github.com/rhasspy/piper)
  - A fast, lightweight neural TTS engine with Finnish voice support, designed for offline use on CPUs and embedded devices.

### Speech-to-Text (STT)

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

- [Fairseq](https://github.com/facebookresearch/fairseq)  
  Meta's sequence modeling toolkit used in training multilingual MT models like NLLB. Also used in many research projects involving Finnish.

- [ELG – European Language Grid](https://live.european-language-grid.eu/catalogue/search?language=fi&modality=machine-translation)  
  Aggregates various Finnish-compatible machine translation systems. Includes both open and commercial services developed across Europe.

---

### Pipelines and Frameworks

- [OpenNMT](https://opennmt.net/)  
  A general-purpose neural machine translation framework. Finnish support depends on available training data (can be combined with OPUS datasets).

- [MarianNMT](https://marian-nmt.github.io/)  
  High-performance NMT framework used to train many Opus-MT models. Supports custom training for Finnish models using OPUS corpora.

---

### Commercial Machine Translation APIs

These are proprietary services that support Finnish, often used in production environments:

- [Google Cloud Translation](https://cloud.google.com/translate)  
  Fast, production-ready neural MT API with Finnish support. Offers both standard and custom model options via AutoML.

- [DeepL Translator](https://www.deepl.com/translator)  
  Widely praised for translation quality. Supports Finnish with a polished web UI, desktop apps, and a commercial API.

- [Microsoft Translator (Azure)](https://www.microsoft.com/en-us/translator/)  
  Neural MT service by Microsoft. Finnish is supported and integrated into many Microsoft products and services.

- [Amazon Translate](https://aws.amazon.com/translate/)  
  Neural MT as a managed service on AWS. Finnish is included in the supported languages.

- [Lingsoft MT Services](https://www.lingsoft.fi/en/solutions/language-services/translation)  
  Commercial MT solutions developed in Finland. Often used in Finnish government and healthcare sectors. Some services may be available via ELG.




## Papers

- [A Broad-coverage Corpus for Finnish Named Entity Recognition](http://www.lrec-conf.org/proceedings/lrec2020/pdf/2020.lrec-1.567.pdf)
- [An Expanded Massive Multilingual Dataset for High-Performance Language Technologies](https://arxiv.org/abs/2503.10267)

## Future Directions

- todo

## Contributing

Contributions are welcome! Please see the [CONTRIBUTING](CONTRIBUTING.md) file for guidelines.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
