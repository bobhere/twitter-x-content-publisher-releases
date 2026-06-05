# Twitter/X 内容发布台公开更新源

这是 **公开更新仓库**，不是源码仓库。

仓库地址：

```text
https://github.com/bobhere/twitter-x-content-publisher-releases
```

它只负责客户端自动更新。

## 只允许放什么

- `update_manifest.json`
- 无密钥更新包 `TwitterX_Content_Publisher_Update.zip`

## 绝对不要放什么

- 私有源码仓库历史
- 真实 `feishu_config.json`
- 飞书应用密钥
- 飞书 Base token / table_id
- 本地缓存 `posts_cache.csv`
- 批量生成内容 CSV
- 任何客户或业务内容

## 对应的私有源码仓库

```text
https://github.com/bobhere/twitter-x-content-publisher
```

私有源码仓库负责保存源码、构建脚本、文档和开发历史。

## 客户端如何使用

客户端启动时会读取：

```text
https://raw.githubusercontent.com/bobhere/twitter-x-content-publisher-releases/main/update_manifest.json
```

如果发现新版本，会提示用户一键更新。更新时会保留每台电脑自己的飞书配置和本地缓存。

## 当前版本

当前公开更新版本以 `update_manifest.json` 里的 `version` 为准。
