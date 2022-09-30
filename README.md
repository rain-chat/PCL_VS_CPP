# PCL点云使用手册
## 一、配置PCL
### 1.下载PCL 
下载地址：
```
https://github.com/PointCloudLibrary/pcl/releases
```
目标文件：
```
PCL-1.12.0-AllInOne-msvc2019-win64.exe
pcl-1.12.0-pdb-msvc2019-win64.zip
```
### 2.运行 PCL-1.12.0-AllInOne-msvc2019-win64.exe
安装目录默认就行，也可以指定。我使用的是默认 C:\Program Files\PCL 1.12.1
![image](https://user-images.githubusercontent.com/75610421/193257443-831748d4-be59-4973-95cf-ef1cc5bc0f22.png)

这里选择第二个，第一个也行。都需要手动配置一些东西。其他地方直接下一步即可。

### 3.安装 OpenNI-Windows-x64-2.2.msi
该文件是上一步安装时自动下载的文件。上一步安装目录是C:\Program Files\PCL 1.12.1

该文件所在目录 C:\Program Files\PCL 1.12.1\3rdParty\OpenNI2

运行该程序，界面如下，如果不确定是否安装过，可以先点remove,再点repair。

![image](https://user-images.githubusercontent.com/75610421/193259654-ec7118f2-56fc-4147-9018-98e23df7526c.png)

安装目录需改为C:\Program Files\PCL 1.12.1\3rdParty\OpenNI2，即OpenNI-Windows-x64-2.2.msi所在目录

### 4.解压 pcl-1.12.0-pdb-msvc2019-win64.zip并将里边的文件复制到C:\Program Files\PCL 1.12.1\bin目录。
![image](https://user-images.githubusercontent.com/75610421/193260926-4db30ed8-c20e-4140-ab00-c8381b253c19.png)

![image](https://user-images.githubusercontent.com/75610421/193260604-af170e9c-3af9-423a-984a-326266da524a.png)

### 5.配置   系统环境变量。
如果第一步点了第二个。这四个就自动配置完成了。具体内容如下。
```
OPENNI2_INCLUDE64    C:\Program Files\PCL 1.12.1\3rdParty\OpenNI2\Include\
OPENNI2_LIB64        C:\Program Files\PCL 1.12.1\3rdParty\OpenNI2\Lib\
OPENNI2_REDIST64     C:\Program Files\PCL 1.12.1\3rdParty\OpenNI2\Redist\
PCL_ROOT             C:\Program Files\PCL 1.12.1
```
![image](https://user-images.githubusercontent.com/75610421/193261666-7377bb7b-99a5-44da-a1f5-f081f9b5eea8.png)
接下来是我们需要配置的。
编辑Path,添加下列地址
```
C:\Program Files\PCL 1.12.1\3rdParty\OpenNI2\Lib
C:\Program Files\PCL 1.12.1\3rdParty\OpenNI2\Tools
C:\Program Files\PCL 1.12.1\3rdParty\OpenNI2\Redist
C:\Program Files\PCL 1.12.1\bin
C:\Program Files\PCL 1.12.1\3rdParty\VTK\bin
C:\Program Files\PCL 1.12.1\3rdParty\Boost\include
C:\Program Files\PCL 1.12.1\3rdParty\FLANN\bin
C:\Program Files\PCL 1.12.1\3rdParty\Qhull\bin
```
根据自己安装PCL的目录作改变，上述地址实际上就是PCL的目录地址，其他同理，直接找到对应目录复制以免错误。
![image](https://user-images.githubusercontent.com/75610421/193264744-97b6770c-5a4c-469b-b5d7-dfa51916f3df.png)
![image](https://user-images.githubusercontent.com/75610421/193264854-11be8803-8ef9-4f55-9735-3ef66a7316b3.png)

配置完成如下图

![image](https://user-images.githubusercontent.com/75610421/193262715-5159274e-a707-4d66-84f6-d5d99fa26d6d.png)


