# CatPictureCaptioning

This is the github repository for our group's submission for COMP 646, Spring 2022. 

Members: Ayush Sachdeva, Akash Karanam, Nathan Powell. 

Summary: 
Image captioning is one of the core tasks at the intersection of Computer Vision and Natural Language Processing. The standard deep learning approach for this task is to pass an image through a trained Convolutional Neural Network (CNN) to extract a feature matrix and then hand off this feature matrix to a recurrent neural network (RNN) to generate a sequence of words that form the caption. However, the task of social media image captioning is far more nuanced since a functional model needs to understand the cultural context, sarcasm, and hyperbole in addition to the visual and semantic elements in the image. Furthermore, the grammar and syntax of social media captions differ from ordinary captions because social media captions try to elicit a response from the reader while ordinary captions are more objective and thus use a more consistent grammatical structure. To encapsulate this grammar, we finetune the T5 text encoder on social media captions and prompt it with keywords given by the users and those generated from a resnet-50 backbone feature extractor/encoder with a subsequent text decoder. Due to limited computational resources, we limit the dataset to only captions for an integral yet possibly holistic section of social media, cat pictures. 

Training data: Redcaps Dataset (https://redcaps.xyz/)
