 * unzip:for file.zip larger than 4G using the command:
     ```
     7za x mypack.zip
     ```
  * check the version of cuda:
    ```
    nvidia-smi
    ```
  *[download]
     *解压分为7z(7za x filename),unzip(unzip filename.zip)
     *下载分为wget(for all file types: wget + download link)和gdown(专用Google drive)
  *question: 因为import在上一级无法载入模块
     ```
     import sys
     import os
     sys.path.append(os.path.abspath(os.path.join(__file__, "..", "..")))
     ```
