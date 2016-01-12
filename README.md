# WeiXin
关于微信开发调试
1.下载fiddler
2.通过host绑定本地ip/远程测试ip到目标域名

选择tools-->hosts，在弹出窗口中添加代理地址（自定义）和要访问的ip

3.fiddler设置代理：

       1、首先，确保安装 Fiddler 的电脑和手机在同一局域网内，因为要将手机的代理指向 PC 机，不能互相访问是不行的。
       2、Fiddler 开启远程连接。Fiddler 主菜单 Tools -> Fiddler Options…-> Connections页签，选中Allow remote computers to connect。

       3、重启Fidler（这一步很重要，必须做）。

       4、获取PC的IP地址：
4.打开IPhone, 找到你的网络连接，打开HTTP代理，输入Fiddler所在机器的IP地址(比如:192.168.1.104) 以及Fiddler的端口号8888
大功告成，可以使用手机访问设定的域名，别忘了在微信公众号里将此域名配置为js安全接口域名。之后就可以在本地调试js-sdk了。

