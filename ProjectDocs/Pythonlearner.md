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
# Some methods for cloud transfer data:
## azcopy:
需要定位到文件夹，然后:
```
./azcopy copy 'link' dir --recursive
```

# baipan convey data
## install related packages:
```
pip install requests -i https://pypi.doubanio.com/simple
pip install bypy -i https://pypi.doubanio.com/simple
```
## then,get the corresponding authorization:
```
bypy info
```
## download specific data from the folder named 'bypy':
```
bypy downdir -v
#use the below command to download specific data
bypy downdir dirname -v
#upload
bypy upload -v
```
## Cancel authorization:
```
bypy -c
```
## List all files
```
bypy list
```

