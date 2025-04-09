### 📊 Finnish UD Treebanks Comparison

| Feature                          | **UD_Finnish-TDT**                                | **UD_Finnish-FTB**                                 |
|----------------------------------|----------------------------------------------------|-----------------------------------------------------|
| **Full Name**                   | Turku Dependency Treebank                         | FinnTreeBank 1                                      |
| **Source Type**                | Real-world texts (news, blogs, fiction, etc.)     | Grammatical examples from VISK grammar             |
| **Purpose**                    | Broad language coverage, parsing, NLP tasks        | Illustrating grammatical constructions              |
| **Annotation Origin**         | Fully manually annotated, Stanford → UD conversion | Auto-converted from native format, partially revised |
| **Genre Coverage**            | Diverse, multi-genre                               | Narrow, grammar-focused                            |
| **Annotation Quality**        | High, consistent with UD standards                | Variable, with fallback `dep` relations used       |
| **Tokenization & Punctuation** | Consistent UD-style token & punctuation handling   | Some inconsistencies; punctuation often misattached |
| **Multiword Tokens**          | Carefully handled and annotated                    | Sometimes inconsistently handled                              |
| **Relation Labels**           | Full UD relation set, manual revisions             | Some mappings incomplete, frequent `dep` usage     |
| **Usage Suitability**         | Parser training, real-world NLP                    | Grammar study, illustrative purposes               |
| **Sentence Count**            | ~15,000 (train/dev/test)                          | ~18,000 (train/dev/test)                           |
| **Maintainers**               | TurkuNLP (University of Turku)                     | FIN-CLARIN, University of Helsinki                 |
| **License**                   | CC BY-SA 4.0                                       | CC BY 4.0                                           |

---
