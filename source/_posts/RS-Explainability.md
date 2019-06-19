---
title: RS_Explainability 
toc: true
date: 2019-06-07 23:56:11
tags:
categories: Recommendation_System
---

<img src="Explainable-RS/ExplainableRS0.png" width=500px />

**PanXiang**
							2019.4.9

__Problem__

why such items are recommended

why they not only provideusers with the recommendations

effectiveness

efficiency

persuasiveness

user satisfaction

(how presented)display style:text/visual

(what information used)model:matrix factorization\,topic modeling\, graphbased models\, deep learning\, knowledge\-graph embedding\,  association rule mining

__Time Line__

__CF(Memory\-Based)__

__C__  __ontent\-__  __B__  __ased__  __CF(feature based)__

(price\, color\, brand of the goods in e\-commerce\, or the genre\, director\, duration of the movies inreview systems)

__User\-based CF__  __(user embedding?)__

__Item\-based CF(Item embedding?)__

MF(Model\-Based)

生成式模型/判别式模型?

__MF__

__LFM(Latent Factor Model)__

m user

n  item

A: user\-(item favor value)

U: user\-feature

V: feature\-(itemfavor value)

<img src="Explainable-RS/ExplainableRS1.png" width=277px />

<img src="Explainable-RS/ExplainableRS2.png" width=500px />

__MF__

__LFM(Latent Factor Model)__  __/Singular Value Decomposition(SVD)?__

m user

n  item

A: user\-(item favor value)

U: user\-feature

V: feature\-(itemfavor value)

<img src="Explainable-RS/ExplainableRS3.png" width=277px />

<img src="Explainable-RS/ExplainableRS4.png" width=451px />

<img src="Explainable-RS/ExplainableRS5.png" width=500px />

<img src="Explainable-RS/ExplainableRS6.png" width=500px />

<img src="Explainable-RS/ExplainableRS7.png" width=227px />

<img src="Explainable-RS/ExplainableRS8.png" width=500px />

yi反应喜好偏置

I(u)所有交互

<img src="Explainable-RS/ExplainableRS9.png" width=500px />

behaviour can reflect favor

2008 KDD Factorization Meets the Neighborhood: a Multifaceted Collaborative Filtering Model

__E__  __FM(Explicit Factor Model)__

\+explicit user opinions

explicit product features

user opinions by phrase\-level sentiment analysis on user reviews

generate according to specific product features to the user’s interests and the hidden features learned

SIGIR 2014Explicit Factor Models for Explainable Recommendation based on Phrase\-level Sentiment Analysis

__EFM(Explicit Factor Model)__

<img src="Explainable-RS/ExplainableRS10.png" width=500px />

<img src="Explainable-RS/ExplainableRS11.png" width=500px />

SIGIR 2014Explicit Factor Models for Explainable Recommendation based on Phrase\-level Sentiment Analysis

__EFM(Explicit Factor Model)__

<img src="Explainable-RS/ExplainableRS12.png" width=500px />

N=5 for five stars

feature Fj is mentioned by user ui for tij times

<img src="Explainable-RS/ExplainableRS13.png" width=500px />

Fj is mentioned for k times on item pi

SIGIR 2014Explicit Factor Models for Explainable Recommendation based on Phrase\-level Sentiment Analysis

__EFM(Explicit Factor Model)__

__Explicit__  __features__

<img src="Explainable-RS/ExplainableRS14.png" width=500px />

feature: screen/earphone

factor: ???

X:user\-feature attention matrix

Y:item\-feature quality matrix

U1 user\- factor

V    feature\-factor

U2 item\- factor

r factor nums

m user

p feature

n item

SIGIR 2014Explicit Factor Models for Explainable Recommendation based on Phrase\-level Sentiment Analysis

__EFM(Explicit Factor Model)__

__Latent__  __f__  __actors__

<img src="Explainable-RS/ExplainableRS15.png" width=500px />

<img src="Explainable-RS/ExplainableRS16.png" width=500px />

When r = 0\, this model reduces to a traditional latent factorization model on user\-item rating matrix A

which means that the explicit features are not used for recommendations

__EFM(Explicit Factor Model)__  __\+SVD\+\+?__

<img src="Explainable-RS/ExplainableRS17.png" width=500px />

<img src="Explainable-RS/ExplainableRS18.png" width=500px />

<img src="Explainable-RS/ExplainableRS19.png" width=500px />

<img src="Explainable-RS/ExplainableRS20.png" width=410px />

SIGIR’18 Explainable Recommendation via Multi\-Task Learning in Opinionated Text Data

<img src="Explainable-RS/ExplainableRS21.png" width=500px />

<img src="Explainable-RS/ExplainableRS22.png" width=500px />

__ConvMF=CNN\+PMF__

__PMF__

R: score Mat

posterior probability

M item

N doc

<img src="Explainable-RS/ExplainableRS23.png" width=500px />

<img src="Explainable-RS/ExplainableRS24.png" width=481px />

<img src="Explainable-RS/ExplainableRS25.png" width=500px />

<img src="Explainable-RS/ExplainableRS26.png" width=156px />

<img src="Explainable-RS/ExplainableRS27.png" width=500px />

<img src="Explainable-RS/ExplainableRS28.png" width=128px />

<img src="Explainable-RS/ExplainableRS29.png" width=129px />

<img src="Explainable-RS/ExplainableRS30.png" width=500px />

