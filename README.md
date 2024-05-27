*Neural Style Transfer*

This tutorial uses deep learning to compose one image in the style of another image . This is known as neural style transfer and the technique is outlined in A Neural Algorithm of Artistic Style.

Note: This tutorial demonstrates the original style-transfer algorithm. It optimizes the image content to a particular style. Modern approaches train a model to generate the stylized image directly (similar to CycleGAN). This approach is much faster (up to 1000x).

For a simple application of style transfer with a pretrained model from TensorFlow Hub, check out the Fast style transfer for arbitrary styles tutorial that uses an arbitrary image stylization model. For an example of style transfer with TensorFlow Lite, refer to Artistic style transfer with TensorFlow Lite.

Neural style transfer is an optimization technique used to take two images—a content image and a style reference image (such as an artwork by a famous painter)—and blend them together so the output image looks like the content image, but “painted” in the style of the style reference image.

This is implemented by optimizing the output image to match the content statistics of the content image and the style statistics of the style reference image. These statistics are extracted from the images using a convolutional network.
