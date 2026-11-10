---
layout: default
title: Edwards Tong
---

# Quarter 2 Project Reflections

**Name:** Edwards Tong  
**UCSD email:** [edtong@ucsd.edu](mailto:edtong@ucsd.edu)  
**Section:** D25  
**Mentor:** Jingbo Shang

**What is the most interesting topic covered in your domain this quarter?**

The most interesting topic to me is how changing the order of examples in a prompt can change a language model's answers. This is part of in-context learning, where a model uses examples in the prompt to help answer a new question. The paper we are studying shows that changing the order can matter about as much as choosing different examples. I find this surprising because the examples still contain the same information. I want to understand how we can find a good order and check that it also works on new questions.

**Describe a potential investigation you would like to pursue for your Quarter 2 Project.**

I would like to study whether we can find a good example order with fewer model runs. I would start with one small open-source model and a dataset where the model chooses a category for each input. I would compare trying random orders with a method that swaps two examples at a time and keeps changes that improve the score. Both methods would use the same examples and the same number of model runs. I would choose the order using a development set, which is data used to improve the method, and then check it on a separate test set. I would compare accuracy, time used, and how much the results change across repeated runs. If time allows, I would try a second dataset.

**What is a potential change you'd make to the approach taken in your current Quarter 1 Project?**

Our Quarter 1 project is to recreate results from [*Order Matters: Rethinking Prompt Construction in In-Context Learning*](https://arxiv.org/abs/2511.09700). After recreating the main results, I would repeat the experiments with different random choices to see how much the results change. This would help us check whether the findings are reliable rather than the result of one lucky run. I would follow the paper's rule for putting examples in a starting order, so we can compare changing the examples with changing their order fairly. I would also test whether trying more orders improves accuracy enough to be worth the extra time. I would use development data to choose an order and keep test data separate for the final check.

**What other techniques would you be interested in using in your project?**

I would like to try ordering examples by how similar they are to the question being asked. I would also try improving an order by swapping two examples at a time. I would compare these methods with random orders while keeping the examples and number of model runs the same. Another idea is to run the model with several orders and use the answer chosen most often. This might make its answers more reliable. Finally, I would check whether an order that works well on one dataset also works on another, since the paper shows that this is not always the case.
