# Download MIMIC
```
CommandException: 30000 file/object could not be transferred Error
```
# 在使用到huggingface时，下载连接不稳定导致，ConnectError。
```
import os
os.environ["HF_ENDPOINT"] = "https://hf-mirror.com"
```
