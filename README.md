# CAMELYON_BENCHMARK
## INTRODUCTION
### *why we do this work?*
Multiple Instance Learning **_(MIL)_** methods are mainstream approaches for pathological image classification and analysis.
The ***CAMELYON-16/17*** datasets are commonly used to evaluate ***MIL*** methods. 
However, they have the following issues:
* **_CAMELYON-16/17_** datasets contain some problematic slides
* Pixel-annotations of **_CAMELYON-16/17_** test-dataset not accurate enough
* Different **_MIL_** methods do not have a unified dataset-split and evaluation-metrics on the ***CAMELYON*** dataset
* To conclude,there is no ***BENCHMARK*** for ***MIL*** methods
### *what we do in this work?*
We do the following work to establish a ***CAMELYON-BENCHMARK***
* Remove some problematic slides.
* Correct problematic annotations.
* Merge the **_CAMELYON-16/17_** datasets and add some new slides to organize a larger, more balanced **_CAMELYON-NEW_** dataset.
* Evaluate mainstream ***MIL*** methods on the **_CAMELYON-NEW_** dataset.
* Evaluate mainstream feature extractors on the **_CAMELYON-NEW_** dataset.
* Use more comprehensive evaluation metrics to assess different methods.
* In summary, we establish a new **_CAMELYON-BENCHMARK_**.

