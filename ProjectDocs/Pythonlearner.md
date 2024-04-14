# 充分提升下载速度
```
pip install 要安装的包名 -i https://pypi.douban.com/simple
```
# 读取npz文件
``` 
import numpy as np
file_path="data_00001.npz"
poem=np.load(file_path,allow_pickle=True)
poem.files
```
# 一些云端下载的方式
## azcopy:
需要定位到文件夹，然后:
```
./azcopy copy 'link' dir --recursive
```

