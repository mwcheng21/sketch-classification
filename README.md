# sketch-classification
Finetuning ImageNet Image Classifiers for Free-hand Sketch Recognition Classification

20 Epoch fine tuning
alexnet     top1:0.6685  top5:0.886
vgg         top1:0.727   top5:0.9105
squeezenet  top1:0.664   top5:0.8765
densenet    top1:0.7515  top5:0.92975
resnet      top1:0.72625 top5:0.91725

15 Epoch fine tuning
alexnet     top1:0.66125 top5:0.874
vgg         top1:0.72875 top5:0.92075
squeezenet  top1:0.6585  top5:0.87
densenet    top1:0.75325 top5:0.93
resnet      top1:0.72875 top5:0.92075


Sketches differ from images in 2 ways. The most obvious way is the lack of color. The other is the slight inacuracies in hand drawn images, such as imperfect proportions, straight lines, and other common features. As a result, sketches are not always classified correctly, as they do not always have the same features.
Some have tried using pretrained imagenet classifiers to classify sketches. However these sketches are usually well drawn sketches by artists, which means typcial features of the image still exist. However, these models are not cognizant of the fact that most people do not have the time or ability to draw such detailed sketches.
These "free hand" sketches have less details, and are resemble the item much less than other artistic scketches.

Sketches can be classified into two categories. Either they are drawn by an artist anc closelt resemble the object, or they are drawn by a lay man and have some resemblence, but with little detail. The latter will be refered to as "free hand" sketches. Free hand sketches contain less detail, and are often misshapen and have obvious deformations, which make it more difficult to recognize for a computer. 