# encoder4editing with MobileNetV3
  <img src="https://img.shields.io/badge/python-3-green"></a>
  <img src="https://img.shields.io/badge/pytorch-1.9-yellowgreen"></a>
  <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-yellow.svg"></a>
  <a href="https://github.com/omertov/encoder4editing"><img src="https://img.shields.io/badge/reference-e4e-yellowgreen"></a>


<p align="center">
<img src="sample/e4e_mobile_1024p.png" width="800px"/>
<br>
The demo of different styles images of e4e-mbv3 framework.</p>

## Description  

Re-implementation of e4e that use mobilenet-v3 and stylegan2-1024p. Then mix different styles by stylegan2 and convert to openvino.

## Citation

This code is heavily based on [encoder4editing](https://github.com/omertov/encoder4editing) and [stylegan2-pytorch](https://github.com/rosinality/stylegan2-pytorch). Thanks `omertov` and `rosinality` so much to make his work available 🙏🙏🙏 

## Pretrained Models

链接: https://pan.baidu.com/s/1JlJTyBmFLZhju4MpDHLdAA  密码: 086q

[Google Drive](https://drive.google.com/file/d/18zK4A_iM6v8wHQAxd9_dmqGxLg3Z3Oyh/view?usp=share_link)

## Training Log
### Tensorboard

<p align="center">
<img src="sample/train_log1.png" width="800px"/>
<img src="sample/train_log2.png" width="800px"/>
<br>
The loss of training.</p>

## Test
``` 
python scripts/inference.py \
--images_dir=./test_images/ \
--save_dir=./sample \
./ckpt/best_model.pt
```

## More
[Inference on openvino and more demo](https://github.com/TalkUHulk/realworld-stylegan2-encoder)



