# Finetuning pretrained ImageNet Image Classifiers for Free-hand Sketch Recognition
## !!!!!CURRENTLY IN PROGRESS!!!!!!

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

## Models:
Get model:
Click link, URL will be in format `https://drive.google.com/file/d/<FILEID>/view`
`!wget --load-cookies /tmp/cookies.txt "https://docs.google.com/uc?export=download&confirm=$(wget --quiet --save-cookies /tmp/cookies.txt --keep-session-cookies --no-check-certificate 'https://docs.google.com/uc?export=download&id=<FILEID>' -O- | sed -rn 's/.*confirm=([0-9A-Za-z_]+).*/\1\n/p')&id=1qEGk84k8KGK93jRD9OIlW1Ed4c5Iq96Z" -O <FILEOUTPUT> && rm -rf /tmp/cookies.txt`

Load model:
`import torch
model = torch.load('<FILEOUTPUT>')`


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

