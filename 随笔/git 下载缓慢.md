## 解决使用git clone 命令下载缓慢问题
亲测方法二有效
### 方法一：修改host文件
windiws host文件位置：C:\Windows\System32\drivers\etc 可以用记事本打开
linux host文件位置: \etc\hosts
通过[网站](https://www.ipaddress.com/)获取 ```github.com``` 和```github.global.fastly.net``` 的IP Address(多个IP时任选一个),
在host 文件添加如下
```
IP Address1 github.com
IP Address2 github.global.fastly.net
```
在终端或CMD中，执行```ipconfig/flushdns```命令
### 方法二：使用github cnpmjs镜像
修改```git clone https://github.com/xxx.git``` 为```git clone https://github.com.cnpmjs.org/xxx.git```，通过使用代加速
### 方法三：使用gitlab镜像
使用```git clone https://gitlab.com/xxx.git```
### 方法三：使用码云
从[码云](www.gitee.com)上clone