# My-list
本人自用的list规则，用于备份config.yaml文件在线获取规则。

## 地址
 直连地址

https://raw.githubusercontent.com/ec-to/My-list/main/DIRECT.list


 代理地址

https://raw.githubusercontent.com/ec-to/My-list/main/PROXY.list

## 加速域名

https://v6.gh-proxy.org/  （优先）

https://ghproxy.net/ 

https://mirror.ghproxy.com/ 

https://gh-proxy.com/ 

https://ghproxy.org/


## 代码示例

规则集配置
```
  在线直连: # 在线自定义直连域名列表
    <<: *Classical
    path: ./etc/在线直连.list  
    url: "https://v6.gh-proxy.org/https://raw.githubusercontent.com/ec-to/My-list/main/DIRECT.list"
  在线代理: # 在线自定义直连域名列表
    <<: *Classical
    path: ./etc/在线代理.list  
    url: "https://v6.gh-proxy.org/https://raw.githubusercontent.com/ec-to/My-list/main/PROXY.list"
```

路由配置
```
  - RULE-SET,本地直连,国内直连名单
  - RULE-SET,在线直连,国内直连名单
  - RULE-SET,本地代理,海外代理名单
  - RULE-SET,在线代理,海外代理名单
```
