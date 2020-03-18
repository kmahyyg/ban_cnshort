# ban_cnshort

Ban China Short Video Websites。 屏蔽中国的主流短视频网站。

# 帮助完善

请将域名提交到 [Issue #1](https://github.com/kmahyyg/ban_cnshort/issues/1) 或 开启一个新的 Pull Request。

# 覆盖

目前 (2018-8) 覆盖了：
抖音、头条、西化、梨视频、秒拍、快手、趣拍、美拍、火山小视频、二更视频、百度

**如有存在没有覆盖的情况，请抓包后提交对应域名的 PR。**

# 使用办法

直接复制到路由器 Hosts 文件.

支持 DPI 和 行为管控 的路由器请直接控制对应域名。（例如： Gocloud 高恪固件）

# Dnsmasq 用户

请直接将本 Repo 下的 `dnsmasq-localhost.conf` 添加到下述文件中即可：`/etc/NetworkManager/dnsmasq.d/dnsmasq-localhost.conf`

## 华硕路由器梅林固件使用方法

SSH 登入路由器后，在 `/jffs/configs` 目录下新建一个 `dnsmasq.conf.add` 文件，将本 Repo 下的 `dnsmasq-localhost.conf` 内容复制进去，保存。
然后输入 `service restart_dnsmasq` 命令，看到 `Done.` 了之后就可以使用了。
