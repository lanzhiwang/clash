```bash
$ cat ~/.config/clash/config.yaml
#---------------------------------------------------#
## 配置文件需要放置在 $HOME/.config/clash/*.yaml

## 这份文件是clashX的基础配置文件，请尽量新建配置文件进行修改。
## 端口设置请在 菜单条图标->配置->更多配置 中进行修改

## 如果您不知道如何操作，请参阅 官方Github文档 https://dreamacro.github.io/clash/
#---------------------------------------------------#

mode: rule
log-level: info

proxies:

proxy-groups:

rules:
  - DOMAIN-SUFFIX,google.com,DIRECT
  - DOMAIN-KEYWORD,google,DIRECT
  - DOMAIN,google.com,DIRECT
  - DOMAIN-SUFFIX,ad.com,REJECT
  - GEOIP,CN,DIRECT
  - MATCH,DIRECT
$
```


