# MvMHAT: Multi-view Multi-Human Association and Tracking

> [**Self-supervised Multi-view Multi-Human Association and Tracking**](https://github.com/realgump/MvMHAT/blob/main/readme/PDF%20coming%20soon),            
> Yiyang Gan, Ruize Han, Liqiang Yin, Wei Feng, Song Wang

- A self-supervised learning framework for MvMHAT.
- A new benchmark for training and testing MvMHAT.

Contact: [realgump@tju.edu.cn](mailto:realgump@tju.edu.cn). Any questions or discussions are welcomed! 

![](https://github.com/realgump/MvMHAT/blob/main/readme/1.jpg)


## Abstract
Multi-human association and tracking (MHAT) with multi-view cameras, aims to track a group of people over time in each view, meanwhile, identify the same person across different views at the same time. This is a relatively new problem but has significance for multi-person scene video surveillance. Different from previous multiple object tracking (MOT) and multi-target multi-camera tracking (MTMCT) tasks, which only consider the over-time human association, multi-view MHAT requires to jointly achieve the cross-spatial-temporal data association. In this paper, we model this problem with a self-supervised learning framework and propose an end-to-end network to solve it. Specifically, we proposed a spatial-temporal association network with three designed self-supervised learning losses including self-similarity loss, transitive-similarity loss, and symmetrical-consistency loss, to simultaneously associate the human over time and across views. Besides, to promote the research on multi-view MHAT, we build a new large-scale benchmark for algorithm training and testing. Extensive experiments on the proposed datasets verify the effectiveness of our method.

![](https://github.com/realgump/MvMHAT/blob/main/readme/2.jpg)

## Install
The code was tested on Ubuntu 16.04, with Anaconda Python 3.6 and PyTorch v1.7.1. NVIDIA GPUs are needed for both training and testing. After install Anaconda:
0. [Optional but recommended] create a new conda environment：
~~~
   conda create -n MVMHAT python=3.6
~~~
And activate the environment:
~~~
   conda activate MVMHAT
~~~
1. Install pytorch:
~~~
   conda install pytorch=1.7.1 torchvision -c pytorch
~~~
2. Clone the repository:
~~~
   MVMHAT_ROOT=/path/to/clone/MVMHAT
   git clone https://github.com/realgump/MvMHAT.git $MVMHAT_ROOT
~~~
3. Install the requirements:
~~~
   pip install -r requirements.txt
~~~
4. Download the pretrained model to promote convergence:
~~~
   cd $MVMHAT_ROOT/model
   wget https://download.pytorch.org/models/resnet50-19c8e357.pth
~~~

## Citation
If you find this project useful for your research, please use the following BibTeX entry.

    @inproceedings{gan2021mvmhat,
      title={Self-supervised Multi-view Multi-Human Association and Tracking},
      author={Yiyang Gan, Ruize Han, Liqiang Yin, Wei Feng, Song Wang},
      booktitle={ACM MM},
      year={2021}
    }

## References
Portions of the code are borrowed from [deep-sort](https://github.com/nwojke/deep_sort), thanks for their great work.

**More information is coming soon ...**
