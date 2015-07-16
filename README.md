#SSHMole

OSX 下最好用的 ssh 代理工具。  

##使用说明
1. 第一次打开需要输出管理员密码，绝对安全，不信看代码。  
2. 在Server Config窗口输入服务器、帐号密码，点击Connect：  
![demo](https://raw.githubusercontent.com/OpenFibers/SSHMole/master/DemoPics/demo1.png)  
3. 打开Safari上网。或使用Google Drive、Dropbox等客户端（浏览器或App自动检测系统代理设置即可）。  
4. 随时从系统菜单栏更改服务器或代理设置：  
![demo](https://raw.githubusercontent.com/OpenFibers/SSHMole/master/DemoPics/demo2.png)  
5. 使用时请自觉遵守当地法律法规。  

##Features
1. 多份服务器配置，并支持iCloud同步。  
2. 服务端密码保存在Keychain里，安全。  
3. 支持自动代理（PAC），内置PAC HTTP server，一键更改系统代理设置。
4. 可自定义PAC，或从Web获取最新PAC文件。  
5. 可设置开机自动启动，启动或唤醒Mac时，自动重连上次成功的连接。  

##没有VPS怎么办
买一台。穷用[bandwagon host](http://www.tennfy.com/1347.html)年付$3.99每月100G流量。富用linode。  

##如何共享代理给其他设备
1. 在连接前勾选 Allow Connections from LAN，同局域网内的其他设备即可访问连接成功的SOCKS代理  
2. 连接后本机9099端口会开启HTTP服务，返回PAC文件，同局域网内的其他设备可设置HTTP自动代理为下列链接之一：  
http://your-ip-address:9099/global.pac  全局模式  
http://your-ip-address:9099/whitelist.pac  白名单模式  
http://your-ip-address:9099/blacklist.pac  黑名单模式  
http://your-ip-address:9099/direct.pac  直连（一般没什么卵用）  
http://your-ip-address:9099/mirror.pac  和SSHMole中代理模式相同  

##Logo为什么这么像百度logo？
反正在google搜paw icon就找到这么个矢量图。别问跟百度什么关系，一毛钱关系都没有。凑合看吧。欢迎设计师朋友捐赠Icon。  

##为什么App没经Developer ID签名？
没钱。欢迎土豪捐赠开发帐号，请邮件联系openfibers@gmail.com。  

##下载地址
[SSHMole v1.0.3 build 120](https://github.com/OpenFibers/SSHMole/raw/master/Product/SSHMole_v1.0.3_build120.zip)  

##Change log
[SSHMole v1.0.3 build 120](https://github.com/OpenFibers/SSHMole/raw/master/Product/SSHMole_v1.0.3_build120.zip)  
修复默认PAC文件安装失败。使用过1.0.2之前的版本的话，需要手动删除~/Library/Containers/openthread.SSHMole文件夹，再启动新版

[SSHMole v1.0.2 build 118](https://github.com/OpenFibers/SSHMole/raw/master/Product/SSHMole_v1.0.2_build118.zip)  
修复全新安装启动崩溃（SSHMoleSystemConfigurationHelper未复制或权限错误）

[SSHMole v1.0.1 build 116](https://github.com/OpenFibers/SSHMole/raw/master/Product/SSHMole_v1.0.1_build116.zip)  
修复断开连接或退出时，系统代理设置未被清空的 bug

[SSHMole v1.0 build 114](https://github.com/OpenFibers/SSHMole/raw/master/Product/SSHMole_v1.0_build114.zip)  
自动代理(PAC)、自动连接、Status bar 菜单

[SSHMole v0.1](https://github.com/OpenFibers/SSHMole/raw/master/Product/SSHMole_v0.1.zip)  
全局代理功能

##TODO
1. 增加提示状态menu：未连接/PAC url & SOCKS address
2. 列表中保存两个配置；当第二个通过更改配置和第一个ID一致时，UI会重叠  
3. 中文支持

##Third Party Libs
[GCDWebServer](https://github.com/swisspol/GCDWebServer) by [swisspol](https://github.com/swisspol)  
[SCEvents](http://stuconnolly.com/projects/code/) by [Stuart Connolly](http://stuconnolly.com/about/)  
[OTHTTPRequest](https://github.com/OpenFibers/OTHTTPRequest)  