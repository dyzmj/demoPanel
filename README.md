# demoPanel

混淆个人专属 BPB 代码。详细搭建过程参见 [demoPanel](https://www.haoyep.com/posts/cf-bpb-vpn/)。

BPB在[Release v3.2.3](https://github.com/bia-pain-bache/BPB-Worker-Panel/releases/tag/v3.2.3)中指出，直接未经混淆的代码很容易让Cloudflare检测到并报1101错误。因此本文不再更新混淆脚本。实际上，已经成功部署的BPB脚本也一直是可以正常运行的，没必要跟进最新版本。如果确实想自己混淆，可以拉BPB库，按照[workflows](https://github.com/bia-pain-bache/BPB-Worker-Panel/blob/main/.github/workflows/build.yml)过程编译混淆。

>1 - 由于代码暴露给Cloudflare（将来可能出现1101错误），没有任何混淆文件从发布版本中永远删除。所以请选择一个之前没有返回过1101的Cloudflare账户。
>2 - 如果你正在使用工人部署和得到1101，请删除工人和更改工人和页面>子域从右手工具栏。应用新的子域需要几分钟的时间。
