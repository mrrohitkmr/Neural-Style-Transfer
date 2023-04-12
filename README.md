# Neural Style Transfer

This repository contains a simple implementation of neural style transfer using TensorFlow. Neural style transfer is a technique that uses a neural network to apply the style of one image to the content of another image.


### What is NST algorithm?
The algorithm transfers style from one input image (the style image) onto another input image (the content image) using CNN nets (usually VGG-16/19) and gives a composite, stylized image out which keeps the content from the content image but takes the style from the style image.

<p align="center">
<img src="data/examples/bridge/green_bridge_vg_la_cafe_o_lbfgs_i_content_h_500_m_vgg19_cw_100000.0_sw_30000.0_tv_1.0.jpg" width="570"/>
<img src="data/examples/bridge/content_style.jpg" width="260"/>
</p>

### Why yet another NST repo?
It's the **cleanest and most concise** NST repo that I know of + it's written in **PyTorch!** :heart:

Most of NST repos were written in TensorFlow (before it even had L-BFGS optimizer) and torch (obsolete framework, used Lua) and are overly complicated often times including multiple functionalities (video, static image, color transfer, etc.) in 1 repo and exposing 100 parameters over command-line (out of which maybe 5 or 6 may actually be used on a regular basis).

## Examples

Transfering style gives beautiful artistic results:

<p align="center">
<img src="data/examples/bridge/green_bridge_vg_starry_night_o_lbfgs_i_content_h_500_m_vgg19_cw_100000.0_sw_30000.0_tv_1.0_resized.jpg" width="270px">
<img src="data/examples/bridge/green_bridge_edtaonisl_o_lbfgs_i_content_h_500_m_vgg19_cw_100000.0_sw_30000.0_tv_1.0_resized.jpg" width="270px">
<img src="data/examples/bridge/green_bridge_wave_crop_o_lbfgs_i_content_h_500_m_vgg19_cw_100000.0_sw_30000.0_tv_1.0_resized.jpg" width="270px">

<img src="data/examples/lion/lion_candy_o_lbfgs_i_content_h_500_m_vgg19_cw_100000.0_sw_30000.0_tv_1.0_resized.jpg" width="270px">
<img src="data/examples/lion/lion_edtaonisl_o_lbfgs_i_content_h_500_m_vgg19_cw_100000.0_sw_30000.0_tv_1.0_resized.jpg" width="270px">
<img src="data/examples/lion/lion_vg_la_cafe_o_lbfgs_i_content_h_500_m_vgg19_cw_100000.0_sw_30000.0_tv_1.0_resized.jpg" width="270px">
</p>

And here are some results coupled with their style:

<p align="center">
<img src="data/examples/figures/figures_ben_giles_o_lbfgs_i_content_h_500_m_vgg19_cw_100000.0_sw_30000.0_tv_1.0_resized.jpg" width="400px">
<img src="data/style-images/ben_giles.jpg" width="267px">

<img src="data/examples/figures/figures_wave_crop_o_lbfgs_i_content_h_500_m_vgg19_cw_100000.0_sw_30000.0_tv_1.0_resized.jpg" width="400px">
<img src="data/style-images/wave_crop.jpg" width="267px">

<img src="data/examples/figures/figures_vg_wheat_field_w_350_m_vgg19_cw_100000.0_sw_300000.0_tv_1.0_resized.jpg" width="400px">
<img src="data/style-images/vg_wheat_field_cropped.jpg" width="267px">

<img src="data/examples/figures/figures_vg_starry_night_w_350_m_vgg19_cw_100000.0_sw_30000.0_tv_1.0_resized.jpg" width="400px">
<img src="data/style-images/vg_starry_night_resized.jpg" width="267px">
</p>

*Note: all of the stylized images were produced by me (using this repo), credits for original image artists [are given bellow](#acknowledgements).*

# Acknowledgments
This implementation is based on the following papers:

A Neural Algorithm of Artistic Style, Gatys et al. (2015)
Perceptual Losses for Real-Time Style Transfer and Super-Resolution, Johnson et al. (2016)

## Connect with me

If you'd love to have some more AI-related content in your life :nerd_face:, consider:
* Follow me on [LinkedIn](https://www.linkedin.com/in/rohitkumar-ml/)  :bulb:
*  :books: :heart:

## Licence

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/gordicaleksa/pytorch-neural-style-transfer/blob/master/LICENCE)
