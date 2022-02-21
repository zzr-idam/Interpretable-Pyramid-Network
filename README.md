# LapDehazeNet

This is the official code for the paper "Single UHD Image Dehazing via Interpretable Pyramid Network"

Currently, most single image dehazing models cannot run an ultra-high-resolution (UHD) image with a single GPU shader in real-time. To address the problem, we introduce the principle of infinite approximation of Taylor's theorem with the Laplace pyramid pattern to build a model which is capable of handling 4K hazy images in real-time. The N branch networks of the pyramid network correspond to the N constraint terms in Taylor's theorem. Low-order polynomials reconstruct the low-frequency information of the image (e.g. color, illumination). High-order polynomials regress the high-frequency information of the image (e.g. texture). In addition, we propose a Tucker reconstruction-based regularization term that acts on each branch network of the pyramid model. It further constrains the generation of anomalous signals in the feature space. Extensive experimental results demonstrate that our approach can not only run 4K images with haze in real-time on a single GPU (80FPS) but also has unparalleled interpretability. The developed method achieves state-of-the-art (SOTA) performance on two benchmarks (O/I-HAZE) and our updated 4KID dataset while providing the reliable groundwork for subsequent optimization schemes.

## Environment Preparing

```
python 3.7
pytorch 1.7.1
```

### Testing

We provide some example images for testing in `Test/test_imgs/`

```
python test.py
```

### Note:

The `10303.pth` saves the whole model, and relevant documents required have been stored in the `Mou`folder.

## Cite

https://arxiv.org/abs/2202.08589

## Code
address: https://pan.baidu.com/s/1gVuZDE3rIhw9elFmqON6bQ  password:4qsa 
