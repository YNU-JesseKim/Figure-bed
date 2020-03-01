# GitHub+PicGo搭建在线图床

## 1 创建GitHub账号

直接到[GitHub](https://github.com/)官网注册即可，可以选择邮箱或者其他方式。

## 2 创建仓库

注册完GitHub账号以后登录，按照下面的操作创建一个仓库。

点击加号新建一个仓库：

![](https://cdn.jsdelivr.net/gh/YNU-JesseKim/Figure-bed/img/static/image-2020022516251574.png)

填写仓库信息：

![](https://cdn.jsdelivr.net/gh/YNU-JesseKim/Figure-bed/img/static/image-2020022516290581.png)

## 3 生成token

点击个人，点击设置：

![](https://cdn.jsdelivr.net/gh/YNU-JesseKim/Figure-bed/img/static/image-20200225163541095.png)

下拉找到Developer settings点击：

![](https://cdn.jsdelivr.net/gh/YNU-JesseKim/Figure-bed/img/static/image-20200225163750054.png)

点击Personal access tokens：

![](https://cdn.jsdelivr.net/gh/YNU-JesseKim/Figure-bed/img/static/image-20200225163846279.png)

点击Generate new token：

![](https://cdn.jsdelivr.net/gh/YNU-JesseKim/Figure-bed/img/static/image-20200225163940029.png)

自定义一个名字，勾选repo：

![](https://cdn.jsdelivr.net/gh/YNU-JesseKim/Figure-bed/img/static/image-20200225164120598.png)

接着下拉点击Generate token即可

![](https://cdn.jsdelivr.net/gh/YNU-JesseKim/Figure-bed/img/static/image-20200225164222694.png)

接着就能看见创建的token。注意token只显示这一次，之后就隐藏不能查看了，所以复制保存起来。

![](https://cdn.jsdelivr.net/gh/YNU-JesseKim/Figure-bed/img/static/image-20200225164430692.png)

## 4 配置PicGo

先下载PicGo，点击[PicGo的GitHub下载地址](https://github.com/Molunerfinn/PicGo/releases)下载

- Windows 下载最新版本的 `exe` 文件。还可以使用 [Scoop](https://scoop.sh/) 来安装 PicGo: `scoop bucket add helbing https://github.com/helbing/scoop-bucket` & `scoop install picgo`。
- macOS 下载最新版本的 `dmg` 文件。还可以使用 `brew cask` 来安装 PicGo: `brew cask install picgo`。
- Linux下载 `AppImage` 文件。如果是 Arch 类的 Linux 用户，可以直接通过 `aurman -S picgo-appimage` 来安装 PicGo。

下载后安装打开，按照如下格式填写即可：

![](https://cdn.jsdelivr.net/gh/YNU-JesseKim/Figure-bed/img/static/image-20200225165258876.png)

说明：

- 仓库名是：用户名/仓库名
- 分支名填写master即可
- Token把刚刚生成保存的复制粘贴过来即可
- 指定存储路径可选，不填则上传后直接在readme目录下

补充一点，可以结合jsDelivr来加速，只需要在自定义域名一栏配置即可，如下图所示：

![](https://cdn.jsdelivr.net/gh/YNU-JesseKim/Figure-bed/img/static/image-20200226104841012.png)

格式：https://cdn.jsdelivr.net/gh/用户名/图床仓库名

## 5 快捷键和相关配置

可以把快捷键设置为自己习惯的按键（自定义）：

![](https://cdn.jsdelivr.net/gh/YNU-JesseKim/Figure-bed/img/static/image-20200225170003890.png)

因为该软件轻量，建议打开更新提示和开机自启：

![](https://cdn.jsdelivr.net/gh/YNU-JesseKim/Figure-bed/img/static/image-20200225170230071.png)

到此就配置完毕了。

## 6 使用说明

只要有图片在剪切板（无论是复制的还是刚刚截图编辑好的），通过设定的快捷键就可以上传到GitHub，上传完成后就可以Ctrl + V粘贴图片地址了，而生成的图片地址也可以选择，这样上传完成后就能得到自己想要的链接格式。

![](https://cdn.jsdelivr.net/gh/YNU-JesseKim/Figure-bed/img/static/image-20200225170708217.png)
