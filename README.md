# Comparing the performance of different neural networks to classify low surface brightness galaxies.

In the last years, innovative works, fueled by robust sky surveys and efficient
methods of detection, rekindled the interest of the scientific community for Low
Surface Brightness Galaxies, a peculiar class of galaxies with low superficial stellar
density that are very faint and diffuse in optical images.
If the automatic detection of these galaxies in photometric surveys is already a
complicated task, given their low surface brightness, searches for these objects suffer an aditional problem: the enormous amount of artifacts that are detected in the

images and also have low surface brightness. With the growing amount of astrono-
mical data, visual inspection to reject detected artifacts becomes impratical and it is

necessary to develop efficient methods to separate Low Surface Brightness Galaxies
from artifacts. Deep Learning methods, like Convolutional Neural Networks, are
considered the state-of-the-art in several image classification problems.
In this work, we aim at comparing the performance of the Visual Tranformers
network, which recently caused a huge impact in the literature for challenging the
paradigm of the state-of-the-art, with Convolutional Neural Networks to identify
Low Surface Brightness Galaxies. To do that, we implemented a Visual Transformers
Network and compared it with the DeepShadows Network, a Convolutional Neural
Network developed by Tanoglidis et al. (2021b). Both networks were trained using
the only image set of these objects publicly avaliable, composed of 40000 images
from the Dark Energy Survey. We verified that our model achieved slightly superior
metrics in comparison with DeepShadows. Between those, when trained on the
dataset using the PNG format, the standard model of our network achieved an
accuracy = 0.929, which is 0.98% higher than the one of DeepShadows. However,
when computing the uncertainties on the metrics of our method using the bootstrap
method, we have noticied that the performance of our network was as good as the
one obtained by DeepShadows when considering de 95% confidence interval of the
metrics. Besides that, using images of the same dataset, but in the FITS format, we
implemented a method to pre-processes the input data, which aims to improve the
performance of the networks. This method consists of doing a contrast adjusment
to highlight low surface brightness objects in the images. We noticed that the
contrast adjustment contribuited both to the ViT standard model and DeepShadows
to achieve a higher performance. However, the best training result with the FITS
image set did not overcome the results of both networks when applied to the PNG
dataset. Like Dosovitskiy et al. (2021) showed, with the increase of the datasets,
the Visual Tranformers Networks can overcome the performance of Convolutional
Neural Networks, therefore that seems to be an specially interesting paradigm to
Vision Transformers.

Thesis (in protuguese) avaliable at https://drive.google.com/file/d/1-8ufORBAZ1wq8IUS_H35kHiGg_cutbaK/view?usp=sharing

Any doubts, please wrtite to manuel.stveras@gmail.com
