# BASAR-Black-box-Attack-on-Skeletal-Action-Recognition
BASAR:Black-box Attack on Skeletal Action Recognition, CVPR 2021

## Description

This is the source code of our CVPR 2021 paper: BASAR:Black-box Attack on Skeletal Action Recognition. BASAR is the first black-box adversarial attack approach for skeletal motions, which explores the interplay between the classifiation boundary and the natural motion manifold.  

Paper here: https://arxiv.org/abs/2103.05266

### Dependencies

Below is the key environment under which the code was developed, not necessarily the minimal requirements:

1. Python 3.7
2. pytorch 1.8.1
3. Cuda 11.2

And other libraries such as numpy and GEKKO. GEKKO is designed for large-scale optimization and accesses solvers of constrained, unconstrained, continuous, and discrete problems. The method to obtain GEKKO and tutorials can be found in https://apmonitor.com/wiki/index.php/Main/GekkoPythonOptimization. 

### Installing
No installation needed other than dependencies.

### Warning
The code has not been exhaustively tested. You need to run it at your own risk. The author will try to actively maintain it and fix reported bugs but this can be delayed.

### HDM05 demo

* The code assumes that you have normalised your data and know how to recover it after learning.
* After attack, we provide a not-so-structured code snippet for unnormalising the adversarial samples in datapress/post-processing.py

You can download the pre-processed data from [GoogleDrive](https://drive.google.com/file/d/1LyD-jf3X20wBbhKu071AwDDYvzFN7wjT/view?usp=sharing) or [BaiduYun(password:fmhm)](https://pan.baidu.com/s/1Itb94YjwUVqZmM9HLW6U3g) and extract files with
``` 
cd data
unzip <path to hdm05.zip>
```
run 

``` 
cd demo
python untargeted_attack_op_stgcn_hdm05.py
```

### Apologies

Due to the workload, the code is not constructed perfectly. Some code reading is probably needed before you can run the code. 

## Authors

Yunfeng Diao, Tianjia Shao, Yongliang Yang, Kun Zhou and He Wang

Yunfeng Diao, dyf@my.swjtu.edu.cn

He Wang, h.e.wang@leeds.ac.uk, [Personal website](https://drhewang.com)

Project Webpage: http://drhewang.com/pages/AAHAR.html

## Version History
* 0.1
    * Initial Release

## Citation (Bibtex)
Please cite our papers if you find it useful:

1. Yunfeng Diao, Tianjia Shao, Yongliang Yang, Kun Zhou and He Wang, BASAR:Black-box Attack on Skeletal Action Recognition, CVPR 2021

    @InProceedings{Diao_Basar_2020,
    author={Yunfeng Diao, Tianjia Shao, Yongliang Yang, Kun Zhou and He Wang},
    booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
    title={BASAR:Black-box Attack on Skeletal Action Recognition},
    year={2021},
    month={June},
}

2. He Wang, Feixiang He, Zhexi Peng, Tianjia Shao, Yongliang Yang, Kun Zhou and David Hogg, Understanding the Robustness of Skeleton-based Action Recognition under Adversarial Attack, CVPR 2021

    @InProceedings{Wang_Understanding_2020,
    author={He Wang, Feixiang He, Zhexi Peng, Tianjia Shao, Yongliang Yang, Kun Zhou and David Hogg},
    booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
    title={Understanding the Robustness of Skeleton-based Action Recognition under Adversarial Attack},
    year={2021},
    month={June},
    }


## Contact
Please email Yunfeng Diao dyf@my.swjtu.edu.cn for further questions.

## Acknowledgments
This project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement No 899739 CrowdDNA, EPSRC (EP/R031193/1), NSF China (No. 61772462, No. U1736217), RCUK grant CAMERA (EP/M023281/1, EP/T014865/1) and the 100 Talents Program of Zhejiang University.
