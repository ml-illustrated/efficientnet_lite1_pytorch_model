# efficientnet-lite1-pytorch-model

Pretrained Pytorch model file for EfficientNet Lite1

## Installation

```
pip install efficientnet_lite1_pytorch_model
```

## Basic Usage

```
from efficientnet_lite1_pytorch_model import EfficientnetLite1ModelFile
print( 'model file path is %s' % ( EfficientnetLite1ModelFile.get_model_file_path() ) )
```

## Actual Usage

Install the model package from [EfficientNet-Lite-PyTorch](https://github.com/ml-illustrated/EfficientNet-Lite-PyTorch):
```
pip install efficientnet_lite_pytorch
```

Load the model with pretrained weights:
```
from efficientnet_lite_pytorch import EfficientNet

from efficientnet_lite1_pytorch_model import EfficientnetLite1ModelFile
weights_path = EfficientnetLite1ModelFile.get_model_file_path()

lite1_model = EfficientNet.from_pretrained('efficientnet-lite1', weights_path = weights_path )
```


## Credits

This package was created with _Cookiecutter_ and the `audreyr/cookiecutter-pypackage` project template.

- _Cookiecutter_: https://github.com/audreyr/cookiecutter
- `audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
- `cookiecutter-ml-model-files`: https://github.com/ml-illustrated/cookiecutter-ml-model-files
