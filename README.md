# Surge 规则配置文件
_________________

> 规则不是万能的

> 不是所有广告都能简单的依靠规则阻止！

# 简介
本项目基于 [ConnersHua](https://github.com/ConnersHua) 修改而来。

# 规则集
## Reject.list
   - 含基于域名、IP 规则及 HTTP 规则
## Hijacking.list
   - 运营商劫持及臭名昭著的网站和应用
## GlobalMedia.list
   - 海外流媒体服务，如需细化海外流媒体（Youtube、Netflix、PronHub...）策略需排在此规则之前
## Special.list
   - 后续规则修正
## Global.list
   - 海外加速 - Proxy
## China.list
   - 中国直连 - DIRECT
## Apple.list
   - 如无特殊需求可不用加此策略及选择代理，在大部分地区 Apple CDN 可正常工作，使用代理后可能导致「Cannot Connect to iCloud」等问题
_________________

## 引入NextDNS （nextdns.io）

   - 屏蔽广告，跟踪器和恶意网站
   - 获取有关您的Internet流量的深入分析
   - 保护您的隐私并绕过审查制度
   - 保护您的孩子免受成人侵害

> 默认已添加事件脚本network-changed （脚本链接如下，需更改里面 linked IP）

[nextdns.io获取 linked IP](https://github.com/langkhach270389/Scripting/blob/master/Surge/nextdns_linkedip.js)

## 其他

> Youtube 去视频广告会造成以下问题
   - 网页版可能无法正常播放
   - YouTube Premium 用户无法正常播放

> 默认启用，如果无需启用需在「HTTPS 解密(MitM)」的「主机名」列表中禁用 (-) 或删除：

```properties
*.googlevideo.com
```

> ⚠️ 注意：如果开启了代理服务器的「UDP 转发」会失效。


## 感谢


* [@lhie1](https://github.com/lhie1)

* [@ConnersHua](https://github.com/ConnersHua)

* [@chavyleung](https://github.com/chavyleung)

* [@yichahucha](https://github.com/yichahucha)

* [@langkhach](https://github.com/langkhach270389)

* [@Choler](https://github.com/Choler)

* [@Meeta](https://github.com/MeetaGit)

* [@NobyDa](https://github.com/NobyDa)


原文: https://github.com/maicoo-l/Surge


Telegram 频道: https://t.me/who_channel
_________________

## License
> 可以拷贝、转发，但是必须提供原作者信息，同时也不能将本项目用于商业用途。
