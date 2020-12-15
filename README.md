# sketch-classification
Finetuning ImageNet Image Classifiers for Free-hand Sketch Recognition Classification
CURRENTLY IN PROGRESS


20 Epoch fine tuning
| Model type | top-1  | top-5  |
|------------|---|---|
| alexnet    | 0.659  | 0.8805 |
| vgg        | 0.72425| 0.909  |
| squeezenet | 0.6595 | 0.87925|
| densenet   | 0.75175| 0.93375|
| resnet     | 0.735  | 0.923  |
| googlenet  | 0.7175 | 0.91875|
| mobilenet  | 0.729  | 0.91475|
| shufflenet | 0.168  | 0.392  |
| resnext    | 0.7555 | 0.94   |
| mnasnet    | 0.7205 | 0.92075|
| wideresnet | 0.76525| 0.93525|


15 Epoch fine tuning
| Model type | top-1  | top-5  |
|------------|---|---|
| alexnet    | 0.66125  | 0.874  |
| vgg        | 0.7215  | 0.909   |
| squeezenet | 0.6585  | 0.87  |
| densenet   | 0.75325  | 0.93  |
| resnet     | 0.72875  | 0.92075  |
| googlenet     | 0.6775  | 0.87825  |


Vanilla models - no fine tuning
| Model type | top-1  | top-5  |
|------------|---|---|
| alexnet    | 0.005  | 0.02375  |
| vgg        | 0.00425  | 0.022   |
| squeezenet | 0.0055  | 0.026  |
| densenet   | 0.0025  | 0.02325  |
| resnet     | 0.00425  | 0.02275  |
| googlenet     | 0.00025  | 0.00075  |


**Note how densenet top-1 is twice as good as all other methods
