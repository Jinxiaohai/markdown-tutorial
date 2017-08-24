#### 首先安装centos的free和nonfiree的仓库  
* 使用下面的命令安装：  
```shell
yum install localinstall –nogpgcheck https://download1.rpmfusion.org/free/el/rpmfusion-free-release-7.noarch.rpm  
yum install localinstall –nogpgcheck https://download1.rpmfusion.org/nonfree/el/rpmfusion-nonfree-release-7.noarch.rpm  
```

### 安装额外的软件源epel和nux-dextop  
* 安装的方式及命令：  
```shell
rpm -Uvh http://li.nux.ro/download/nux/dextop/el7/x86_64/nux-dextop-release-0-1.el7.nux.noarch.rpm  
```

#### 安装所需要的解码工具和依赖文件  
* 安装的命令：  
```shell
yum -y –enablerepo=nux-dextop install gstreamer-ffmpeg vlc gstreamer-plugins-ugly gstreamer-plugins-bad gstreamer-plugins-ugly ffmpeg libvdpau mpg123 mplayer mplayer-gui gstreamer-plugins-bad-nonfree gstreamer1-libav gstreamer1-plugins-bad-freeworld gstreamer1-plugins-ugly  
```

> centos 发行版一直以来视频解码都是比较难解决的问题，希望在这里可以给你提供帮助。  
