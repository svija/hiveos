
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


hiveos card
=====================================
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
