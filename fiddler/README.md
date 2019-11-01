[fiddler官网](http://www.telerik.com/fiddler)
* 配置fiddler
    * 点击页面顶部Tools,选择fiddler options（有的版本直接显示的是options
    ![](https://github.com/Elf-ball/test/raw/master/fiddler/1.png)
    * 在弹框中选择connections,点击勾选页面中的Allow remote computers to connect(这里顺带检查下端口号是否为8888)
    ![](https://github.com/Elf-ball/test/raw/master/fiddler/2.png)
    * 进入弹框页Https,勾选Capture HTTPS traffic,这里可能会选择安装证书.安装完证书后勾选Igonore sever certificate errors(unsafe)
    ![](https://github.com/Elf-ball/test/raw/master/fiddler/3.png)
    * 重启fiddler
    * fiddler安装配置完成,准备抓取手机数据.保证手机和电脑的网络处于同一局域网下
    * 手机链接局域网wifi，进入wifi高级设置设置代理为手动.设置代理服务器地址为电脑IP地址（进入电脑cmd使用命令ipconfig获取），设置端口号为8888
    
    ![](https://github.com/Elf-ball/test/raw/master/fiddler/4.png)
    
    * 进入手机浏览器在搜索栏中输入Ip地址加端口号.如：192.168.0.0：8888
    
    ![](https://github.com/Elf-ball/test/raw/master/fiddler/5.png)
    * 这里就会进入到fiddler页面,点击页面最底部链接安装证书
    * 配置完成,在手机上操作就能在电脑上看到手机请求的数据了


# 备注
    * 如果设置完fiddler后，抓iOS数据包的时候提示“连接的服务器可能被伪装”，就在iOS设置-通用-关于手机-证书信任设置->进入证书信任设置中打开下载下的证书信任开关
