# My-list
本人自用的list规则，用于备份config.yaml文件在线获取规则。

直连地址

https://raw.githubusercontent.com/ec-to/My-list/main/DIRECT.list


代理地址

https://raw.githubusercontent.com/ec-to/My-list/main/proxy.list


加速域名

https://v6.gh-proxy.org/  （优先）

https://ghproxy.net/ 

https://mirror.ghproxy.com/ 

https://gh-proxy.com/ 

https://ghproxy.org/



代码示例
```code
  在线直连: # 本地自定义直连域名列表
    <<: *Classical
    path: ./etc/在线直连.list  
    url: "https://v6.gh-proxy.org/https://raw.githubusercontent.com/ec-to/My-list/main/DIRECT.list"
  在线代理: # 本地自定义直连域名列表
    <<: *Classical
    path: ./etc/在线代理.list  
    url: "https://v6.gh-proxy.org/https://raw.githubusercontent.com/ec-to/My-list/main/proxy.list"
```
