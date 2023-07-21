# *ART generation using speech emotions*
Translation of speech to image directly without text is an interesting and useful topic due to the potential application in computer-aided design, human to computer interaction, creation of an art form, etc. So we have focused on developing Deep learning and GANs based model which will take speech as an input from the user, analyze the emotions associated with it and accordingly generate the artwork which has been demanded by the user which will in turn provide a personalized experience. 

The approach used here is convolutional VQGAN to learn a codebook of context-rich visual parts, whose composition is subsequently modeled with autoregressive transformer architecture. Concept of CLIP-Contrastive Language Image-Pre-Training, also uses transformers which is a model trained to determine which caption from a set of captions best fits with a given image is used in our project. 

The input speech is classified into 8 different emotions using MLP classifier trained of RAVDESS emotional speech audio dataset and this acts as a base filter for the VQGAN model. Text converted from speech plays an important role in producing the final output image using CLIP model. VQGAN+CLIP model together utilizes both emotions and text to generate a more personalized artwork.

