# knowledge-distillation
This repository contains experiments with Knowledge Distillation on a variety of datasets and tasks.

**Knowledge Distillation** is a technique that is used for generating *lightweight, production-suitable* models while compromising very little on the model performance.

It makes use of a unique training process:
1. A heavy and complex model (Teacher) is trained to an optimal degree on a task.
2. A lighter and simpler model (Student) is trained on a combination of hard targets (the target variable) and soft targets (the logits of the Teacher model).

Deeper details of the training, like the loss function and parameters, are described in the notebooks.

The advantages of using the Student model are that it's much quicker at inference and interestingly, preserves the [dark knowledge](https://www.ttic.edu/dl/dark14.pdf) of the data.
