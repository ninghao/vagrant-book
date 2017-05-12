# 管理镜像

**任务：**

熟悉虚拟机镜像的管理流程。

## 镜像

box 就是 Vagrant 里用的系统镜像。镜像有点像是把安装好的操作系统打了个包，生成一个文件。Vagrant 里的 box 有不同的类型，可以用在不同的 Provider 上，比如有适合在 Virtualbox 上用的 box，有适合在 VMware 上用的 box。

Vagrant 在它的云服务上提供下载这些镜像，有的镜像是 CentOS 系统，有些是 Ubuntu 系统，有些可能是用户自己修改之后的某类操作系统。比如有些镜像里面已经安装好了网站的运行环境，用这种镜像创建的虚拟机，启动以后就会拥有一个配置好的网站运行环境了。

### 搜索镜像

在 Atlas 上面可以搜索你需要的镜像，你也可以把自己做好的镜像推送给 Atlas，这样所有人都可以使用你做的镜像了。

**Atlas**

[https://atlas.hashicorp.com/boxes/search](https://atlas.hashicorp.com/boxes/search)

**下面是 centos/7 这个镜像的地址：**

[https://atlas.hashicorp.com/centos/boxes/7](https://atlas.hashicorp.com/centos/boxes/7)

这个镜像的名字是 centos/7，centos 是用户在 Atlas 上的用户名，直接是操作系统的名字，所以这个用户应该就是 CentOS 官方用户。斜线后面的 7 是这个镜像的拥有者为镜像起的名字，如果是官方用户提供的镜像，一般会用它表示镜像里的操作系统的版本。

打开镜像的页面，你会看到镜像的介绍，可用的版本，还有镜像适用的 Provider 都有什么，这个 centos/7 镜像有几个不同的类型：

* vmware\_desktop
* virtualbox
* libvirt




