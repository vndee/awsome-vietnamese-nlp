# Vietnamese Natural Language Processing Resources

- [Corpus](#Corpus)
- [Text Processing Toolkit](#Text-Processing-Toolkit)
- [Pre-trained Language Model](#Pre-trained-Language-Model)
- [Sentiment Analysis](#Sentiment-Analysis)

### Corpus
- [VN News Corpus](https://github.com/binhvq/news-corpus): 50GB of uncompressed texts crawled from a wide range ofnews websites and topics.
- [VNESEcorpus](http://viet.jnlp.org/download-du-lieu-tu-vung-corpus): 650.000 sentences from vietnamnet.vn, dantri.com.vn, nhandan.com.vn.
- [VNTQcorpus(samll)](http://viet.jnlp.org/download-du-lieu-tu-vung-corpus): 300.000 sentences from vnthuquan.net.
- [VNTQcorpus(big)](http://viet.jnlp.org/download-du-lieu-tu-vung-corpus): 1.750.000 sentences from vnthuquan.net.
- [WikiDumps](https://dumps.wikimedia.org/): You can download directly or use scripts from [viwik18](https://github.com/NTT123/viwik18), [viwik19](https://github.com/NTT123/viwik19).
- [Vietnamese Treebank](https://vlsp.hpda.vn/demo/?page=resources): VLSP Project.
- [Vietnamese Stopwords](https://github.com/stopwords/vietnamese-stopwords):  Vietnamese stopwords.
- [Vietnamese Dictionary](https://www.informatik.uni-leipzig.de/~duc/Dict/): Vietnamese dictionary.
- [vietnamese-wordnet](https://github.com/zeloru/vietnamese-wordnet): Vietnamese wordnet.

### Text Processing Toolkit
- [coccoc-tokenizer](https://github.com/coccoc/coccoc-tokenizer): High performance tokenizer for Vietnamese language. It is written in C++ with Python and Java bindings.
- [RDRSegmenter](https://github.com/datquocnguyen/RDRsegmenter):  Fast and accurate Vietnamese word segmenter (LREC 2018).
- [RDRPOSTagger](https://github.com/datquocnguyen/RDRPOSTagger): Fast and accurate POS and morphological tagging toolkit (EACL 2014).
- [VnCoreNLP](https://github.com/vncorenlp/VnCoreNLP):  A Vietnamese natural language processing toolkit (NAACL 2018).
- [vlp-tok](https://github.com/phuonglh/vlp): Vietnamese text processing library developed in the Scala programming language.
- [nnvlp](https://github.com/pth1993/NNVLP): Neural network-based Vietnamese language processing toolkit.
- [jPTDP](https://github.com/datquocnguyen/jPTDP):  Neural network models for joint POS tagging and dependency parsing (CoNLL 2017-2018).
- [vi_spacy](https://github.com/trungtv/vi_spacy): vietnamese language model compatible with Spacy.
- [underthesea](https://underthesea.readthedocs.io/en/latest/readme.html): Underthesea - Vietnamese NLP toolkit.
- [vnlp](https://bitbucket.org/epilab/vnlp/wiki/Home): GATE plugin for Vietnamese language processing.
- [pyvi](https://github.com/trungtv/pyvi): Python Vietnamese toolkit.
- [JVnTextPro](http://jvntextpro.sourceforge.net/): Java-based Vietnamese text processing tool.
- [DongDu](https://github.com/rockkhuya/DongDu): C++ implementation of Vietnamese word segmentation tool.
- [VLSP Toolkit](https://vlsp.hpda.vn/demo/?page=resources): Vietnamese tokenizer from VLSP.
- [vTools](https://github.com/lupanh/vTools): Vietnamese NLP toolkit: Tokenizer, Sentence detector, POS tagger, Phrase chunker.
- [JNSP](http://jnsp.sourceforge.net/): Java Implementation of Ngram Statistic Package.

### Pre-trained Language Model
- [RoBERTa Vietnamese](https://github.com/nguyenvulebinh/vietnamese-roberta): Pre-trained embedding using RoBERTa architecture on Vietnamese corpus.
- [PhoBERT](https://github.com/VinAIResearch/PhoBERT): Pre-trained language models for Vietnamese (another implementation of RoBERTa for Vietnamese).
- [ALBERT for Vietnamese](https://github.com/ngoanpv/albert_vi): "A Lite" version of BERT for Vietnamese.
- [Vietnamese ELECTRA](https://github.com/nguyenvulebinh/vietnamese-electra):  Electra pre-trained model using Vietnamese corpus.

### Sentiment Analysis
#### Benchmark
- **[VLSP 2016 Share Task: Sentiment Analysis](https://vlsp.org.vn/vlsp2016/eval/sa)**.
    - Train: 5100 sentences (1700 positive, 1700 neutral, 1700 negative).
    - Test: 1050 sentences (350 positive, 350 neutral, 350 negative).

        | Model                 | F1 | Paper | Code |
        |-----------------------|----|-------|------|
        | Perceptron/SVM/Maxent |  80.05  |   DSKTLAB: Vietnamese Sentiment Analysis for Product Reviews  |      |
        | SVM/MLNN/LSTM | 71.44   | A Simple Supervised Learning Approach to Sentiment Classification at VLSP 2016 |      |
        | Ensemble: Random forest, SVM, Naive Bayes | 71.22 | A Lightweight Ensemble Method for Sentiment Classification Task | |
        | Ensemble: SVM, LR, LSTM, CNN | 69.71 | An Ensemble of Shallow and Deep Learning Algorithms for Vietnamese Sentiment Analysis | |
        | SVM | 67.54 | Sentiment Analysis for Vietnamese using Support Vector Machines with application to Facebook comments | |
        | SVM/MLNN | 67.23 | A Multi-layer Neural Network-based System for Vietnamese Sentiment Analysis at the VLSP 2016 Evaluation Campaign | |
        | Multi-channel LSTM-CNN | 59.61 | Multi-channel LSTM-CNN model for Vietnamese sentiment analysis | [official](https://github.com/ntienhuy/MultiChannel) |

- **[VLSP 2018 Shared Task: Aspect Based Sentiment Analysis](https://vlsp.org.vn/vlsp2018)**.
    - **Restaurant Dataset**: 2961 reviews (train), 1290 reviews (development), 500 reviews (test).
    
        | Model| Aspect (F1) | Aspect Polarity (F1) | Paper | Code |
        |---|---|---|---|---|
        | CNN | 0.80 | | Deep Learning for Aspect Detection on Vietnamese Reviews | |
        | SVM | 0.77 | 0.61 | NLP@UIT at VLSP 2018: A Supervised Method For Aspect Based Sentiment Analysis | |
        | SVM | 0.54 | 0.48 | Using Multilayer Perceptron for Aspect-based Sentiment Analysis at VLSP 2018 SA Task | |
    
    - **Hotel Dataset**: 3000 reviews (training), 2000 reviews (development), 600 reviews (test).
        
        | Model| Aspect (F1) | Aspect Polarity (F1) | Paper | Code |
        |---|---|---|---|---|
        | SVM | 0.70 | 0.61 | NLP@UIT at VLSP 2018: A Supervised Method For Aspect Based Sentiment Analysis | |
        | CNN | 0.69 | | Deep Learning for Aspect Detection on Vietnamese Reviews | |
        | SVM | 0.56 | 0.53 | Using Multilayer Perceptron for Aspect-based Sentiment Analysis at VLSP 2018 SA Task | |

- **[Vietnamese Student's Feedback Corpus (UIT-VSFC)](https://ieeexplore.ieee.org/document/8573337)**.
    - UIT-VSFC consists of over 16,000 sentences for sentiment analysis and topic classification.
    
        | Model | Sentiment (F1) | Topic (F1) | Paper | Code |
        |-------|----------------|------------|-------|------|
        | Bi-LSTM/Word2Vec | 0.896 | 0.92 | Deep Learning versus Traditional Classifiers on Vietnamese Student’s Feedback Corpus | |
        | Maximum Entropy Classifier | 0.88 | 0.84 | UIT-VSFC: Vietnamese Student’s Feedback Corpus for Sentiment Analysis | |

- Papers:
    - Dang-Khoa Nguyen-Nhat, Huu-Thanh Duong. One-Document Training for Vietnamese Sentiment Analysis. CSoNet 2019: Computational Data and Social Networks pp 189-200, 2019.
    - Phu, V.N., Chau, V.T.N., Tran, V.T.N. et al. A Valence-Totaling Model for Vietnamese sentiment classification. Evolving Systems 10, 453–499 (2019).
    - Tran, Thien Khai., Phan, Tuoi Thi. A hybrid approach for building a Vietnamese sentiment dictionary. Journal of Intelligent & Fuzzy Systemvol, 35, no. 1, pp. 967-978, 2018.
    - T. A. Nguyen and P. Q. N. Minh, "Using multilayer perceptron for aspect-based sentiment analysis at vlsp-2018 sa task," in In Proceedings of the Fifth International workshop on Vietnamese Language and Speech Processing (VLSP 2018), 2018.
    - T. D. Van, K. V. Nguyen, and N. L.-T. Nguyen., "Nlp@uit at vlsp 2018: A supervised method for aspect based sentiment analysis," in In Proceedings of the Fifth International workshop on Vietnamese Language and Speech Processing (VLSP 2018), 2018.
    - N. V. Vi, H. V. Minh, and N. T. Tam, "Sentiment analysis for vietnamese using support vector machines with application to facebook," in in The Fourth International Workshop on Vietnamese Language and Speech Processing (VLSP 2016), 2016.
    - N. Hy, L. Tung, L. Viet-Thang, and D. Dien, "A simple supervised learning approach to sentiment classication at vlsp 2016," in in The Fourth International Workshop on Vietnamese Language and Speech Processing (VLSP 2016), 2016. 
    - P. M. Q. Nhat and T. T. Tran, "A lightweight ensemble method for sentiment classication task," in in The Fourth International Workshop on Vietnamese Language and Speech Processing (VLSP 2016), 2016.
    - T. T. Tran, X. Ho, and N. T. Nguyen, "A multi-layer neural network based system for vietnamese sentiment analysis at the vlsp 2016 evaluation campaign," in in The Fourth International Workshop on Vietnamese Language and Speech Processing (VLSP 2016), 2016.
    - T. P. Quynh-Trang, N. Xuan-Truong, T. Van-Hien, N. Thi-Cham, and T. Mai-Vu, "Dsktlab: Vietnamese sentiment analysis for product reviews," in The Fourth International Workshop on Vietnamese Language and Speech Processing (VLSP 2016), 2016.
    - Kieu, Binh & Pham, Son. Sentiment Analysis for Vietnamese. 152 - 157. 10.1109/KSE.2010.33, (2010).

### Text-To-Speech
#### Dataset:
- [VietTTS-v1](https://github.com/NTT123/Vietnamese-Text-To-Speech-Dataset): A synthesized dataset for Vietnamese TTS task (35.1 hrs).
