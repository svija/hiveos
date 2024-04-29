
hiveos  cpu 
======================================
cd /hive
mkdir btfcpu
sudo chmod 777 -R ./btfcpu
cd btfcpu
wget   https://www.iepool.com/IEPool_BCF_Miner_ver2.8.1.zip
sudo chmod 777 ./IEPool_BTF_Miner_ver2.8.1.zip
sudo unzip ./IEPool_BTF_Miner_ver2.8.1.zip
sudo chmod 777 -R ./*
sudo unzip ./IEPool_BTF_Miner_ver2.8.1.zip
sudo chmod 777 -R ./*
cd  IEPool_BTF_Miner_ver2.8.1
sudo chmod 777 ./*
sudo vim run.sh
-----------------------------------------------------------
根据hiveos 的cpu配置，如果是24 CPU 则： -t 48
iepool的run.sh配置有误，把--coinbaseaddress 更改为: -u   <doji钱包地址>.<矿工名>
运行： ./run.sh
-----------------------------------------------------------


hiveos card
=====================================
-----------------------------------------------------------
操作前：先设置飞行表,安装好驱动，CUDA
BTC  - CCminer  -  sha256d - <doji钱包地址>.<矿工名>  -  密码填写:BTF   -  Tpruvot  - 版本2.3.1
执行飞行表会自动更新CCminer到Rig机，然后webshell粘贴以下脚本执行。
-----------------------------------------------------------



echo "下载HIVEOS CCMINER依赖库"
echo "***********************************************"
wget https://github.com/svija/hiveos/releases/download/hiveos/hiveos.zip
echo "解压依赖库..."
echo "***********************************************"
sudo  chmod 777 -R ./hiveos.zip
sudo unzip ./hiveos.zip
sudo chmod 777 -R ./*
echo "开始安装 CCminer依赖库"
echo "***********************************************"
sudo ./install.sh



----------------------------------------
运行矿机前，应手动修改ccminer目录中cgminer.conf 替换矿池线路和钱包地址
----------------------------------------
