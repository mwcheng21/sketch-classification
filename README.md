# Finetuning pretrained ImageNet Image Classifiers for Free-hand Sketch Recognition

20 Epoch fine tuning
| Model type | top-1  | top-5  |
|------------|---|---|
|AlexNet       |0.659    |0.8805|
|SqueezeNet    |0.6595   |0.87925|
|VGG-11_bn          |0.72425  |0.909|
|VGG-11 |0.69725  |0.89175|
|VGG-19_bn         |0.73825  |0.924|
|VGG-19 |0.721  |0.9055|
|ShuffleNet    |0.168    |0.392|
|MobileNet     |0.729    |0.91475|
|MNASNet       |0.7205   |0.92075|
|GoogLeNet     |0.7175   |0.91875|
|ResNet-18        |0.735    |0.923|
|ResNet-101 |0.7575  |0.93025|
|ResNet-152     |0.7655  |0.93575|
|Wide ResNet-50    |0.76525  |0.93525|
|Wide ResNet-101 |0.766  |0.9425|
|ResNeXt-50       |0.7555   |0.94|
|ResNeXt-101 |0.777  |0.9452|
|DenseNet-121      |0.75175  |0.93375|
|DenseNet-161 |0.77  |0.9375|
|DenseNet-201   |0.771  |0.94025|

## Models:
Get model:
Click link, URL will be in format `https://drive.google.com/file/d/<FILEID>/view`
Replace `<FILEID>` and `FILEOUTPUT` in this command
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

[Shufflenet](https://drive.google.com/file/d/1-CBr2qc8xHAqtYuXKnEKrKOe6JySiQyx/view?usp=sharing)

[ResneXt](https://drive.google.com/file/d/1-LaeQCCzjcNpIb3Cu7pnuL2rfGj48DVc/view?usp=sharing)

[AlexNet](https://drive.google.com/file/d/1-S2glVkseE-GCd9fjeeCxbys71i1HqFh/view?usp=sharing)

[VGG](https://drive.google.com/file/d/1-cCo9FNSL3EUPIJEPV-RDyl-QLHzE5Gm/view?usp=sharing)

[SqueezeNet](https://drive.google.com/file/d/1-vaCEBBqCPO6dSrOJawdXAViK-UmXFWP/view?usp=sharing)

[DenseNet](https://drive.google.com/file/d/104mZmdDZFcVPLhQmNwlxWdTEcOmeZA4-/view?usp=sharing)

[MNASTNet](https://drive.google.com/file/d/106PacomRKaiy8k47iOFUmsPlGekmFQ39/view?usp=sharing)

[Wide ResNet](https://drive.google.com/file/d/109MTLD6o8hYkfqS5dL-mv5XOd0njIwh0/view?usp=sharing)

[ResNet](https://drive.google.com/file/d/10Go0fA8TdjL66cKw6H5aHCXjknOyisuG/view?usp=sharing)

[GoogLeNet](https://drive.google.com/file/d/10S2v3TkP_9dHh-dXrO7uNj5f0nXZSpmT/view?usp=sharing)

[MobileNet](https://drive.google.com/file/d/1weqhBx0Rs4b7rfOQI8G9gHm8crBp1b3Y/view?usp=sharing)


## Dataset
[TU-Berlin Sketch dataset](http://cybertron.cg.tu-berlin.de/eitz/projects/classifysketch/) under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
