# gfwlist2AdGuardHome
转换gfwlist到AdGuardHome规则文件，并添加Ali DNS与Dnspod DNS（使用DoH）作为默认DNS。同时对同济域名（*.tongji.edu.cn）使用同济DNS（202.120.190.208），以实现校内网访问。

使用Github Action定期更新文件。

文件地址：https://github.com/SiuKam/gfwlist2AdGuardHome/releases/latest/download/adguardhome_gfwlist.txt

脚本修改自[kpivy8/gfwlist2AdGuardHome](https://github.com/kpivy8/gfwlist2AdGuardHome)


## 脚本依赖
- base64
- curl (https)
- Perl5 v5.10.0+

## 脚本语法
- ./gfwlist2adguardhome.sh -s 8.8.8.8:53
- ./gfwlist2adguardhome.sh -s https://1.0.0.1/dns-query
- ./gfwlist2adguardhome.sh -s tls://1dot1dot1dot1.cloudflare-dns.com
- ./gfwlist2adguardhome.sh -s tcp://1.1.1.1
- ./gfwlist2adguardhome.sh -s tls://1dot1dot1dot1.cloudflare-dns.com
- ./gfwlist2adguardhome.sh -s sdns://AgcAAAAAAAAABzcuNy43LjcAAAovZG5zLXF1ZXJ5

