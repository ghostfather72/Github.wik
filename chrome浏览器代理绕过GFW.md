### 安装SwitchyOmega
首先你需要安装SwitchyOmega.SwitchyOmega可以[在谷歌应用商店安装](https://chrome.google.com/webstore/detail/proxy-switchyomega/padekgcemlokbadohgkifijomclgjgif/?hl=en)
如果因为网络问题安装失败，

可以直接[在Github上下载最新离线包](https://github.com/FelisCatus/SwitchyOmega/releases)，然后按照下载页面上的说明手动安装。

### 导入备份
![图](https://github.com/FelisCatus/SwitchyOmega/wiki/images/t1/step1.png)


按照下图，在导入导出页面点击“从备份文件恢复[备份文件下载](https://raw.githubusercontent.com/gugejun/The-chain/master/pac.bak)
下图中打开一个选择文件的对话框，这时候选择刚下载好的备份文件就行了

![图](https://github.com/FelisCatus/SwitchyOmega/wiki/images/t1/step2.png)

### 设置代理服务器



![图](https://github.com/FelisCatus/SwitchyOmega/wiki/images/t1/step3.png)

这部分比较简单，在“GFWed”情景模式设置好代理协议和端口就好了。再一次说明，请仔细阅读您所使用的代理软件说明书，尤其是不要填错了代理协议（常见的有HTTP或SOCKS），因为那个填错了有一大堆问题，程序还不会提示你填错了。

添加pac下载地址：https://raw.githubusercontent.com/breakwa11/gfw_whitelist/master/whiteiplist.pac

![图](https://github.com/gugejun/Picture/blob/master/1.png?raw=true)

接下来添加规则列表网址，已迁移到[github参考](https://github.com/gfwlist/gfwlist)
最新地址：https://raw.githubusercontent.com/bfwlist/web/master/a.txt
https://raw.githubusercontent.com/gfwlist/gfwlist/master/gfwlist.txt



### 依次改成自动切换模式

![图](https://github.com/gugejun/Picture/blob/master/2.png?raw=true)

Google Chrome已经支持基于https和SPDY的安全代理。其原理和效果与SSH，shadowsocks以及goagent类似：

将普通流量封装在加密通道之中，这样GFW就看不见流量的内容
域名的解析在代理服务器这端完成，所以本地不用担心域名污染的问题。配合pac的使用，可以享受国内CDN的服务。达到一次设置完全免维护
本地不从服务器端取得ip，只适合浏览器内的应用，不适合VoIP，网络游戏等应用。
优点有：

在PC和Mac上Chrome已经原生支持，不需要依赖额外的客户端;
封装的协议是https或SPDY，GFW完全没有DPI识别的可能，这是翻墙终极方案的一部分;
由Google支持，客户端和服务器端的软件成熟并且稳定，未来更新也可靠。
现有的缺点有：

暂时只适用于PC和Mac上的Chrome。Android的客户端有待开发.iOS客户端的可行性暂时还不清楚。