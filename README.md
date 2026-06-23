# LeapTool2 Updates

这是 LeapTool2 的公开更新分发仓库，只放在线更新需要的公开产物。

本仓库可以公开，不应该包含源码。

允许放在这里的内容：

- `update.json`
- changelog
- APK / patch 的公开下载地址
- 文件大小和 sha256
- 必要的发布说明

不应该放在这里的内容：

- `app/`、`shared/`、`gradle/` 等源码目录
- release 签名 keystore
- token、密码、私钥
- 用户数据或调试日志

APK 和增量补丁优先上传到 GitHub/Gitee Release 附件，不建议长期直接提交进 Git 历史。

客户端更新入口：

```text
update.json
```

建议客户端优先读取 Gitee 公开地址，失败后回退 GitHub 公开地址。
