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

##下载地址
[SSHMole v1.0 build 114](https://github.com/OpenFibers/SSHMole/raw/master/Product/SSHMole_v1.0_build114.zip) 

##历史版本
[SSHMole v0.1](https://github.com/OpenFibers/SSHMole/raw/master/Product/SSHMole_v0.1.zip) 仅支持全局代理

##TODO
1. 列表中保存两个配置；当第二个通过更改配置和第一个ID一致时，UI会重叠  
2. 中文支持