## CAMELYON-NEW
### *balanced-dataset-split* 
* We apply balanced-dataset-split
* Details will be released soon
### *download*
* [BAIDU-PAN-LINK](https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md)
* [GOOGLE-PAN-LINK](https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md)
## BASELINE
* ***MEAN_MIL*** [Attention-based Deep Multiple Instance Learning](https://arxiv.org/abs/1802.04712) ***(ICML 2018)*** 
* ***MAX_MIL*** [Attention-based Deep Multiple Instance Learning](https://arxiv.org/abs/1802.04712) ***(ICML 2018)*** 
* ***AB_MIL*** [Attention-based Deep Multiple Instance Learning](https://arxiv.org/abs/1802.04712) ***(ICML 2018)*** 
* ***TRANS_MIL*** [Transformer based Correlated Multiple Instance Learning for WSI Classification](https://arxiv.org/abs/2106.00908) ***(NeurIPS 2021)***
* ***DS_MIL*** [Dual-stream MIL Network for WSI Classification with Self-supervised Contrastive Learning](https://arxiv.org/abs/2011.08939) ***(CVPR 2021)***
* ***CLAM_MIL*** [Data Efficient and Weakly Supervised Computational Pathology on WSI](https://arxiv.org/abs/2004.09666) ***(NAT BIOMED ENG 2021)***
* ***WENO_MIL*** [Bi-directional Weakly Supervised Knowledge Distillation for WSI Classification](https://arxiv.org/abs/2210.03664) ***(NeurIPS 2022)***
* ***DTFD_MIL*** [Double-Tier Feature Distillation MIL for Histopathology WSI Classification](https://arxiv.org/abs/2203.12081) ***(CVPR 2022)***
* ***RRT_MIL*** [Towards Foundation Model-Level Performance in Computational Pathology](https://arxiv.org/abs/2402.17228) ***(CVPR 2024)***
* ***WIKG_MIL*** [Dynamic Graph Representation with Knowledge-aware Attention for WSI Analysis](https://arxiv.org/abs/2403.07719) ***(CVPR 2024)***
* ***UPDATING...***

## FEATURE-ENCODER
* ***VIT_S (IMAGENT-PRETRAINED)*** [Transformers for Image Recognition at Scale](https://arxiv.org/abs/2010.11929) ***(ICLR 2021)*** 
* ***PLIP(WSI-Contrastive-Learning)*** [A visual–language model for WSI using medical Twitter](https://www.nature.com/articles/s41591-023-02504-3) ***(NAT MED 2023)***
* ***PLIP(WSI-Contrastive-Learning)*** [A visual–language model for WSI using medical Twitter](https://www.nature.com/articles/s41591-023-02504-3) ***(NAT MED 2023)***
* ***UPDATING...***

  
## SETTINGS
* Obtain the patches on 20X Magnification
* Keep the Hyperparameter settings of original implement
* Use uniform,balanced dataset-split


## RUSULTS
### Refine-CAMELYON-17 (4 classes)
#### *vit_s-benchmark*

|MIL|PARAMS|ACC|B-ACC|AUC|F1|PRE|
|:-----:|:-----:|:----:|:------:|:------:|:-------------:|:--------------:|
|cifar100|mobilenet|3.3M|34.02|10.56|60|60|40|40|200|
|cifar100|mobilenetv2|2.36M|31.92|09.02|60|60|40|40|200|
|cifar100|squeezenet|0.78M|30.59|8.36|60|60|40|40|200|
|cifar100|shufflenet|1.0M|29.94|8.35|60|60|40|40|200|
|cifar100|shufflenetv2|1.3M|30.49|8.49|60|60|40|40|200|
|cifar100|vgg11_bn|28.5M|31.36|11.85|60|60|40|40|200|
|cifar100|vgg13_bn|28.7M|28.00|9.71|60|60|40|40|200|
|cifar100|vgg16_bn|34.0M|27.07|8.84|60|60|40|40|200|
|cifar100|vgg19_bn|39.0M|27.77|8.84|60|60|40|40|200|
|cifar100|resnet18|11.2M|24.39|6.95|60|60|40|40|200|
|cifar100|resnet34|21.3M|23.24|6.63|60|60|40|40|200|
|cifar100|resnet50|23.7M|22.61|6.04|60|60|40|40|200|
|cifar100|resnet101|42.7M|22.22|5.61|60|60|40|40|200|
|cifar100|resnet152|58.3M|22.31|5.81|60|60|40|40|200|
|cifar100|preactresnet18|11.3M|27.08|8.53|60|60|40|40|200|
|cifar100|preactresnet34|21.5M|24.79|7.68|60|60|40|40|200|
|cifar100|preactresnet50|23.9M|25.73|8.15|60|60|40|40|200|
|cifar100|preactresnet101|42.9M|24.84|7.83|60|60|40|40|200|
|cifar100|preactresnet152|58.6M|22.71|6.62|60|60|40|40|200|
|cifar100|resnext50|14.8M|22.23|6.00|60|60|40|40|200|
|cifar100|resnext101|25.3M|22.22|5.99|60|60|40|40|200|
|cifar100|resnext152|33.3M|22.40|5.58|60|60|40|40|200|
|cifar100|attention59|55.7M|33.75|12.90|60|60|40|40|200|
|cifar100|attention92|102.5M|36.52|11.47|60|60|40|40|200|
|cifar100|densenet121|7.0M|22.99|6.45|60|60|40|40|200|
|cifar100|densenet161|26M|21.56|6.04|60|60|60|40|200|
|cifar100|densenet201|18M|21.46|5.9|60|60|40|40|200|
|cifar100|googlenet|6.2M|21.97|5.94|60|60|40|40|200|
|cifar100|inceptionv3|22.3M|22.81|6.39|60|60|40|40|200|
|cifar100|inceptionv4|41.3M|24.14|6.90|60|60|40|40|200|
|cifar100|inceptionresnetv2|65.4M|27.51|9.11|60|60|40|40|200|
|cifar100|xception|21.0M|25.07|7.32|60|60|40|40|200|
|cifar100|seresnet18|11.4M|23.56|6.68|60|60|40|40|200|
|cifar100|seresnet34|21.6M|22.07|6.12|60|60|40|40|200|
|cifar100|seresnet50|26.5M|21.42|5.58|60|60|40|40|200|
|cifar100|seresnet101|47.7M|20.98|5.41|60|60|40|40|200|
|cifar100|seresnet152|66.2M|20.66|5.19|60|60|40|40|200|
|cifar100|nasnet|5.2M|22.71|5.91|60|60|40|40|200|
|cifar100|wideresnet-40-10|55.9M|21.25|5.77|60|60|40|40|200|
|cifar100|stochasticdepth18|11.22M|31.40|8.84|60|60|40|40|200|
|cifar100|stochasticdepth34|21.36M|27.72|7.32|60|60|40|40|200|
|cifar100|stochasticdepth50|23.71M|23.35|5.76|60|60|40|40|200|
|cifar100|stochasticdepth101|42.69M|21.28|5.39|60|60|40|40|200|
