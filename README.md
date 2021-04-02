# The-most-successful-install-process-of-python
copy from https://www.jianshu.com/p/6059f7fc2cd0


1.准备

在安装之前，请使用以下命令安装Python的先决条件。


sudo apt-get install build-essential checkinstall


sudo apt-get install libreadline-gplv2-dev libncursesw5-dev libssl-dev libsqlite3-dev tk-dev libgdbm-dev libc6-dev libbz2-dev
    
    
2.安装

使用python官方站点的以下命令下载Python。您也可以下载最新版本代替下面指定的版本。


cd /usr/src


sudo wget https://www.python.org/ftp/python/3.7.0/Python-3.7.0.tgz


sudo tar xzf Python-3.7.0.tgz


3. 编译

使用下面的命令集来使用altinstall在您的系统上编译python源代码。


cd Python-3.7.0


sudo ./configure --enable-optimizations --with-ssl


sudo make altinstall


make altinstall用于防止替换默认的python二进制文件/ usr / bin / python。


4.检查Python版本


python3.7 -V


问题：安装python3.7出现ModuleNotFoundError: No module named ‘_ctypes’解决办法


解决办法：


sudo apt-get update


sudo apt-get upgrade


sudo apt-get dist-upgrade


sudo apt-get install build-essential python-dev python-setuptools python-pip python-smbus


sudo apt-get install build-essential libncursesw5-dev libgdbm-dev libc6-dev


sudo apt-get install zlib1g-dev libsqlite3-dev tk-dev


sudo apt-get install libssl-dev openssl


sudo apt-get install libffi-dev


make install


作者：hiekay
链接：https://www.jianshu.com/p/6059f7fc2cd0
来源：简书
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。
