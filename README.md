# RankIQA:Learning from Rankings for No-reference Image Quality assessment
The paper will appear in ICCV 2017. The code and model will be undated later.

## Authors

Xialei Liu, Joost van de Weijer and Andrew D. Bagdanov

## Institutions

[Computer Vision Center, Barcelona, Spain](http://www.cvc.uab.es/lamp/)

Media Integration and Communication Center, University of Florence, Florence, Italy

## Abstract

We propose a no-reference image quality assessment
  (NR-IQA) approach that learns from rankings 
  (RankIQA). To address the problem of limited IQA dataset size, we
  train a Siamese Network to rank images in terms of image quality by
  using synthetically generated distortions for which relative image
  quality is known. These ranked image sets can be automatically
  generated without laborious human labeling. We then use
  fine-tuning to transfer the knowledge represented in the trained
  Siamese Network to a traditional CNN that estimates absolute image
  quality from single images. We demonstrate how our approach can be
  made significantly more efficient than traditional Siamese Networks
  by forward propagating a batch of images through a single network
  and backpropagating gradients derived from all pairs of images in
  the batch. Experiments on the TID2013 benchmark show that we improve the state-of-the-art by over 5%. Furthermore, on the LIVE benchmark we show that our approach is superior to existing NR-IQA techniques and that we even outperform the state-of-the-art in full-reference IQA (FR-IQA) methods without having to resort to high-quality reference images to infer IQA.

## Models

The main idea our approach to address the problem of limited IQA dataset size in order to train a deep CNN.

![Our_approach]
[Our_approach]: https://github.com/xialeiliu/RankIQA/tree/master/figs/models.png

## Results

We have reported experimental results on different IQA datasets including TID2013, LIVE, CSIQ, MLIVE.

## Framework

All training and testing are done in Caffe framework.

## Citation

Please cite our paper if you are inspired by the idea.
