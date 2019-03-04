# Single Image Super-Resolution (RGB vs HSV)

## Abstract
*abstract text*

## Related Works
### [SRResNet](https://arxiv.org/abs/1609.04802)
* first deep ResNet for SISR
* post-upscaling > pre-upscaling

### [EDSR](https://arxiv.org/abs/1707.02921)
* using ResBlocks && removing batch-normalization
* increasing features > increasing depth
* residual scaling (x0.1)
* L1-loss (MAE) > L2-loss (MSE)
* geometric self-ensemble
* multi-scale model

### [WDSR](https://arxiv.org/abs/1808.08718)
* "wide" activation (expand features before ReLU)
* weight normalization instead BN
* global residual pathway + upsampling layer

## Contribution
* SISR implementation training by HSV image representation
* Comparison of RGB and HSV results

## Getting Started
* Training dataset: [DIV2K](https://data.vision.ee.ethz.ch/cvl/DIV2K/)
* Framework: [TensorFlow](https://www.tensorflow.org/)
* Hardware: [Google Colab](https://colab.research.google.com)

## Architecture
![EDSR](https://raw.githubusercontent.com/mkhlmnkn/SuperRes-RGB-vs-HSV/master/images/for%20readme/edsr%20arch%20.png)

## Benchmark Results
### DIV2K 0809
![0809](https://raw.githubusercontent.com/mkhlmnkn/SuperRes-RGB-vs-HSV/master/images/for%20readme/0809.png)
### DIV2K 0841
![0841](https://raw.githubusercontent.com/mkhlmnkn/SuperRes-RGB-vs-HSV/master/images/for%20readme/0841.png)
### DIV2K 0853
![0853](https://raw.githubusercontent.com/mkhlmnkn/SuperRes-RGB-vs-HSV/master/images/for%20readme/0853.png)

## Conclusion
It seems that RGB is better than HSV.\
N.B. The lion is the best in any case.
