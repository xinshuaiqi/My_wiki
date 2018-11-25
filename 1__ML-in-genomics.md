<<<<<<< HEAD
# Machine Learning in genomics

[TOC]





## [Wiki： Machine learning in bioinformatics](https://en.wikipedia.org/wiki/Machine_learning_in_bioinformatics)



# Entry level knowledge:



### Basic

##### [[莫烦python](https://morvanzhou.github.io/) (python 入门+ Machine Learning)

##### [TensorFlow 官方文档中文版](http://docs.pythontab.com/tensorflow/)

##### Keras Documentation](https://keras.io/) and [中文文档](https://keras-cn.readthedocs.io/en/latest/)





### People in ML

##### Geoff Hinton, google, godfather of Deep learning

University of Toronto Computer Science

https://en.wikipedia.org/wiki/Geoffrey_Hinton



##### Yann LeCun, facebook, father of CNN

http://yann.lecun.com/

https://en.wikipedia.org/wiki/Yann_LeCun



##### Yoshua Bengio

Canaca; ANN; DL;

##### Yair Weiss



# Advanced knowledge

### Useful resources:

##### A list of deep learning implementations in **biology**: [link](https://github.com/hussius/deeplearning-biology)

##### A curated list of awesome deep learning applications in the field of **computational biology** [link](https://github.com/gokceneraslan/awesome-deepbio)

##### **[Practical Deep Learning For Coders**](http://course.fast.ai/)

##### [Udemy: Deep Learning A-Z™: Hands-On Artificial Neural Networks $$](https://www.udemy.com/deeplearning/)



### YouTube

