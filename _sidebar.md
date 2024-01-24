<!-- _sidebar.md -->

* Typora+Docsify使用指南
  * [Docsify使用指南](/ProjectDocs/Docsify使用指南.md) <!--注意这里是相对路径-->
  * [Typora+Docsify快速入门](/ProjectDocs/Typora+Docsify快速入门.md)
* Docsify部署
  * [Docsify部署教程](/ProjectDocs/Docsify部署教程.md)
* python
  * [spyder](/ProjectDocs/爬虫.md)
  * [Random Forest](/ProjectDocs/RF.md)
  * [MUST KNOW!!!](/ProjectDocs/Python learner.md)
* R
  * [packages](/ProjectDocs/R包.md)
* Cloud Computing
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

* Linux
  * [Docker](https://blog.csdn.net/xyl192960/article/details/120246820)
     * 利用wget命令即可从网页下载，下面的例子是将网页上的该文件下载到当前路径下
       ```
       wget https://download.pytorch.org/models/resnet18-5c106cde.pth
       ```
     * 对下载的文件进行重命名，例如命名为resnet18.pth
       ```
       wget -O resnet18.pth https://download.pytorch.org/models/resnet18-5c106cde.pth
       ```
 
 

