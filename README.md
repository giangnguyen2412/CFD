# Citation
If you find our work useful in your research, please consider citing:

```
@inproceedings{nguyen2021explaining,
  title={Explaining how deep neural networks forget by deep visualization},
  author={Nguyen, Giang and Chen, Shuan and Jun, Tae Joon and Kim, Daeyoung},
  booktitle={International Conference on Pattern Recognition},
  pages={162--173},
  year={2021},
  organization={Springer}
}
```

# CFD
Code for "Explaining How Deep Neural Networks Forget by Deep Visualization" or "Dissecting Catastrophic Forgetting in Continual Learning by Deep Visualization"

Linked to this [repo](https://github.com/giangnguyen2412/dissect_catastrophic_forgetting)

## How if the output of CFD is layer 1?
- We are observing the IoU drop, then the result of CFD is greater than 1.

## Do we always freeze the 1st layer in CF?
- Nope. We run CFD and CF independently. After running CFD to analyze catastrophic forgetting, you can determine to apply CF or not.
If not, your feature extractor will update new global information on earlier layers. 
