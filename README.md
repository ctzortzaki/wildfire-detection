Detecting wildfires quickly and accurately is important to help stop them from spreading and causing damage
to the environment, wildlife, and people. Traditional methods like watching from towers or using satellite
images can be slow, limited in coverage, or require constant human attention. In contrast, deep learning
models can automatically look at images from drones, ground cameras, or satellites and detect signs of fire
or smoke in real time.

However, wildfire detection is not easy. Fire and smoke can look very different depending on the light-
ing, weather, background, and camera quality. For example, a sunset or fog can look like a fire, which can
confuse the model. This makes it hard for even advanced computer vision systems to always get it right.
In the past, researchers used simple features like color and edges along with basic machine learning models.
These worked okay in simple cases. Later, deep learning models like ResNet and EfficientNet performed
much better. More recently, Vision Transformers (ViTs) have shown strong results by understanding the
overall image better. Still, many models don’t do well when they are trained on small datasets or when they
face unfamiliar scenes.

In this project, we test and compare several deep learning models for wildfire detection using a small public
dataset. Our main contributions are:

• We compare a ResNet-18 model trained from scratch with one that is pretrained on a larger
dataset (ImageNet) and fine-tuned for wildfire detection.

• We also use a Vision Transformer (ViT) model to see how well it can detect fires in complex images.

• To deal with the small dataset, we use data augmentation—both common image changes (like
flipping and color adjustment) and synthetic image generation using a diffusion model to create
fake fire images.

Our goal is to find out which models and methods work best for this problem when data is limited and the
scenes are complex. By improving the training data and using smart model settings, we aim to build better
systems for detecting wildfires in real-world situations.
