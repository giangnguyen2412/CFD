# CFD
Code for "Explaining How Deep Neural Networks Forget by Deep Visualization" or "Dissecting Catastrophic Forgetting in Continual Learning by Deep Visualization"

Linked to this [repo](https://github.com/giangnguyen2412/dissect_catastrophic_forgetting)

## How if the output of CFD is layer 1?
- We are observing the IoU drop, then the result of CFD is greater than 1.

## Do we always freeze the 1st layer in CF?
- Nope. We run CFD and CF independently. After running CFD to analyze catastrophic forgetting, you can determine to apply CF or not.
If not, your feature extractor will update new global information on earlier layers. 
