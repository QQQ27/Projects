[清华tuna源](https://mirrors.tuna.tsinghua.edu.cn/help/anaconda/)
anaconda配置文件 用户文件夹下.condrc文件
换源后报错：CondaHTTPError: HTTP 000 CONNECTION FAILED for url <...> Elapsed: - An HTTP error occurred when trying to retrieve this URL. 
* https --> http
* 添加代理：export all_proxy=socks5://127.0.0.1:1080