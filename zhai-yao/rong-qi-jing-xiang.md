# 容器镜像

华南理工大学高性能计算平台支持Singularity容器平台，支持在不同镜像上运行不同的AI作业模板。

## 本地安装Singularity

下列命令为在本地的Centos7系统上搭建Singularity容器制作环境。

```text
git clone https://github.com/sylabs/singularity.git

cd singularity

git fetch --all

git checkout 2.5.0

./autogen.sh

./configure --prefix=/usr/local

make -j4 && make install
```

{% hint style="info" %}
若在configure步骤中出现报错：configure: error: Unable to find the libarchive headers, need package libarchive-devel \(libarchive-dev on Debian/Ubuntu\)，请执行：
{% endhint %}

{% tabs %}
{% tab title="CentOS" %}
```text
yum install -y libarchive-devel
```
{% endtab %}

{% tab title="Ubuntu" %}
```
apt-get install -y libarchive-dev
```
{% endtab %}
{% endtabs %}

完成安装后，执行下列命令查看是否安装成功。

```text
singularity --version
```

## 查找镜像

Singularity容器支持从Docker容器转换，前往最大的容器网站

## 制作镜像



## 上传镜像

## 管理镜像

