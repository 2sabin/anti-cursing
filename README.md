# anti-cursing

**"anti-cursing"** is a python package that detects and switches negative or any kind of cursing word from sentences or comments whateverπ€¬

You just install the package the way you install any other package and then you can use it in your code.

The whole thing is gonna be updated soon.

So this is __**the very first idea**__

<hr>

# Concept
There are often situations where you have to code something, detect a forbidden word, and change it to another word.
Hardcoding all parts is very inconvenient, and in the Python ecosystem, there are many packages to address.
One of them is **"anti-cursing"**.

The package, which operates exclusively for **Korean**, does not simply change the banned word by setting it up, but detects and replaces the banned word by learning a deep learning model.

Therefore, it is easy to cope with new malicious words as long as they are learned.
For this purpose, semi-supervied learning through pseudo labeling is used.

Additionally, instead of changing malicious words to special characters such as --- or ***, you can convert them into emojis to make them more natural.

# Contents

- [Installation](#installation)
- [Usage](#usage)
- [Model comparison](#model-comparison)
- [Dataset](#dataset)
- [Used API](#used-api)
- [License](#license)
- [Working Example](#working-example)
- [References](#references)
- [Project Status](#project-status)
- [Future Work](#future-work)


# Installation

You can install the package using pip:

```bash
pip install anti-cursing
```

**it doesn't work yet, but it will soon!!π¨π»βπ»**

# Usage

```python
from anti_cursing import anti_cursing

anti_cursing("λλ λκ° μ’μ§λ§, λλ λλ¬΄ κ°μλΌμΌ")
```

```bash
λλ λκ° μ’μ§λ§, λλ λλ¬΄ πΌπ»μΌ
```

# Model-comparison

| Classification | KcElectra | KoBERT | RoBERTa-large | etc(maybe further more) |
| --- | --- | --- | --- | --- |
| Validation Accuracy | | | | |
| Validation Loss | | | | |
| Training Loss | | | | |
| Epoch | | | | |
| Batch-size | | | | |
| transformers | | | | |

# Dataset
* ### Smilegate-AI 
  * https://github.com/smilegate-ai/korean_unsmile_dataset
  * Korean Sentiment Analysis
  * [paper](#korean-unsmile-dataset)
* ### Naver portal news articles crawling
  * https://news.naver.com
  * Non-labeled Data for Test Dataset
* ### π Emoji unicode crawling for encoding
  * https://unicode.org/emoji/charts/full-emoji-list.html

# Used-api
### Google translator
* https://cloud.google.com/translate/docs (API DOCS)

# License

This repository is licensed under the MIT license. See LICENSE for details.

Click here to see the License information --> [License](LICENSE)

# Working-example
---- some video is gonna be placed here ----

# References

### Sentiment Analysis Based on Deep Learning : A Comparative Study
  * Nhan Cach Dang, Maria N. Moreno-Garcia, Fernando De la Prieta. 2006. Sentiment Analysis Based on Deep Learning : A Comparative Study. In Proceedings of the 2006 Conference on Empirical Methods in Natural Language Processing (EMNLP 2006), pages 1β8, Prague, Czech Republic. Association for Computational Linguistics.
### Attention is all you need
  * Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N Gomez, Lukasz Kaiser, and Illia Polosukhin. 2017. Attention is all you need. In Advances in Neural Information Processing Systems, pages 6000β6010.
### BERT : Pre-training of Deep Bidirectional Transformers for Language Understanding
  * Jacob Devlin, Ming-Wei Chang, Kenton Lee, and Kristina Toutanova. 2018. BERT:         Pre-training of deep bidirectional transformers for language understanding. In Proceedings of the 2018 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 1 (Long Papers), pages 4171β4186.

### Electra : Pre-training Text Encoders as Discriminators Rather Than Generators
  * Kevin Clark, Minh-Thang Luong, Quoc V. Le, Christopher D. Manning. 2019. Electra: Pre-training text encoders as discriminators rather than generators. In Proceedings of the 2019 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 1 (Long Papers), pages 4171β4186.

### BIDAF : Bidirectional Attention Flow for Machine Comprehension
  * Minjoon Seo, Aniruddha Kembhavi, Ali Farhadi, Hannaneh Hajishirzi. 2016. Bidirectional Attention Flow for Machine Comprehension. In Proceedings of the 2016 Conference on Empirical Methods in Natural Language Processing, pages 2129β2139.

### Effect of Negation in Sentences on Sentiment Analysis and Polarity Detection
  * Partha Mukherjeea, Saptarshi Ghoshb, and Saptarshi Ghoshc. 2018. Effect of Negation in Sentences on Sentiment Analysis and Polarity Detection. In Proceedings of the 2018 Conference on Empirical Methods in Natural Language Processing, pages 2129β2139.

### KOAS : Korean Text Offensiveness Analysis System
  * Seonghwan Kim, Seongwon Lee, and Seungwon Do. 2019. KOAS: Korean Text Offensiveness Analysis System. In Proceedings of the 2019 Conference on Empirical Methods in Natural Language Processing and the 9th International Joint Conference on Natural Language Processing (EMNLP-IJCNLP), pages 1β11.

### Korean Unsmile Dataset
  * Seonghwan Kim, Seongwon Lee, and Seungwon Do. 2019. Korean Unsmile Dataset. In Proceedings of the 2019 Conference on Empirical Methods in Natural Language Processing and the 9th International Joint Conference on Natural Language Processing (EMNLP-IJCNLP), pages 1β11.
# Project-status

![10%](https://geps.dev/progress/10)

# Future-work
update soon plz bare with me ππ»

<hr>

# KOREAN FROM HERE / μ¬κΈ°λΆν΄ νκ΅­μ΄ μ€λͺμλλ€.
# anti-cursing

**"anti-cursing"**μ λ¬Έμ₯μ΄λ λκΈμμ λΆμ μ μ΄κ±°λ λͺ¨λ  μ’λ₯μ μμ€μ κ°μ§νκ³  μ ννλ νμ΄μ¬ ν¨ν€μ§μλλ€π€¬

λ€λ₯Έ ν¨ν€μ§λ₯Ό μ€μΉνλ λ°©μκ³Ό λμΌνκ² ν¨ν€μ§λ₯Ό μ€μΉν λ€μ μ½λμμ μ¬μ©ν  μ μμ΅λλ€.

μμ§ μμ΄λμ΄ κ΅¬μ λ¨κ³μ΄κΈ° λλ¬Έμ **μλ¬΄κ²λ μλνμ§ μμ§λ§** κ³§ μλνλλ‘ μλ°μ΄νΈν  μμ μλλ€.

<hr>

# Concept

λ¬΄μΈκ° μ½λ©μ νλ©°, κΈμ§ λ¨μ΄λ₯Ό κ°μ§νκ³  κ·Έκ²μ λ€λ₯Έ λ¨μ΄λ‘ λ°κΏμΌν  μν©μ΄ μ’μ’ μκΉλλ€.
λͺ¨λ  λΆλΆμ νλμ½λ©νλ κ²μ΄ λ§€μ° λΆνΈνλ©°, νμ΄μ¬ μνκ³μμλ μ΄λ₯Ό ν΄κ²°νκΈ° μν λ§μ ν¨ν€μ§κ° μμ΅λλ€.
κ·Έ μ€ νλκ° **"anti-cursing"**μλλ€.

νκ΅­μ΄ μ μ©μΌλ‘ λμνλ ν΄λΉ ν¨ν€μ§λ λ¨μν κΈμ§ λ¨μ΄λ₯Ό κΈ°μ‘΄μ μ€μ νμ¬ λ°κΎΈλ κ²μ΄ μλ, λ₯λ¬λ λͺ¨λΈμ νμ΅νμ¬ κΈμ§ λ¨μ΄λ₯Ό κ°μ§νκ³  λ°κΏλλ€.
λ°λΌμ μλ‘­κ² μκΈ°λ μμ± λ¨μ΄μ λν΄μλ νμ΅λ§ μ΄λ£¨μ΄μ§λ€λ©΄ μ½κ² λμ²ν  μ μμ΅λλ€.
μ΄λ₯Ό μν΄ pseudo labelingμ ν΅ν semi-supervied learningμ μ¬μ©ν©λλ€. 

μΆκ°λ‘ μμ±λ¨μ΄λ₯Ό ---λ ***κ°μ νΉμλ¬Έμλ‘ λ³κ²½νλ κ²μ΄ μλ, μ΄λͺ¨μ§λ‘ λ³ννμ¬ λμ± μμ°μ€λ½κ² λ°κΏ μ μμ΅λλ€.
# λͺ©μ°¨

- [μ€μΉ](#μ€μΉ)
- [μ¬μ©λ²](#μ¬μ©λ²)
- [λͺ¨λΈ μ±λ₯ λΉκ΅](#λͺ¨λΈ-μ±λ₯-λΉκ΅)
- [λ°μ΄ν°μ](#λ°μ΄ν°μ)
- [μ¬μ© API](#μ¬μ©-api)
- [License](#license)
- [μλ μμ](#μλ-μμ)
- [μ°Έκ³ λ¬Έν](#μ°Έκ³ λ¬Έν)
- [μ§νμν©](#μ§νμν©)
- [λ°μ ](#λ°μ )


# μ€μΉ

pipλ₯Ό μ¬μ©νμ¬ ν¨ν€μ§λ₯Ό μ€μΉν  μ μμ΅λλ€.
```bash
pip install anti-cursing
```

**μμ§ μλ¬΄κ²λ μλνμ§ μμ§λ§, κ³§ μλνλλ‘ μλ°μ΄νΈν  μμ μλλ€π¨π»βπ».**

# μ¬μ©λ²

```python
from anti_cursing import anti_cursing

anti_cursing("λλ λκ° μ’μ§λ§, λλ λλ¬΄ κ°μλΌμΌ")
```

```bash
λλ λκ° μ’μ§λ§, λλ λλ¬΄ πΌπ»μΌ
```

# λͺ¨λΈ μ±λ₯ λΉκ΅

| Classification | KcElectra | KoBERT | RoBERTa-large | κΈ°ν(μΆκ°μμ ) |
| --- | --- | --- | --- | --- |
| Validation Accuracy | | | | |
| Validation Loss | | | | |
| Training Loss | | | | |
| Epoch | | | | |
| Batch-size | | | | |
| transformers | | | | |

# λ°μ΄ν°μ
* ### Smilegate-AI 
  * https://github.com/smilegate-ai/korean_unsmile_dataset
  * νκ΅­μ΄ κ°μ λΆλ₯ λ°μ΄ν°μ
  * [paper](#korean-unsmile-dataset)
* ### λ€μ΄λ² λ΄μ€ κΈ°μ¬ ν¬λ‘€λ§
  * https://news.naver.com
  * νμ€νΈλ₯Ό μν λ°μ΄ν°μ
* ### π μ΄λͺ¨μ§ μ λμ½λ λ°μ΄ν°μ
  * https://unicode.org/emoji/charts/full-emoji-list.html

# μ¬μ© API
### Google translator
* https://cloud.google.com/translate/docs (API λ¬Έμ)

# License

μ΄ νλ‘μ νΈλ MIT λΌμ΄μΌμ€λ₯Ό λ°λ¦λλ€. μμΈν λ΄μ©μ LICENSE νμΌμ μ°Έκ³ ν΄μ£ΌμΈμ.

λΌμ΄μΌμ€ μ λ³΄ --> [License](LICENSE)

# μλ μμ
---- μλ μμκ° μΆκ°λ  μμ μλλ€ ----

# μ°Έκ³ λ¬Έν

### Sentiment Analysis Based on Deep Learning : A Comparative Study
  * Nhan Cach Dang, Maria N. Moreno-Garcia, Fernando De la Prieta. 2006. Sentiment Analysis Based on Deep Learning : A Comparative Study. In Proceedings of the 2006 Conference on Empirical Methods in Natural Language Processing (EMNLP 2006), pages 1β8, Prague, Czech Republic. Association for Computational Linguistics.
### Attention is all you need
  * Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N Gomez, Lukasz Kaiser, and Illia Polosukhin. 2017. Attention is all you need. In Advances in Neural Information Processing Systems, pages 6000β6010.
### BERT : Pre-training of Deep Bidirectional Transformers for Language Understanding
  * Jacob Devlin, Ming-Wei Chang, Kenton Lee, and Kristina Toutanova. 2018. BERT:         Pre-training of deep bidirectional transformers for language understanding. In Proceedings of the 2018 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 1 (Long Papers), pages 4171β4186.

### Electra : Pre-training Text Encoders as Discriminators Rather Than Generators
  * Kevin Clark, Minh-Thang Luong, Quoc V. Le, Christopher D. Manning. 2019. Electra: Pre-training text encoders as discriminators rather than generators. In Proceedings of the 2019 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies, Volume 1 (Long Papers), pages 4171β4186.

### BIDAF : Bidirectional Attention Flow for Machine Comprehension
  * Minjoon Seo, Aniruddha Kembhavi, Ali Farhadi, Hannaneh Hajishirzi. 2016. Bidirectional Attention Flow for Machine Comprehension. In Proceedings of the 2016 Conference on Empirical Methods in Natural Language Processing, pages 2129β2139.

### Effect of Negation in Sentences on Sentiment Analysis and Polarity Detection
  * Partha Mukherjeea, Saptarshi Ghoshb, and Saptarshi Ghoshc. 2018. Effect of Negation in Sentences on Sentiment Analysis and Polarity Detection. In Proceedings of the 2018 Conference on Empirical Methods in Natural Language Processing, pages 2129β2139.

### KOAS : Korean Text Offensiveness Analysis System
  * Seonghwan Kim, Seongwon Lee, and Seungwon Do. 2019. KOAS: Korean Text Offensiveness Analysis System. In Proceedings of the 2019 Conference on Empirical Methods in Natural Language Processing and the 9th International Joint Conference on Natural Language Processing (EMNLP-IJCNLP), pages 1β11.

### Korean Unsmile Dataset
  * Seonghwan Kim, Seongwon Lee, and Seungwon Do. 2019. Korean Unsmile Dataset. In Proceedings of the 2019 Conference on Empirical Methods in Natural Language Processing and the 9th International Joint Conference on Natural Language Processing (EMNLP-IJCNLP), pages 1β11.
# μ§νμν©

![10%](https://geps.dev/progress/10)

# λ°μ 
μμΌλ‘ μΆκ°λ  μμ μλλ€ μ μλ§ κΈ°λ€λ €μ£ΌμΈμππ»
