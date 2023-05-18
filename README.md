# Adv. Comp. Vision & Pattern Recognition (2022-2B)

### VGG16 Attention Test

Currently only contains a vgg16 test notebook (see [attention.ipynb](vgg16_attention_test/attention.ipynb)).

This notebook takes the pretrained vgg16 CNN, runs each layer sequentially on an image, and then displays the output of each layer.

Most layers output a 3D tensor (width, height, channels), where channels is usually 64. To be able visualize this, we can take the mean of the channels to get a 2D tensor (width, height),
and diplay this as a heatmap.

The final few layers are single dimensional tensors, which we can display as a bar graph.

At the end, we then make a prediction on the image, and display the top 5 predictions. This is a sanity check to verify the network is actually predicting something meaningful.
