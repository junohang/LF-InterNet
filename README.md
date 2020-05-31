***PyTorch implementation of "Spatial-Angular Interaction for Light Field Image Super-Resolution". arXiv 2019. [<a href="https://arxiv.org/pdf/1912.07849v2.pdf">PDF</a>]*** <br>

## Overview
<img src="https://raw.github.com/YingqianWang/LF-InterNet/master/Figs/Network.jpg" width="600">
***Fig. 1: An overview of our LF-InterNet***<br><br>

<img src="https://raw.github.com/YingqianWang/LF-InterNet/master/Figs/SFEAFE.jpg" width="400"><br>
***Fig. 2: An illustration of angular feature extractor (AFE) and spatial feature extractor (SFE).***<br><br>

## Requirement
* **PyTorch 1.3.0, torchvision 0.4.1. The code is tested with python=3.7, cuda=9.0.**
* **Matlab (For training/test data generation and performance evaluation)**

## Train
Training codes will be released soon.

## Test
* **Download the test sets and unzip them to `./data`. Here, we provide a demo test set (<a href="https://yingqianwang.github.io/homepage/">data_demo.zip</a>) which only includes one test scene, and we also provide the full test set (<a href="https://yingqianwang.github.io/homepage/">data.zip</a>) which is used in our paper.** 
* **Download our pretrained models (<a href="https://yingqianwang.github.io/homepage/">log.zip</a>) and unzip them to `./log`.**
* **Run `GenerateDataForTest.m` to generate test data.**
* **Run `test.py` to perform a demo inference. Note that, the selected pretrained model should match the generated input data and the preset network architecture. Initial results (`.mat` files) will be saved to `./results`.**
* **Run `evaluation.m` to calculate PSNR and SSIM scores and transform initial results (`.mat` files) into `.png` images.**

## Quantitative Results
<img src="https://raw.github.com/YingqianWang/LF-InterNet/master/Figs/Quantitative.jpg" width="800"><br>
<br>
## Qualitative Results
<img src="https://raw.github.com/YingqianWang/LF-InterNet/master/Figs/Qualitative.jpg" width="800"><br>

## Efficiency
<img src="https://raw.github.com/YingqianWang/LF-InterNet/master/Figs/Efficiency.jpg" width="800"><br>

## Performance w.r.t. Perspectives
<img src="https://raw.github.com/YingqianWang/LF-InterNet/master/Figs/PwrtP.jpg" width="800"><br>

## Performance Under Real-World Degradation
<img src="https://raw.github.com/YingqianWang/LF-InterNet/master/Figs/VisualReal.jpg" width="800"><br>

## Citiation
```
@article{LF-InterNet,<br>
  title={Spatial-Angular Interaction for Light Field Image Super-Resolution},<br>
  author={Wang, Yingqian and Wang, Longguang and Yang, Jungang and An, Wei and Yu, Jingyi and Guo, Yulan},<br>
  journal={arXiv preprint arXiv:1912.07849},<br>
  year={2019}<br>
}<br>
```

## Contact
**Please contact *Yingqian Wang* (wangyingqian16@nudt.edu.cn) for any question about this work.**
