# Indoor-and-outdoor-scene-recognition-using-VGG-and-Resnet

Visually disabled people have their own style of doing things and lives an
ordinary life with. But due to inaccessible infrastructure and social challenges
they definitely face troubles. To navigate around places is the biggest challenge
for a blind person, especially the one with complete loss of vision. They know
the position of everything in the house therefore they can easily roam in their
house without any help. But they have difficulty in recognizing scenes when they
are in other places. So, we decided to make an indoor and outdoor scene

5

recognition System. We are interested in this project after we went through few
papers in this area. As a result, we are highly motivated to develop a system that
recognizes the scene in the real-time environment.

Scene recognition is still a developing area in computer vision there are multiple
applications of scene recognition. Due to so much variability in the environment,
this becomes quite difficult to recognize the background scene of the image. Still,
we have so much more to explore in this area, as data is generated day by day at
a rapid rate it becomes important to recognizing and understand the features in
that data. Several recognition techniques work well with image data, but in the
case of scene recognition, it is not giving promising results due to less variability.



For training the model we will be using CNN which will produce audio output by
converting an input image into a string of text and text to audio. And due to lack
of integrated framework or portable device which can help in understanding and
recognizing visual scene for visually impaired people. And to address the
problem of the indoor scene the model exploits local and global discriminative
information. This model will work as a navigator or assistance system which will
help people with partial blindness or fully visually impaired to navigate indoor
scenes.
• To help navigate in an indoor place for people with partial or full visual
impairment the system will work as an assistive system to help them
recognize the surrounding.

• For addressing the problem of indoor scene recognition, this model will
exploit the local as well as global discriminative information.



## Dataset
The dataset that we have used is the MIT indoor scene database with sixty-seven
indoor scene classes with 15620 images containing kitchen, airport, gym, etc. The
images in the indoor scene dataset vary throughout classes, however, in every
class there are around a hundred images. All images are in the format of JPG. In
high-level vision, indoor scene recognition is a difficult problem. Most models
and algorithms of scene recognition perform poorly in the indoor scene domain
that display the best performance in the case of outdoor scenes. This problem
happens because when we classify some indoor scenes like corridors it will
become easier to classify them due to their global properties, while other scenes
like a bookstore can be better classified for the objects they contain.



## Transfer learning
This preliminary segment introduces the models and algorithms used in this
project. For implementation, we used the transfer learning technique. So far, the
algorithms traditionally designed for machine learning and deep learning
techniques are work in isolation. For resolving particular tasks these algorithms
are trained. The models are rebuilt from scratch once the feature-space
distribution changes.

Transfer learning is the concept of making use of knowledge obtained for one
task to resolve associated ones and to overcoming the isolated learning paradigm.
Transfer learning isn't a new idea, this is very particular to deep learning. The
conventional techniques of training and building a machine learning models is
different from using transfer learning principle following method.

Traditional learning is remoted and takes place simply based totally on particular
on training separate model on dataset and tasks. There will be no knowledge
present which used from one model and transferred to another. In transfer
learning, for training the latest models we can reuse information from previously
trained models.

To resolve the issue of computer vision domain, where features like shape, edge,
corners and intensity which are low-level features are shared all through tasks, to
resolving this permit transfer of knowledge among tasks. As we've discussed,
knowledge from a present task will acts as a further input while learning a new
aim task. There are three types of transfer models.
• Train the whole model whilst the dataset is large but isn't the same as the
pre-trained version’s dataset.

• Train a few and leave other frozen when the dataset is massive similar to
dataset of pretrained model or when we have small dataset different from
the pre-trained dataset.
Lastly, keep the full model freeze feed the dense layer according to the
classifier wherein we've got the small dataset that is same as pre-trained
dataset.

We are only training some layers and leave others frozen where
the subsampling triple layer which is extremely complex and having millions of
parameters and extracts features, is left alone at the value obtained during the
pretraining. While the parameters of fully connected layers are modified by the
use of a small set of new images. Transfer learning is modifying just a few layers
of the model, so it is going to take less time as compared to training all the layers,
and it may be accelerated by a GPU. It enables fine-tuning a pre-existing model
to work for tasks that do not have a lot of data available.

Pretrained models are used in transfer learning techniques the choice of using the
pre-trained model relies upon the size of the datasetand the number of
computational resources available. These models include
• Fine-tuning in this the final classifier layer of a network is swapped out and
replaced with a SoftMax layer the right size to fit the current dataset while
keeping the learned parameters of all other layers.

• Freezing for smaller dataset it is common to freeze some first layers of the
network, meaning the parameters of the pre-trained network are not
modified in these layers. The other layers are trained on the new task as
before.

• Feature extraction is the loosest usage of pre-trained networks.