[Deep learning for genomics - Anshul Kundaje](https://youtu.be/X5mdoxR9qag)

[James Zou: "Deep learning for genomics: Introduction and examples"](
https://youtu.be/JYt1IqdDAPc)



##### [James Zhou Teaching](https://sites.google.com/site/jamesyzou/teaching)

**CS 329M Algorithms of advanced machine learning.**  **(website)**https://canvas.stanford.edu/courses/51037

**CS 273B Deep learning in genomics and bio-medicine.** **(website)** https://canvas.stanford.edu/courses/66218/

see my github for the downloaed course material



##### [Anshul Kundaje Teaching](https://sites.google.com/site/anshulkundaje/teaching)

Tutorials: https://sites.google.com/site/anshulkundaje/inotes





### Chinese in ML

##### Yifei Chen

https://scholar.google.com/citations?user=ygovHrsAAAAJ&hl=en

Department of Computer Science, University of California, Irvine, CA 92697, USA

##### [JIAN ZHOU](http://www.princeton.edu/~jzthree/)

http://www.princeton.edu/~jzthree/

##### James Zhou

https://sites.google.com/site/jamesyzou/home




### Papers:

##### [Evolutionarily informed deep learning methods: Predicting transcript abundance from DNA sequence](https://www.biorxiv.org/content/early/2018/07/19/372367)



##### [Deep Learning for Genomics: A Concise Overview](https://arxiv.org/abs/1802.00810)



##### [Deep learning for biology](https://www.nature.com/articles/d41586-018-02174-z)



##### [Deep Learning for Population Genetic Inference](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004845)

```
 * jointly inferring natural selection and demography
 
 * We find many regions of the genome that have experienced hard sweeps, and fewer under selection on standing variation (soft sweep) or balancing selection.
 
```

##### [Deep learning for computational biology](http://msb.embopress.org/content/12/7/878.abstract)

[C Angermueller](https://scholar.google.com/citations?user=OXZC0mQAAAAJ&hl=en&oi=sra), T Pärnamaa, [L Parts](https://scholar.google.com/citations?user=ktEf4ZUAAAAJ&hl=en&oi=sra)… - Molecular systems …, 2016 - msb.embopress.org

```markdown
# the most accurate prediction of gene expression levels is currently made from a broad set of epigenetic features using sparse linear models (Karlic et al, 2010; Cheng et al, 2011) or random forests (Li et al, 2015)

Most of these applications can be described within the canonical machine learning workflow, which involves four steps: 
* data cleaning and pre‐processing, 
* feature extraction, 
* model fitting and 
* evaluation 

A major recent advance in machine learning is automating this critical step by learning a suitable representation of the data with deep artificial neural networks

Briefly, a deep neural network takes the raw data at the lowest (input) layer and transforms them into increasingly abstract feature representations by successively combining outputs from the preceding layer in a data‐driven manner, encapsulating highly complicated functions in the process

depth of the layer X the width of the layer

backward propagation algorithm ultimately enabling efficient training of neural networks using stochastic gradient descent


其他的DNN变形
convolutional neural networks, which are widely used for **modelling images**
recurrent neural networks for **sequential data**
restricted Boltzmann machines and autoencoders for **unsupervised learning**

comprehensive background on all technical details, which can be found in the more specialized literature (Bengio, 2012; Bengio et al, 2013; Deng, 2014; Schmidhuber, 2015; Goodfellow et al, 2016). 
```



##### [*Machine learning** applications in **genetics** and **genomics**](https://www.nature.com/articles/nrg3920)

[MW Libbrecht](https://scholar.google.com/citations?user=O4SMk-sAAAAJ&hl=en&oi=sra), [WS Noble](https://scholar.google.com/citations?user=plt2_DsAAAAJ&hl=en&oi=sra) - Nature Reviews **Genetics**, 2015 - nature.com



##### [Machine Learning in Genomics – Current Efforts and Future Applications](https://www.techemergence.com/machine-learning-in-genomics-applications/)



##### [Deep learning meets genome biology](https://www.oreilly.com/ideas/deep-learning-meets-genome-biology)

An interview with Brendan Frey about realizing new possibilities in genomic medicine.



##### [TRAINING AND APPLYING GENOMIC DEEP LEARNING MODELS](https://blog.dnanexus.com/2018-05-31-training-and-applying-genomic-deep-learning-models/)



##### [**Opportunities** and **obstacles** for **deep learning** in **biology** and **medicine**](http://rsif.royalsocietypublishing.org/content/15/141/20170387.abstract)

T Ching, [DS Himmelstein](https://scholar.google.com/citations?user=x9OwD9oAAAAJ&hl=en&oi=sra)… - Journal of The …, 2018 - rsif.royalsocietypublishing.org

```markdown
# Abstract:
Convolutionary neural network (CNN) is a popular choice for supervised DNA motif prediction due to its excellent performances. To employ CNN, the input DNA sequences are required to be encoded as numerical values and represented as either vectors or multi-dimensional matrices. This paper evaluated a simple and more compact ordinal encoding method versus the popular one-hot encoding for DNA sequences. 

We compared the performances of both encoding methods using three sets of datasets enriched with DNA motifs. We found that 
1. the ordinal encoding performs comparable to the one-hot method but with significant reduction in training time. 
2. In addition, the one-hot encoding performances were rather consistent across various datasets but would require suitable CNN configuration to perform well. 
3. The ordinal encoding with matrix representation performed best in some of the evaluated datasets. 

This study implied that the performances of CNN for DNA motif discovery depends on the suitable design of the sequence encoding and representation. The good performances of the ordinal encoding method demonstrates that there are still rooms for improvement for the one-hot encoding method.
```



 

### Nice examples

##### By Lex Flagel
The Unreasonable Effectiveness of Convolutional Neural Networks in Population Genetic Inference
https://www.biorxiv.org/content/biorxiv/early/2018/10/22/336073.full.pdf
https://github.com/flag0010/pop_gen_cnn

##### [Evaluation of convolutionary neural networks modeling of DNA sequences using ordinal versus one-hot encoding method](https://ieeexplore.ieee.org/abstract/document/8270400)
##### "Whole-genome deep learning analysis reveals causal role of noncoding mutations in autism", Zhou et al 2018 <https://t.co/gv8KodjhDr>



##### @@[Deep learning of genomic variation and regulatory network data](https://academic.oup.com/hmg/article-abstract/27/R1/R63/4966854)

[A Telenti](https://scholar.google.com/citations?user=YkSJ7-8AAAAJ&hl=en&oi=sra), [C Lippert](https://scholar.google.com/citations?user=RVl8TE0AAAAJ&hl=en&oi=sra), [PC Chang](https://scholar.google.com/citations?user=8_8omVoAAAAJ&hl=en&oi=sra)… - Human molecular …, 2018 - academic.oup.com





### Books

[Hands-On Machine Learning with Scikit-Learn and TensorFlow](https://www.amazon.com/Hands-Machine-Learning-Scikit-Learn-TensorFlow/dp/1491962291/ref=sr_1_3?ie=UTF8&qid=1537500797&sr=8-3&keywords=machine+learning&dpID=51%252BkYprYK1L&preST=_SX218_BO1,204,203,200_QL40_&dpSrc=srch)

[The Elements of Statistical Learning](https://www.amazon.com/Elements-Statistical-Learning-Prediction-Statistics/dp/0387848576/ref=sr_1_1?ie=UTF8&qid=1537500853&sr=8-1&keywords=the+elements+of+statistical+learning&dpID=41aQrQaPseL&preST=_SY291_BO1,204,203,200_QL40_&dpSrc=srch)







### Tools

[pysster](https://github.com/budach/pysster): 

**One_Hot_Encoder**

	**One_Hot_Encoder**

Nucleus：基因组学的 TensorFlow 工具包（TensorFlow 开发顶峰 2018）

[Nucleus github ](https://github.com/google/nucleus)

	[Video](https://www.youtube.com/watch?v=7wi9NdGh9oI&feature=share)

[DeepVariant github](https://github.com/google/deepvariant)



### start-up

https://verily.com/
* formerly known as Google Life Sciences 



https://www.deepgenomics.com/
predict the effects of a particular mutation based on its analyses of hundreds of thousands of examples of other mutations; even if there’s not already a record of what those mutations do.

develop a database that provides predictions for how more than 300 million genetic variations could affect a genetic code

### Overall start-up field in genomics
https://medicalfuturist.com/top-companies-genomics

* Personal genomics
* Pharmacogenomics
* Genomics combined with Artificial Intelligence
* Precision Oncology/Medicine
* Genetic ancestry
* Sequencing tech
    * Edico Genome: having sequenced a human genome in just 26 hours in 2015 
    * the first data processor to ever be solely designed for genome sequencing, called DRAGEN.
* CRISPR gene editing 



 

=======
# Machine Learning in genomics

[TOC]





## [Wiki： Machine learning in bioinformatics](https://en.wikipedia.org/wiki/Machine_learning_in_bioinformatics)



# Entry level knowledge:



### Basic

##### [[莫烦python](https://morvanzhou.github.io/) (python 入门+ Machine Learning)

##### [TensorFlow 官方文档中文版](http://docs.pythontab.com/tensorflow/)

##### Keras Documentation](https://keras.io/) and [中文文档](https://keras-cn.readthedocs.io/en/latest/)





### People in ML

##### Geoff Hinton, google, godfather of Deep learning

University of Toronto Computer Science

https://en.wikipedia.org/wiki/Geoffrey_Hinton



##### Yann LeCun, facebook, father of CNN

http://yann.lecun.com/

https://en.wikipedia.org/wiki/Yann_LeCun



##### Yoshua Bengio

Canaca; ANN; DL;

##### Yair Weiss



# Advanced knowledge

### Useful resources:

##### A list of deep learning implementations in **biology**: [link](https://github.com/hussius/deeplearning-biology)

##### A curated list of awesome deep learning applications in the field of **computational biology** [link](https://github.com/gokceneraslan/awesome-deepbio)

##### **[Practical Deep Learning For Coders**](http://course.fast.ai/)

##### [Udemy: Deep Learning A-Z™: Hands-On Artificial Neural Networks $$](https://www.udemy.com/deeplearning/)



### YouTube

[Deep learning for genomics - Anshul Kundaje](https://youtu.be/X5mdoxR9qag)

[James Zou: "Deep learning for genomics: Introduction and examples"](
https://youtu.be/JYt1IqdDAPc)



##### [James Zhou Teaching](https://sites.google.com/site/jamesyzou/teaching)

**CS 329M Algorithms of advanced machine learning.**  **(website)**https://canvas.stanford.edu/courses/51037

**CS 273B Deep learning in genomics and bio-medicine.** **(website)** https://canvas.stanford.edu/courses/66218/

see my github for the downloaed course material



##### [Anshul Kundaje Teaching](https://sites.google.com/site/anshulkundaje/teaching)

Tutorials: https://sites.google.com/site/anshulkundaje/inotes





### Chinese in ML

##### Yifei Chen

https://scholar.google.com/citations?user=ygovHrsAAAAJ&hl=en

Department of Computer Science, University of California, Irvine, CA 92697, USA

##### [JIAN ZHOU](http://www.princeton.edu/~jzthree/)

http://www.princeton.edu/~jzthree/

##### James Zhou

https://sites.google.com/site/jamesyzou/home




### Papers:

##### [Evolutionarily informed deep learning methods: Predicting transcript abundance from DNA sequence](https://www.biorxiv.org/content/early/2018/07/19/372367)



##### [Deep Learning for Genomics: A Concise Overview](https://arxiv.org/abs/1802.00810)



##### [Deep learning for biology](https://www.nature.com/articles/d41586-018-02174-z)



##### [Deep Learning for Population Genetic Inference](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004845)

```
 * jointly inferring natural selection and demography
 
 * We find many regions of the genome that have experienced hard sweeps, and fewer under selection on standing variation (soft sweep) or balancing selection.
 
```

##### [Deep learning for computational biology](http://msb.embopress.org/content/12/7/878.abstract)

[C Angermueller](https://scholar.google.com/citations?user=OXZC0mQAAAAJ&hl=en&oi=sra), T Pärnamaa, [L Parts](https://scholar.google.com/citations?user=ktEf4ZUAAAAJ&hl=en&oi=sra)… - Molecular systems …, 2016 - msb.embopress.org

```markdown
# the most accurate prediction of gene expression levels is currently made from a broad set of epigenetic features using sparse linear models (Karlic et al, 2010; Cheng et al, 2011) or random forests (Li et al, 2015)

Most of these applications can be described within the canonical machine learning workflow, which involves four steps: 
* data cleaning and pre‐processing, 
* feature extraction, 
* model fitting and 
* evaluation 

A major recent advance in machine learning is automating this critical step by learning a suitable representation of the data with deep artificial neural networks

Briefly, a deep neural network takes the raw data at the lowest (input) layer and transforms them into increasingly abstract feature representations by successively combining outputs from the preceding layer in a data‐driven manner, encapsulating highly complicated functions in the process

depth of the layer X the width of the layer

backward propagation algorithm ultimately enabling efficient training of neural networks using stochastic gradient descent


其他的DNN变形
convolutional neural networks, which are widely used for **modelling images**
recurrent neural networks for **sequential data**
restricted Boltzmann machines and autoencoders for **unsupervised learning**

comprehensive background on all technical details, which can be found in the more specialized literature (Bengio, 2012; Bengio et al, 2013; Deng, 2014; Schmidhuber, 2015; Goodfellow et al, 2016). 
```



##### [*Machine learning** applications in **genetics** and **genomics**](https://www.nature.com/articles/nrg3920)

[MW Libbrecht](https://scholar.google.com/citations?user=O4SMk-sAAAAJ&hl=en&oi=sra), [WS Noble](https://scholar.google.com/citations?user=plt2_DsAAAAJ&hl=en&oi=sra) - Nature Reviews **Genetics**, 2015 - nature.com



##### [Machine Learning in Genomics – Current Efforts and Future Applications](https://www.techemergence.com/machine-learning-in-genomics-applications/)



##### [Deep learning meets genome biology](https://www.oreilly.com/ideas/deep-learning-meets-genome-biology)

An interview with Brendan Frey about realizing new possibilities in genomic medicine.



##### [TRAINING AND APPLYING GENOMIC DEEP LEARNING MODELS](https://blog.dnanexus.com/2018-05-31-training-and-applying-genomic-deep-learning-models/)



##### [**Opportunities** and **obstacles** for **deep learning** in **biology** and **medicine**](http://rsif.royalsocietypublishing.org/content/15/141/20170387.abstract)

T Ching, [DS Himmelstein](https://scholar.google.com/citations?user=x9OwD9oAAAAJ&hl=en&oi=sra)… - Journal of The …, 2018 - rsif.royalsocietypublishing.org

```markdown
# Abstract:
Convolutionary neural network (CNN) is a popular choice for supervised DNA motif prediction due to its excellent performances. To employ CNN, the input DNA sequences are required to be encoded as numerical values and represented as either vectors or multi-dimensional matrices. This paper evaluated a simple and more compact ordinal encoding method versus the popular one-hot encoding for DNA sequences. 

We compared the performances of both encoding methods using three sets of datasets enriched with DNA motifs. We found that 
1. the ordinal encoding performs comparable to the one-hot method but with significant reduction in training time. 
2. In addition, the one-hot encoding performances were rather consistent across various datasets but would require suitable CNN configuration to perform well. 
3. The ordinal encoding with matrix representation performed best in some of the evaluated datasets. 

This study implied that the performances of CNN for DNA motif discovery depends on the suitable design of the sequence encoding and representation. The good performances of the ordinal encoding method demonstrates that there are still rooms for improvement for the one-hot encoding method.
```



 

### Nice examples

##### By Lex Flagel
The Unreasonable Effectiveness of Convolutional Neural Networks in Population Genetic Inference
https://www.biorxiv.org/content/biorxiv/early/2018/10/22/336073.full.pdf
https://github.com/flag0010/pop_gen_cnn

##### [Evaluation of convolutionary neural networks modeling of DNA sequences using ordinal versus one-hot encoding method](https://ieeexplore.ieee.org/abstract/document/8270400)
##### "Whole-genome deep learning analysis reveals causal role of noncoding mutations in autism", Zhou et al 2018 <https://t.co/gv8KodjhDr>



##### @@[Deep learning of genomic variation and regulatory network data](https://academic.oup.com/hmg/article-abstract/27/R1/R63/4966854)

[A Telenti](https://scholar.google.com/citations?user=YkSJ7-8AAAAJ&hl=en&oi=sra), [C Lippert](https://scholar.google.com/citations?user=RVl8TE0AAAAJ&hl=en&oi=sra), [PC Chang](https://scholar.google.com/citations?user=8_8omVoAAAAJ&hl=en&oi=sra)… - Human molecular …, 2018 - academic.oup.com





### Books

[Hands-On Machine Learning with Scikit-Learn and TensorFlow](https://www.amazon.com/Hands-Machine-Learning-Scikit-Learn-TensorFlow/dp/1491962291/ref=sr_1_3?ie=UTF8&qid=1537500797&sr=8-3&keywords=machine+learning&dpID=51%252BkYprYK1L&preST=_SX218_BO1,204,203,200_QL40_&dpSrc=srch)

[The Elements of Statistical Learning](https://www.amazon.com/Elements-Statistical-Learning-Prediction-Statistics/dp/0387848576/ref=sr_1_1?ie=UTF8&qid=1537500853&sr=8-1&keywords=the+elements+of+statistical+learning&dpID=41aQrQaPseL&preST=_SY291_BO1,204,203,200_QL40_&dpSrc=srch)







### Tools

[pysster](https://github.com/budach/pysster): 

**One_Hot_Encoder**

	**One_Hot_Encoder**

Nucleus：基因组学的 TensorFlow 工具包（TensorFlow 开发顶峰 2018）

[Nucleus github ](https://github.com/google/nucleus)

	[Video](https://www.youtube.com/watch?v=7wi9NdGh9oI&feature=share)

[DeepVariant github](https://github.com/google/deepvariant)



### start-up

https://verily.com/
* formerly known as Google Life Sciences 



https://www.deepgenomics.com/
predict the effects of a particular mutation based on its analyses of hundreds of thousands of examples of other mutations; even if there’s not already a record of what those mutations do.

develop a database that provides predictions for how more than 300 million genetic variations could affect a genetic code

track record of publishing at top machine learning conferences (NIPS, ICML, ICLR) or has applied deep learning to genomics in a top life sciences journal.

### Overall start-up field in genomics
https://medicalfuturist.com/top-companies-genomics

* Personal genomics
* Pharmacogenomics
* Genomics combined with Artificial Intelligence
* Precision Oncology/Medicine
* Genetic ancestry
* Sequencing tech
    * Edico Genome: having sequenced a human genome in just 26 hours in 2015 
    * the first data processor to ever be solely designed for genome sequencing, called DRAGEN.
* CRISPR gene editing 

The Incredible Convergence Of Deep Learning And Genomics.pdf
https://github.com/xinshuaiqi/My_books/blob/master/The%20Incredible%20Convergence%20Of%20Deep%20Learning%20And%20Genomics.pdf
 

>>>>>>> 77efe550385b7a5c24be99a2d9e12cfd1056e220
