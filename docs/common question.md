---
sidebar_position: 6
---

# 常见问题
### 添加天翼云盘时：设备ID不存在，需要二次设备校验
可能是触发了防控，修改密码后重新添加。
### 阿里云盘视频无法播放，下载显示InvalidArgument？
由于referrer的限制，必须使用移动端token
### 视频播放不了？
检查一下是不是编码不支持，一般浏览器不支持h.265（hevc）等编码视频，ac3等编码音频，Safari不支持的更多，建议使用软件播放。
### 获取中转链接？
允许中转之后，复制对应文件直链，将/d改成/p即可。
### 前端文件在哪里？
为方便安装，前端文件与程序打包在一起了，如需修改，请按照从源码运行自行修改编译或填写自定义样式/脚本字段。
### 密码忘了怎么半？
命令行 ./alist-xxxx -password查看。
### 自定义样式/脚本不生效？
是否前后端分开了？自定义部分为后端处理，只有在不分开时才起作用。
### 上传的文件不显示/删除的文件还在/修改根目录不生效？
程序缓存一小时自动失效，后台右上角可手动清除缓存。
### 如何修改监听端口
程序所在目录的data文件夹下的配置文件：`config.json`，修改其中的port值即可。
### webdav浏览器打开显示Internal Server Error？
webdav是给浏览器用的吗？
### 如何更新？
除了在[更新日志](./changelog.md)中标注了与之前不兼容的版本外，皆可以直接替换二进制文件进行更新。
:::tip
如果阅读文档之后，还未解决你的问题，请优先[在Discussions中提问/讨论](https://github.com/Xhofe/alist/discussions/new)或[提issue](https://github.com/Xhofe/alist/issues/new/choose)。
:::