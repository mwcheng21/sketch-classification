# sketch-classification
Finetuning ImageNet Image Classifiers for Free-hand Sketch Recognition Classification
CURRENTLY IN PROGRESS


20 Epoch fine tuning
| Model type | top-1  | top-5  |
|------------|---|---|
| alexnet    | 0.659  | 0.8805  |
| vgg        | 0.72425  | 0.909   |
| squeezenet | 0.6595  | 0.87925  |
| densenet   | 0.75175  | 0.93375  |
| resnet     | 0.735  | 0.923  |


15 Epoch fine tuning
| Model type | top-1  | top-5  |
|------------|---|---|
| alexnet    | 0.66125  | 0.874  |
| vgg        | 0.7215  | 0.909   |
| squeezenet | 0.6585  | 0.87  |
| densenet   | 0.75325  | 0.93  |
| resnet     | 0.72875  | 0.92075  |


Vanilla models - no fine tuning
| Model type | top-1  | top-5  |
|------------|---|---|
| alexnet    | 0.005  | 0.02375  |
| vgg        | 0.00425  | 0.022   |
| squeezenet | 0.0055  | 0.026  |
| densenet   | 0.0025  | 0.02325  |
| resnet     | 0.00425  | 0.02275  |
*Note how densenet top-1 is twice as good as all other methods

Sketches differ from images in 2 ways. The most obvious way is the lack of color. The other is the slight inacuracies in hand drawn images, such as imperfect proportions, straight lines, and other common features. As a result, sketches are not always classified correctly, as they do not always have the same features.
Some have tried using pretrained imagenet classifiers to classify sketches. However these sketches are usually well drawn sketches by artists, which means typcial features of the image still exist. However, these models are not cognizant of the fact that most people do not have the time or ability to draw such detailed sketches.
These "free hand" sketches have less details, and are resemble the item much less than other artistic scketches.

Sketches can be classified into two categories. Either they are drawn by an artist anc closelt resemble the object, or they are drawn by a lay man and have some resemblence, but with little detail. The latter will be refered to as "free hand" sketches. Free hand sketches contain less detail, and are often misshapen and have obvious deformations, which make it more difficult to recognize for a computer. 