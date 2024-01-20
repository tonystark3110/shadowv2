Shadow removal is an essential task for scene understanding. Many studies consider only matching the image contents, which often causes two types of ghosts: color in-consistencies in shadow regions or artifacts on shadow boundaries. In this paper, we tackle these issues in two ways. First, to carefully learn the border artifacts-free image, we propose a novel network structure named the dual hierarchically aggregation network~(DHAN). It contains a series of growth dilated convolutions as the backbone without any down-samplings, and we hierarchically aggregate multi-context features for attention and prediction, respectively. Second, we argue that training on a limited dataset restricts the textural understanding of the network, which leads to the shadow region color in-consistencies. Currently, the largest dataset contains 2k+ shadow/shadow-free image pairs. However, it has only 0.1k+ unique scenes since many samples share exactly the same background with different shadow positions. Thus, we design a shadow matting generative adversarial network~(SMGAN) to synthesize realistic shadow mattings from a given shadow mask and shadow-free image. With the help of novel masks or scenes, we enhance the current datasets using synthesized shadow images. Experiments show that our DHAN can erase the shadows and produce high-quality ghost-free images. After training on the synthesized and real datasets, our network outperforms other state-of-the-art methods by a large margin.
