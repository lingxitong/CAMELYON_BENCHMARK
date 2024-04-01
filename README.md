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
* ***MHIM_MIL*** [MIL Framework with Masked Hard Instance Mining for WSI Classification](https://arxiv.org/abs/2307.15254) ***(ICCV 2023)***
* ***IB_MIL*** [Interventional Bag Multi-Instance Learning On Whole-Slide Pathological Images](https://arxiv.org/abs/2303.06873) ***(CVPR 2023)***
* ***RTT_MIL*** [Towards Foundation Model-Level Performance in Computational Pathology](https://arxiv.org/abs/2402.17228) ***(CVPR 2024)***
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

  
## RESULTS(4 classes)
Benchmark test of different ***MIL*** methods
### *vit_s-benchmark*

<table>
  <tr>
    <th>MIL</th>
    <th>PARAMS</th>
    <th>ACC</th>
    <th>B-ACC</th>
    <th>AUC</th>
    <th>PRE</th>
    <th>RECALL</th>
    <th>F1</th>
    <th colspan="6">DOWNLOAD</th>
  </tr>
  <tr>
    <td>MEAN</td>
    <td style="text-align: center;">&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>MAX</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>RNN</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>AB</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>GATE_AB</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>TRANS</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>DS</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>CLAM</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>WENO</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>DTFD</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    </tr>
    <tr>
    <td>IB</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    </tr>
    <tr>
    <td>MHIM</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    </tr>
    <tr>
    <td>RTT</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    </tr>
    <tr>
    <td>WIKG</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
<table>


### ***pilp-benchmark***
<table>
  <tr>
    <th>MIL</th>
    <th>PARAMS</th>
    <th>ACC</th>
    <th>B-ACC</th>
    <th>AUC</th>
    <th>RECALL</th>
    <th>F1</th>
    <th colspan="6">DOWNLOAD</th>
  </tr>
  <tr>
    <td>MEAN</td>
    <td style="text-align: center;">&nbsp;&nbsp;&nbsp;00M</td>
    <td>81.95%</td>
    <td>73.37%</td>
    <td>76.70%</td>
    <td>73.37%</td>
    <td>67.23%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>MAX</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>70.81%</td>
    <td>77.26%</td>
    <td>77.48%</td>
    <td>77.26%</td>
    <td>64.30%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>TRANS</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>74.44%</td>
    <td>83.20%</td>
    <td>85.40%</td>
    <td>83.20%</td>
    <td>68.38%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>AB</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>83.28%</td>
    <td>82.76%</td>
    <td>84.88%</td>
    <td>82.76%</td>
    <td>72.19%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>DS</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>CLAM</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>WENO</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>DTFD</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    </tr>
    <tr>
    <td>IB</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    </tr>
    <tr>
    <td>MHIM</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    </tr>
    <tr>
    <td>RTT</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    </tr>
    <tr>
    <td>WIKG</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>88.50%</td>
    <td>84.00%</td>
    <td>86.50%</td>
    <td>84.00%</td>
    <td>75.67%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
<table>



### ***uni-benchmark***
<table>
  <tr>
    <th>MIL</th>
    <th>PARAMS</th>
    <th>ACC</th>
    <th>B-ACC</th>
    <th>AUC</th>
    <th>RECALL</th>
    <th>F1</th>
    <th colspan="6">DOWNLOAD</th>
  </tr>
  <tr>
    <td>MEAN</td>
    <td style="text-align: center;">&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>MAX</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>AB</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>TRANS</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>DS</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>CLAM</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>WENO</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    <tr>
    <td>DTFD</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    </tr>
    <tr>
    <td>IB</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    </tr>
    <tr>
    <td>MHIM</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    </tr>
    <tr>
    <td>RTT</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
    </tr>
    <tr>
    <td>WIKG</td>
    <td>&nbsp;&nbsp;&nbsp;00M</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td>0.00%</td>
    <td><a href="https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md">&nbsp;pre-trained</a></td>
  </tr>
<table>







  
 