<img src="Explainable-RS/ExplainableRS31.png" width=381px />

2016Convolutional matrix factorization for document context\-aware recommendation

__CNN:__

__(Music:Fourier\->image\->CNN predict__

__Genetrate Feature)__

Conv \-Classification\->feature extraction

MF    \-Regression

2016Convolutional matrix factorization for document context\-aware recommendation

<img src="Explainable-RS/ExplainableRS32.png" width=500px />

Z\[t\]:update gate vector

R\[t\]:reset gate vector

RecSys17 Sequential User\-based Recurrent Neural Network Recommendations

<img src="Explainable-RS/ExplainableRS33.png" width=500px />

<img src="Explainable-RS/ExplainableRS34.png" width=491px />

<img src="Explainable-RS/ExplainableRS35.png" width=500px />

RecSys17 Sequential User\-based Recurrent Neural Network Recommendations

<img src="Explainable-RS/ExplainableRS36.png" width=500px />

<img src="Explainable-RS/ExplainableRS37.png" width=500px />

__Text__

__Sentence:__

__Topic words:(features)__

__Visual__

__Friends__

<img src="Explainable-RS/ExplainableRS38.png" width=500px />

<img src="Explainable-RS/ExplainableRS39.png" width=473px />

<img src="Explainable-RS/ExplainableRS40.png" width=500px />

<img src="Explainable-RS/ExplainableRS41.png" width=500px />

<img src="Explainable-RS/ExplainableRS42.png" width=500px />

generated character by

character

<img src="Explainable-RS/ExplainableRS43.png" width=500px />

concatenated word

embeddings of user\, item\, and rating

2018Automatic Generation of Natural Language Explanations

<img src="Explainable-RS/ExplainableRS44.png" width=500px />

__Text\-based(NLP)__

<img src="Explainable-RS/ExplainableRS45.png" width=500px />

2018Automatic Generation of Natural Language Explanations

<img src="Explainable-RS/ExplainableRS46.png" width=500px />

__Text\-based(NLP)__

<img src="Explainable-RS/ExplainableRS47.png" width=500px />

2018Automatic Generation of Natural Language Explanations

<img src="Explainable-RS/ExplainableRS48.png" width=500px />

<img src="Explainable-RS/ExplainableRS49.png" width=500px />

__Knowledge\-base__  __=path comlpetion__

<img src="Explainable-RS/ExplainableRS50.png" width=500px />

<img src="Explainable-RS/ExplainableRS51.png" width=500px />

2019Unifying Knowledge Graph Learning and Recommendation: Towards a Better Understanding of User Preferences

__Knowledge\-base__

<img src="Explainable-RS/ExplainableRS52.png" width=500px />

AAAI2019Unifying Knowledge Graph Learning and Recommendation: Towards a Better Understanding of User Preferences

__Knowledge\-base__

<img src="Explainable-RS/ExplainableRS53.png" width=500px />

AAAI2019Unifying Knowledge Graph Learning and Recommendation: Towards a Better Understanding of User Preferences

__Knowledge\-base__

TransE

TransH

It assumes that each relation

owns a hyperplane\, and the translation between head entity and

tail entity is valid only if they are projected to the same hyperplane

<img src="Explainable-RS/ExplainableRS54.png" width=139px />

<img src="Explainable-RS/ExplainableRS55.png" width=176px />

<img src="Explainable-RS/ExplainableRS56.png" width=500px />

WWW2019Unifying Knowledge Graph Learning and Recommendation:Towards a Better Understanding of User Preferences

__Knowledge\-base__

TransH

<img src="Explainable-RS/ExplainableRS57.png" width=500px />

<img src="Explainable-RS/ExplainableRS58.png" width=242px />

<img src="Explainable-RS/ExplainableRS59.png" width=500px />

<img src="Explainable-RS/ExplainableRS60.png" width=500px />

WWW2019Unifying Knowledge Graph Learning and Recommendation:Towards a Better Understanding of User Preferences

__Evaluation\-RS__

<img src="Explainable-RS/ExplainableRS61.png" width=500px />

<img src="Explainable-RS/ExplainableRS62.png" width=500px />

<img src="Explainable-RS/ExplainableRS63.png" width=500px />

reli = 1 if the i\-th element is a positive item

__Evaluation__  __\-Explainable__

explainability

EP:explainability precision

ER:explainabilityrecall

Text:

BLUE: 不同长度的统计值差异计算

Rough(Recall\-Oriented Understudy for Gisting Evaluation)

<img src="Explainable-RS/ExplainableRS64.png" width=500px />

LCSLongest Child String

Open Question

DL explainability

Heterogenous Information Modeling

Text/Image/Audio Search

Natural Language Generation for Explanation

QA System

Explanation beyond Persuasiveness

letting the user know why not to buy a certain product

the system can help to save time for the users and to win user’s trustin the system

Open Question

Aggregation of Different Explanations

__Explainable ML__

<img src="Explainable-RS/ExplainableRS65.png" width=500px />

<img src="Explainable-RS/ExplainableRS66.png" width=500px />

<img src="Explainable-RS/ExplainableRS67.png" width=500px />

<img src="Explainable-RS/ExplainableRS68.png" width=500px />

__Explainable__  __D__  __L__

<img src="Explainable-RS/ExplainableRS69.png" width=500px />

Understanding Black\-box Predictions via Influence Functions


