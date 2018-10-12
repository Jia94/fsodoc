#################
Singularity
#################

实况分析系统采用Singularity容器技术进行封装，可以有效隔离依赖软件环境的搭建、环境变量的配置等细节。

###安装或更新依赖

.. code:: bash
    sudo yum update && \
    sudo yum groupinstall 'Development Tools' && \
    sudo yum install libarchive-devel
###下载并安装最新版本

.. code:: bash
    git clone https://github.com/singularityware/singularity.git
    cd singularity
    ./autogen.sh
    ./configure --prefix=/usr/local --sysconfdir=/etc
    make
    sudo make install
###导入镜像文件

工作站中应该存在FSO系统的Singularity镜像文件**fso3.simg**

.. code:: bash 

    ls -al fso3.simg
    
###参考网页

http://singularity.lbl.gov/docs-installation
  
