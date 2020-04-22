<h3 align="center">Technical test - ParkDepot</h3>
<p align="center">A deep learning classifier on german plates<p>
  
### Task
- Detect if a plate has **1, 2 or 3 letters for the city description**
- Implement a deep learning classifier
### Dataset
- Real plates 
- Synthetic plates, taht have been generated to construct a bigger dataset
- *Input, example of such a plate:*
<div align="center">
<img src="./MN_NA1998.png" height="40">
</div>

### Used method
- A strong preprocessing pipeline to split data into usable training/validation sets and to transform data dimension
- A manually implemented ResNet model, following the [original paper](https://arxiv.org/abs/1512.03385)
  -  Redefinition of the residual blocks and stacks in PyTorch
- Use of a classic SGD optimizer (`lr=1e-2, momentum=0.9, weight_decay=1e-2`)
- Use of Google GPU capacity, hence the **Google Colab [notebook](./ParkDepot_technical_test.ipynb)**.
### Results
- High final accuracy (0.999%) on test data
