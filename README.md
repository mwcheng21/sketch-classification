# Finetuning pretrained ImageNet Image Classifiers for Free-hand Sketch Recognition

We fine-tuned eleven different types of pretrained ImageNet models for sketch recognition. We show that some recent deep neural network architectures trained on natural images can be better than some architectures that are specifically designed for sketch recognition. We also propose that the commonly used AlexNet performs sub optimally on sketch recognition, and that residual networks are a better alternative. Using the TU-Berlin benchmark we were able to achieve a top-1 accuracy of 77.7% and top-5 accuracy of 94.5% with the ResNeXt architecture.

# Contents
* [Paper](https://github.com/mwcheng21/sketch-classification#paper)
* [Results](https://github.com/mwcheng21/sketch-classification#results)
* [Models](https://github.com/mwcheng21/sketch-classification#models)
* [Dataset](https://github.com/mwcheng21/sketch-classification#dataset)


## Paper
For detailed information see paper [here](https://github.com/mwcheng21/sketch-classification/blob/main/FreehandSketchClassification.pdf)

## Results

For information on each model, see [here](https://pytorch.org/docs/stable/torchvision/models.html)

| Model type | top-1  | top-5  |
|------------|---|---|
|[AlexNet](https://drive.google.com/file/d/1-S2glVkseE-GCd9fjeeCxbys71i1HqFh/view?usp=sharing)       |0.659    |0.8805|
|[SqueezeNet](https://drive.google.com/file/d/1-vaCEBBqCPO6dSrOJawdXAViK-UmXFWP/view?usp=sharing)    |0.6595   |0.87925|
|[VGG-11_(batch norm)](https://drive.google.com/file/d/1-cCo9FNSL3EUPIJEPV-RDyl-QLHzE5Gm/view?usp=sharing)         |0.72425  |0.909|
|[VGG-11](https://drive.google.com/file/d/1-6WvcroMJXcBP1KUHVOGzLkiUnyo8tCD/view?usp=sharing) |0.69725  |0.89175|
|[VGG-19_(batch norm)](https://drive.google.com/file/d/1hsQV2zqyPxzuXxi1GwfC9kjMMAItdOfK/view?usp=sharing)         |0.73825  |0.924|
|[VGG-19](https://drive.google.com/file/d/1NQ9Nsgu96qSjBYW-lzTIW1U7yMMRoy0N/view?usp=sharing) |0.721  |0.9055|
|[ShuffleNet](https://drive.google.com/file/d/1-CBr2qc8xHAqtYuXKnEKrKOe6JySiQyx/view?usp=sharing)    |0.168    |0.392|
|[MobileNet](https://drive.google.com/file/d/1weqhBx0Rs4b7rfOQI8G9gHm8crBp1b3Y/view?usp=sharing)     |0.729    |0.91475|
|[MNASNet](https://drive.google.com/file/d/106PacomRKaiy8k47iOFUmsPlGekmFQ39/view?usp=sharing)       |0.7205   |0.92075|
|[GoogLeNet](https://drive.google.com/file/d/10S2v3TkP_9dHh-dXrO7uNj5f0nXZSpmT/view?usp=sharing)     |0.7175   |0.91875|
|[ResNet-18](https://drive.google.com/file/d/10Go0fA8TdjL66cKw6H5aHCXjknOyisuG/view?usp=sharing)        |0.735    |0.923|
|[ResNet-101](https://drive.google.com/file/d/1-BD8OWxYSDyng1Rynb9XaC1WsZB-1Oh2/view?usp=sharing) |0.7575  |0.93025|
|[ResNet-152](https://drive.google.com/file/d/1-BEdL-nblY9CFQj1mj5803R3_N2wd5rU/view?usp=sharing)     |0.7655  |0.93575|
|[Wide ResNet-50](https://drive.google.com/file/d/109MTLD6o8hYkfqS5dL-mv5XOd0njIwh0/view?usp=sharing)    |0.76525  |0.93525|
|[Wide ResNet-101](https://drive.google.com/file/d/1-K9NjtTn-Sp4MHFIfxNsRQrJiV5H9m6w/view?usp=sharing) |0.766  |0.9425|
|[ResNeXt-50](https://drive.google.com/file/d/1-LaeQCCzjcNpIb3Cu7pnuL2rfGj48DVc/view?usp=sharing)     |0.7555   |0.94|
|[ResNeXt-101](https://drive.google.com/file/d/1-R-E-xYqfOSkmmfCsTlYctdI-YSrcTAz/view?usp=sharing) |0.777  |0.9452|
|[DenseNet-121](https://drive.google.com/file/d/104mZmdDZFcVPLhQmNwlxWdTEcOmeZA4-/view?usp=sharing)     |0.75175  |0.93375|
|[DenseNet-161](https://drive.google.com/file/d/1-N7zlhRC5YqM1Y8beJKXdaBSRrl_9VO9/view?usp=sharing) |0.77  |0.9375|
|[DenseNet-201](https://drive.google.com/file/d/1-3hxZkYCAHmtwgH8HqxuHFXQuUxGOghG/view?usp=sharing)   |0.771  |0.94025|

## Models:
Get model:
Click link in table above, URL will be in format `https://drive.google.com/file/d/<FILEID>/view`
Replace `<FILEID>` and `FILEOUTPUT` in this command to wget it
```bash
wget --load-cookies /tmp/cookies.txt "https://docs.google.com/uc?export=download&confirm=$(wget --quiet --save-cookies /tmp/cookies.txt --keep-session-cookies --no-check-certificate 'https://docs.google.com/uc?export=download&id=<FILEID>' -O- | sed -rn 's/.*confirm=([0-9A-Za-z_]+).*/\1\n/p')&id=<FILEID>" -O <FILEOUTPUT> && rm -rf /tmp/cookies.txt
```

Load model:
```python
import torch
model = torch.load('<FILEOUTPUT>')
```
All models input with size of 224x224 image

Output is 250x1 array

## Dataset
We use the TU-Berlin dataset, split 60/20/20 for train/val/test

[TU-Berlin Sketch dataset](http://cybertron.cg.tu-berlin.de/eitz/projects/classifysketch/) under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
