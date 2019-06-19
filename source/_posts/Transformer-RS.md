---
title: RS_Transformer
toc: true
date: 2019-06-04 02:25:12
tags:
categories: Recommendation_System
---
# Behavior Sequence Transformer for E-commerce Recommendation in Alibaba
![](Transformer-RS/2019-06-04-01-10-36.png)

---


# Abstract
- **Embedding&MLP paradigm**: raw features are embedded into lowdimensional vectors
  -  ignoring the sequential nature of users’ behaviors
-  **Transformer model** to capture the sequential signals underlying users’ behavior sequences for recommendation 


---


# Transforemer(Attention is all you need)
## Architecture
![](Transformer-RS/2019-06-04-01-16-51.png)

---


![](Transformer-RS/2019-06-04-01-17-12.png)

---


![](Transformer-RS/2019-06-04-01-18-04.png)

Every encoder do not share their weights

---



## Self-Attention Encoder
Input Word->Embededing
$$ q_1=V*W_q $$
$$ k_1=V*W_k $$
$$ v_1=V*W_v $$

![](Transformer-RS/2019-06-04-01-30-16.png)

---


![](Transformer-RS/2019-06-04-01-31-21.png)

---



**Position**: diffierent distance to different pos 

![](Transformer-RS/2019-06-04-01-34-53.png)

---




## Decoder
The Unis number is O(Word)  
![](Transformer-RS/2019-06-04-01-39-58.png)  

---


![](Transformer-RS/2019-06-04-01-36-45.png)    

---



## loss  
The differience of 2 distribution
- Cross Entropy
- KL Distance
  

---




# BST

## Architecture
![](Transformer-RS/2019-06-04-01-45-45.png)


---


## Feature
### General Embedding
![](Transformer-RS/2019-06-04-01-46-58.png)

---



### Positional embedding
$$pos(v_i) = t(v_t) − t(v_i)$$

where $t(v_t)$ represents the recommending time and $t(v_i)$ the timestamp when user click item $v_i$.

---



## Transformer
### Self-attention layer  
![](Transformer-RS/2019-06-04-01-49-56.png)

---


![](Transformer-RS/2019-06-04-01-50-42.png)

---




### Point-wise Feed-Forward Networks
![](Transformer-RS/2019-06-04-01-51-23.png)


---


## MLP layers and Loss function
**binary classification problem**   
![](Transformer-RS/2019-06-04-01-52-08.png)  


---


# Result
![](Transformer-RS/2019-06-04-01-53-02.png)
![](Transformer-RS/2019-06-04-01-53-15.png)

---


![](Transformer-RS/2019-06-04-01-53-32.png)



