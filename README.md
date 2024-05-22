
## 代码说明 :ledger: :ledger:

本代码克隆于2024年5月12日，版本号为YOLOv5_v7.0。

本代码在YOLOv5的基础上，集成各种主干网路、注意力机制函数、以及损失函数。

主要用于学习不同模块之间的区别，快速找到适合自己数据集的那个模型。

## 更新日志

2024年5月21日

添加边界框损失函数
```python
GIoU (bool, optional): If True, calculate Generalized IoU. Defaults to False.
DIoU (bool, optional): If True, calculate Distance IoU. Defaults to False.
CIoU (bool, optional): If True, calculate Complete IoU. Defaults to False.

EIoU (bool, optional): If True, calculate Efficient IoU. Defaults to False.
SIoU (bool, optional): If True, calculate Scylla IoU. Defaults to False.
WIoU (bool, optional): 
ShapeIoU (bool, optional): 
mpdiou (bool, optional): 
```

更新注意力机制函数

```python
from .CA import *
from .CBAM import *
from .ECA import *
from .GAM import *
from .DAT import *
```

2024年5月20日
添加基准模型，YOLOv3，YOLOv5，YOLOv6，YOLOv8，YOLOv9


2024年5月18日，添加注意力机制函数

```python
from CA import *
from CBAM import *
from ECA import *
from GAM import *

```


2024年5月16日，添加主干网络

```python
from .FasterBlock import *

from .MobileNetV1 import *
from .MobileNetV2 import *
from .MobileNetV3 import *
from .MobileNetV4 import *
from .MobileViTv1 import *
from .MobileViTv2 import *

from .ShuffleNetV1 import *
from .ShuffleNetV2 import *

from .EfficientNetV1 import *
from .EfficientNetV2 import *
from .EfficientViT2 import *

from .GhostNetV1 import *
from .GhostNetV2 import *
from .GhostNetV3 import *

```

