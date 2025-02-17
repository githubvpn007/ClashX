 # ClashX            
ClashX，ClashX教程，ClashX配置教程，ClashX for mac，vpn代理  



#### 本项目不做VPN分享，如果您希望获得最佳的科学上网方案 [点击这里](https://github.com/githubvpn007/v2rayNvpn)  

#### 如果你想知道clash/ss/ssr/v2ray/trojan 的区别的话 [请点这里](https://github.com/githubvpn007/proxy)


简介
----

Clash 是一个使用 Go 语言编写，基于规则的跨平台代理软件核心程序。  
ClashX 是运行在 macOS 上的一款科学上网工具。  

**支持的协议:**  
 Vmess  
 Shadowsocks  
 Snell  
 SOCKS5  
 
 
 **特色**  
- 可随时切换代理模式及节点  
- 支持节点批量延迟测试  
- 通过托管链接一键配置  
- 规则命中分析  
- 日志输出  


**设备要求**  

系统要求：macOS 10.5 及以上   

设备要求：MacBook / iMac / Mac Pro  



<br/>
<br/>




步骤
----


**1.下载安装**




~~https://github.com/yichengchen/clashX/releases 官方项目已经下架~~  

本站下载： 
|  文件   | 说明  |
|  ----  | ----  |
| [ClashX.dmg](https://github.com/githubvpn007/ClashX/releases/download/ClashX/ClashX.zip)  | macOS 系统安装文件 |
| [源文件压缩包 zip 版本](https://github.com/githubvpn007/ClashX/releases/download/ClashX/1.118.0.zip)  | 源文件压缩包 zip 版本 |
| [Source code (tar.gz)](https://github.com/githubvpn007/ClashX/releases/download/ClashX/1.118.0.tar.gz)  | 源文件压缩包 tar.gz 版本 |



**提示：** ClashXR是第三方修改版本，支持SSR协议。ClashX现已支持SSR协议。ClashXR已经完成了它的历史使命。建议直接使用ClashX最新版本。   




**2.请先在机场官网或其它地方复制自己的 Clash 订阅.没有Clash(R)订阅？[请移步](https://github.com/githubvpn007/v2rayNvpn)**  



**3.请打开 ClashX 软件。**  
首次使用 ClashX 时，macOS 会提醒你此应用来自未知开发者，请允许打开此应用。  
ClashX 首次运行会提示是否安装帮助程序（Helper）。此帮助程序用于设置系统代理，  
否则每次你通过 ClashX 变更系统系统状态（打开或关闭）时都需要输入密码，请点击 “Install”，之后 macOS 会提示输入用户密码。  

![](https://i.postimg.cc/XJjxn4vg/1.png)  


**4.添加订阅**  

启动 ClashX，点击状态栏中的 **ClashX 图标**，依次选择「配置」、「托管配置」、「管理」，在弹出的界面点击添加订阅。  

![](https://i.postimg.cc/pXhCW0P3/2.png)  
![](https://i.postimg.cc/W3583CFc/3.png)  
![](https://i.postimg.cc/rsb9G4Nh/4.png)  


**5.选中我们刚刚订阅生成的配置文件**  

添加订阅若干秒后将在软件里看到刚刚添加的配置文件。

![](https://i.postimg.cc/JzjQJGDq/5.png)  



**6.启动**  

点击 ClashX 状态栏图标，将「出站模式」选为「规则判断」，在「Proxy」或「Gloabal」策略组中可以选择自己喜欢的线路，然后点击「设置为系统代理」即可开始使用。  

「Proxy」或「Gloabal」策略组是用于访问国际互联网的默认策略，一般情况下，所有国际网络的访问都通过该策略组中选择的节点进行连接。  

![](https://i.postimg.cc/yxWPSjcg/6.png)   
![](https://i.postimg.cc/y6rnzqCF/7.png)   
![](https://i.postimg.cc/gkCDnvJj/8.png)   

此时您已可以自由地连接国际互联网。




<br/>
<br/>


策略说明
----

**策略组的特性**  

- 可以包含节点或其他策略组
- 具有多种不同的策略类型
- 服务于规则 



**不同策略组的作用**  


- Global (或Proxy，视配置文件具体情况而定)：主要规则代理分组，需手动选定一个你要使用的节点作为默认的节点。无其它修改的话，所有国际网络的访问都通过该策略组中选择的节点进行连接。  

- Netflix：指Netflix流媒体的分组，如选择香港节点，则显示港区内容。其它地区的同理。  
- Spotify：指Spotify流媒体的分组，仅用于加速访问。Spotify执行锁区政策，根据账号注册时所在地进行内容展示，更换节点并不能显示其它地区的版权内容。  
- YouTube：指YouTube流媒体的分组，使用不同的线路将展示不同地区的特色内容。  
- Telegram：指Telegram（电报）的分组，国内手机号注册的用户选择新加坡线路也许可以加速（注意：是也许。因为+86号段注册的电报用户数据都在新加坡数据中心）。  
- China：访问中国大陆网站所用的策略。大陆用户请选择 DIRECT （直接连接）；海外用户请选择回国线路。  
- Auto：软件每隔一段时间会自动进行测试并排序，自动评选出延迟最低的节点，当其它策略组里选择了 auto 策略，那么效果就是该策略组将每隔一段时间自动切换到延迟最低的线路。（如果你有登陆脸书、IG等社交媒体，不建议使用该策略，以免由于IP变动造成风控，甚至封号。）    
- fallback：可用性策略。与故障转移类似，按照节点顺序选择第一个可用节点。



<br/>
<br/>

常见错误
----

1.如果遇到以下提示：  

说明用错了订阅链接，请检查自己是不是复制错了或者多了空格之类的。  

没有 Clash 订阅链接的可以使用订阅转换API来转换订阅链接。  


`Invalid Config:yaml:
unmarshal errors:line 1:cannot unmarshal !!str c3M6Ly9...`  



2.如果遇到此类提示：  

说明你还没买套餐，或者订阅为空。请联系你所在机场的管理员。  


`Invalid Config:
Value for 'Proxy' is invalid:Unexpected null or empty`  





3.如果遇到此提示:  

说明你使用的加密算法不被Clash支持。请更换加密算法。推荐：ChaCha20-ietf-poly1305  


`...cipher not supported`



<br/>





