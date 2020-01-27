# Deep-Learning-Sequence-Models
Coursera Course
Course Webiste https://www.coursera.org/learn/nlp-sequence-models/home/welcome

1.1 Sampling novel sequences in RNN
- Use the probabilities output by the RNN to randomly sample a chosen word for that time-step as y^(t), Then pass this selected word to the next time-step

1.2 Gated Recurrent Unit (GRU)
-  when Gamma_u =0 (gate=0), C<t> is only dependent on C<t-1>, means don't update, thus it doesn't suffer from much of a vanishing gradient problem
