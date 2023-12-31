﻿# 260D_Online_Batch_Selection_Forgetting_Score
This study delves into the efficacy of online batch selection in neural network
training, focusing on the impact of forgetting scores on training dynamics. We
commence by establishing a baseline model using a simple neural network architec-
ture on the MNIST dataset, prioritizing the observation of accuracy changes over
outright performance. Our methodology incorporates two novel online batch selec-
tion techniques—probabilistic and deterministic—based on dynamically tracked
forgetting scores of training examples. We initially observe that these methods do
not offer a significant advantage over random batch selection on the MNIST dataset,
possibly due to the low forgettability of its examples. However, upon extending our
analysis to the more complex CIFAR-10 dataset, we discover that while our meth-
ods initially outperform random selection, they gradually lose this edge, suggesting
potential overfitting to challenging examples. This research contributes to the
understanding of batch selection strategies in neural network training, particularly
in contexts where data forgettability plays a crucial role. Our findings suggest
avenues for further refinement of online batch selection techniques, especially in
balancing computational efficiency and learning effectiveness in more complex
datasets.

Below is a description of files included:
probalisitic_sgd.ipynb
- initial implementation of methods and initial testing
260DProject.ipynb
- final testing of methods on MNIST dataset
- initally implemented and included standard sgd (no online batch selection). after
  referring with professor, realized random selection and standard were equivalent
  so not included in paper
- future work covered testing on noisy examples, tried rudimentary approach but
  decided not to include results in paper
cifar10.ipynb
- final testing of methods on CIFAR-10 dataset
- diffferent data visualizations to try to understand patterns of our methods
