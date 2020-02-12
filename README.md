# Deep-Learning-Sequence-Models
Coursera Course
Course Webiste https://www.coursera.org/learn/nlp-sequence-models/home/welcome

1.1 Sampling novel sequences in RNN
- Use the probabilities output by the RNN to randomly sample a chosen word for that time-step as y^(t), Then pass this selected word to the next time-step

1.2 Gated Recurrent Unit (GRU)
-  when Gamma_u =0 (gate=0), C<t> is only dependent on C<t-1>, means don't update, thus it doesn't suffer from much of a vanishing gradient problem

1.3 Logistic Regression with a Neural Network mindset project
  - [Building_a_Recurrent_Neural_Network_Step_by_Step Link](Building_a_Recurrent_Neural_Network_Step_by_Step_v3a.ipynb)

1.4 Dinosaurus Land Character Level Language Model Project
 - [Dinosaurus Land Character Level Language Model](Dinosaurus_Island_Character_level_language_model_final_v3a.ipynb)
 
1.5 Improvise a Jazz Solo with an LSTM Network Project
 - [Improvise_a_Jazz_Solo_with_an_LSTM_Network](Improvise_a_Jazz_Solo_with_an_LSTM_Network_v3a.ipynb)
 - [Generated Musci] (my_music.midi)

2.1 Embedding Vector
 -  The dimension of embedding word vectors is usually smaller than the size of the vocabulary. Most common sizes for word vectors ranges between 50 and 400
 - 	T-SNE: t-distributed stochastic neighbor embedding , is a non-linear dimensionality reduction technique
 -  The word vectors empower your model with an incredible ability to generalize. 
 
 2.2 Embedding Matrix
 - Usually we dont' use E*O1234 because it is computationally wasteful. The elemen-wise multiplication will be extremely inefficient.
 
 2.3 Learning word embeddings - Word2vec  
 - When learning word embeddings, we create an artificial task of estimating P(target | context). It is okay if we do poorly on this artificial prediction task; the more important by-product of this task is that we learn a useful set of word embeddings. 
 - target and context are chosen from training set so that they are nearby words
 - Skip-grams: Theta_t and ec are the same dimensions; they are both trained with an optimization algorithm such as Adam or gradient descent.
 
 2.4 Learning word embeddings - Glove
 - Thetai and ej should be initialized randomly at the beginning of training
 - Xij is the number of times word I appears in the context of word j
 - The weighting function f(.) must satisfy f(0)=0; The weighting function helps prevent learning only from extremely common word pairs.
  - Using word embeddings is a form of transfer learning, trained word embeddings should >= separate labeled dataset for your task

2.5 Operations on word vectors Project
 - [Operations on word vectors](Operations_on_word_vectors_v2a.ipynb)
 
2.6 Emojify Project
 - [Emojify Project Link](Emojify_v2a.ipynb)

3.1 Basic Models
 	- Machine translation can be considered as a "conditional language model", the condition is a input sentence to be translated. 
	- The job of green portion (encoder) is to find an encoding of the input sentence (some representation of the input rather than all zeros in language model). The decoder network's job is to generate the corresponding translation.
  - The purple (decoder network) looks identical to the language model that predict the probability of the input sentence.
