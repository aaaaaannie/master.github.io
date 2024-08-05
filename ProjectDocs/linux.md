 * unzip:for file.zip larger than 4G using the command:
     ```
     7za x mypack.zip
     ```
  * check the version of cuda:
    ```
    nvidia-smi
    ```
  * [download]
     * 解压分为7z(7za x filename),unzip(unzip filename.zip)
     * 下载分为wget(for all file types: wget + download link)和gdown(专用Google drive)
  * question: 因为import在上一级无法载入模块
     ```
     import sys
     import os
     sys.path.append(os.path.abspath(os.path.join(__file__, "..", "..")))
     ```
  * download from google cloud
  首先保证电脑中的python可用，激活conda 环境
  1.下载gsutil
     
     ```
     pip install gsutil
     ```
  2.按照如下命令下载即可(会自动生成)
     
     ```
     gsutil -m cp -R  gs://ugc-dataset/original_videos_h264 ./

     ```
* Linux执行sh文件提示Permission denied[https://zhuanlan.zhihu.com/p/481036985]

* jupyter lab 下激活jupyter notebook 中的虚拟环境
     * 先在终端conda激活环境
     * 输入python -m ipykernel install --user --name=myenv指令
     * 在notebook中使用相应的核
* 提取三层文件夹下的子文件
     * for var in /home/sunrui/medfair/data/ADNI_3T/*/*/*/*;do cp "$var"/*.nii /home/sunrui/medfair/data/images-all; done


