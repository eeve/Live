# 看直播

可指定直播源，观看直播。


## 直播源

直播源在 [sources.json](./sources.json) 中定义，可自行添加或删除直播源。


## Chrome跨域问题


### Windows系统

- 在Chrome的快捷图标上点击鼠标右键

- 选择属性

- 选择快捷方式标签

- 在目标里面，在原 `Chrome` 路径的基础上加上一段参数，具体参数根据 `Chrome` 的版本有区别，说明如下：
    
    Chrome 49 之前的版本: --disable-web-security

    Chrome 49 之后的版本: --disable-web-security --user-data-dir=C:\chrometmp （注意 `C:\chrometmp` 是你本地硬盘的一个目录，自己新建它）

- 点击应用

- 点击确定关闭属性窗口

- 关闭所有已打开的 `Chrome` ，重新启动

- 看到地址栏下面的小黄条你使用的是不受支持的命令标记 `--disable-web-security`，就成功了

    ![](https://i.loli.net/2018/07/24/5b56f251d670d.jpg)

    ![](https://i.loli.net/2018/07/24/5b56f331d3ccc.png)
    
    出现上图的提示条，则代表成功。

### MacOS & Linux

方法和Windows类似，找到Chrome的二进制文件，在终端中带上参数打开即可。或者找到相关的启动脚本（桌面快捷方式），在启动脚本里加上参数即可。

