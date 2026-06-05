# Twitter/X 内容发布台公开更新源

这个仓库只用于客户端自动更新。

这里会放：

- `update_manifest.json`
- 无密钥更新包 `TwitterX_Content_Publisher_Update.zip`

这里不会放：

- 私有源码仓库历史
- 真实 `feishu_config.json`
- 飞书应用密钥
- 本地缓存 `posts_cache.csv`
- 批量生成内容 CSV

客户端启动时会读取 `update_manifest.json`。如果发现新版本，会提示用户一键更新。更新时会保留每台电脑自己的飞书配置和本地缓存。
