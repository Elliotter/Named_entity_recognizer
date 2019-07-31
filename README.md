# Named_entity_recognizer
## WHY CREATING THIS PROJECT
Named-entity-recognizer has been a baisc task in natural language processing(NLP) and there have been lots of algorism proposed to achieve
the state-of-art results.In this project I will employ different methods and try to figure out what is exactly going on in each part of model
(only deep learning model here) or how much each part contributes to the final results. This may help us have a better understand of deep neural networks,especially when we have to design our own model without ready-made models can be referred to. 
## Content
### data
1. data:we transfer data into shape of [sen_num,sen_len] and get **datatrain_data.npy / train_label.npy / test_data.npy / test_label.npy**
(sometimes the length of the sentence is needed,train_sen_len.npy,test_sen_len.npy)
2. embeddings:we train word embedding with NLP tools(word2vec/fasttext/glove) and get **embeddings.npy** which index/value mapped to dict **word2id.txt** ( The first line of the matrix must be zero which represents padding or word that is not in range of embedding model)
3. position encoding:recommend auto_encoder network to encode absolute position embedding and employ function sin/cos to encode relative position
4. other features
### 

