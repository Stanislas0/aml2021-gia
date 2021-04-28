# AML2021-Graph Injection Attack & Defense
This is the repository of the project of AML2021: Graph injection attack &amp; defense.

## Usage

The file ```gia_demo.ipynb``` provides an notebook example of the entire process of applying a graph injection attack:

* Data preparation: Use a [Refined Cora](https://github.com/THUDM/Refined-cora-citeseer) dataset as an example. (Download the data and put them in ```/data``)
* Model preparation: [GCN](https://arxiv.org/abs/1609.02907) model as the surrogate model.
* Graph injection attack: Apply [FGSM](https://arxiv.org/abs/1412.6572) attack on the surrogate model and transfer the results to other models (e.g. [GIN](https://arxiv.org/abs/1810.00826), [TAGCN](https://arxiv.org/abs/1710.10370)).

See more details in the file. The trained weights of GIN and TAGCN are saved in ```/saved_models```. The example of generated attack features and adjacency matrix are saved in ```/results```. 

## Requirements

* scipy==1.5.2
* numpy==1.19.1
* torch==1.8.0

## References

* [KDD CUP 2020 official site](https://www.biendata.xyz/competition/kddcup_2020_formal/)
* [KDD CUP 2020 1st-place solution](https://github.com/Stanislas0/KDD_CUP_2020_MLTrack2_SPEIT)

## Contact

If you have any question, please raise an issue or concat qinkai@tsinghua.edu.cn or zoux18@tsinghua.edu.cn.

