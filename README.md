# Awesome Data-Efficient Deep Learning Papers 

<a href="#1">Semi-supervised Learning</a>

<a href="#2">Few-shot Learning</a>

<a href="#3">Data Augmentation</a>

<a name="1"></a>
## Semi-supervised Learning 
-  [**Semi-supervised Learning with a Teacher-student Network for Generalized Attribute Prediction**](https://arxiv.org/abs/2007.09162) (ECCV2020)

    **Abstract :** This paper presents a study on semi-supervised learning to solve the visual attribute prediction problem. In many applications of vision algorithms, the precise recognition of visual attributes of objects is important but still challenging. This is because defining a class hierarchy of attributes is ambiguous, so training data inevitably suffer from class imbalance and label sparsity, leading to a lack of effective annotations. An intuitive solution is to find a method to effectively learn image representations by utilizing unlabeled images. With that in mind, we propose a multi-teacher-single-student (MTSS) approach inspired b`````y the multi-task learning and the distillation of semi-supervised learning. Our MTSS learns task-specific domain experts called teacher networks using the label embedding technique and learns a unified model called a student network by forcing a model to mimic the distributions learned by domain experts. Our experiments demonstrate that our method not only achieves competitive performance on various benchmarks for fashion attribute prediction, but also improves robustness and cross-domain adaptability for unseen domains.
-  [**Improving Object Detection with Selective Self-supervised Self-training**](https://arxiv.org/abs/2007.06769) (ECCV2020)

    **Abstract :** We study how to leverage Web images to augment human-curated object detection datasets. Our approach is two-pronged. On the one hand, we retrieve Web images by image-to-image search, which incurs less domain shift from the curated data than other search methods. The Web images are diverse, supplying a wide variety of object poses, appearances, their interactions with the context, etc. On the other hand, we propose a novel learning method motivated by two parallel lines of work that explore unlabeled data for image classification: self-training and self-supervised learning. They fail to improve object detectors in their vanilla forms due to the domain gap between the Web images and curated datasets. To tackle this challenge, we propose a selective net to rectify the supervision signals in Web images. It not only identifies positive bounding boxes but also creates a safe zone for mining hard negative boxes. We report state-of-the-art results on detecting backpacks and chairs from everyday scenes, along with other challenging object classes.

<a name="2"></a>
## Few-shot Learning

-  [**Impact of base dataset design on few-shot image classification**](https://arxiv.org/abs/2007.08872) (ECCV2020)

    **Abstract :** The quality and generality of deep image features is crucially determined by the data they have been trained on, but little is known about this often overlooked effect. In this paper, we systematically study the effect of variations in the training data by evaluating deep features trained on different image sets in a few-shot classification setting. The experimental protocol we define allows to explore key practical questions. What is the influence of the similarity between base and test classes? Given a fixed annotation budget, what is the optimal trade-off between the number of images per class and the number of classes? Given a fixed dataset, can features be improved by splitting or combining different classes? Should simple or diverse classes be annotated? In a wide range of experiments, we provide clear answers to these questions on the miniImageNet, ImageNet and CUB-200 benchmarks. We also show how the base dataset design can improve performance in few-shot classification more drastically than replacing a simple baseline by an advanced state of the art algorithm.

<a name="3"></a>
## Data Augmentation


-  [**OnlineAugment: Online Data Augmentation with Less Domain Knowledge**](https://arxiv.org/abs/2007.09271) (ECCV2020)

    **Abstract :** Data augmentation is one of the most important tools in training modern deep neural networks. Recently, great advances have been made in searching for optimal augmentation policies in the image classification domain. However, two key points related to data augmentation remain uncovered by the current methods. First is that most if not all modern augmentation search methods are offline and learning policies are isolated from their usage. The learned policies are mostly constant throughout the training process and are not adapted to the current training model state. Second, the policies rely on class-preserving image processing functions. Hence applying current offline methods to new tasks may require domain knowledge to specify such kind of operations. In this work, we offer an orthogonal online data augmentation scheme together with three new augmentation networks, co-trained with the target learning task. It is both more efficient, in the sense that it does not require expensive offline training when entering a new domain, and more adaptive as it adapts to the learner state. Our augmentation networks require less domain knowledge and are easily applicable to new tasks. Extensive experiments demonstrate that the proposed scheme alone performs on par with the state-of-the-art offline data augmentation methods, as well as improving upon the state-of-the-art in combination with those methods.
