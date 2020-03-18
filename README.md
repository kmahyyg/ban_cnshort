# ban_cnshort
Ban China Short Video Websites。 屏蔽中国的主流短视频网站。

# 帮助完善

请将域名提交到 [Issue #1](https://github.com/kmahyyg/ban_cnshort/issues/1) 或 开启一个新的 Pull Request。

# 覆盖

目前覆盖了：
抖音、头条、西化、梨视频、秒拍、快手、趣拍、美拍、火山小视频、二更视频、百度

# 使用办法

直接复制到路由器 hosts.

支持 DPI 和 行为管控 的路由器请直接控制对应域名。（例如： Gocloud 高恪固件）

# Dnsmasq 用户

请直接将本 Repo 下的 dnsmasq-localhost.conf 添加到下述文件中即可：`/etc/NetworkManager/dnsmasq.d/dnsmasq-localhost.conf`

## 华硕路由器梅林固件使用方法

ssh登入路由器后，在/jffs/configs目录下新建一个dnsmasq.conf.add文件，将本Repo下的dnsmasq-localhost.conf内容复制进去，保存。
然后输入service restart_dnsmasq命令，看到Done.了之后就OK了。
