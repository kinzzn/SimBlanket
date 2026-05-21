# SimBlanket

音乐相似度对比打分应用。

## 访问地址

https://player-test-aj0.pages.dev

## 发版流程

1. 确保改动在 `index.html` 中完成

2. 从干净目录部署（避免其他文件干扰）：

```bash
mkdir -p /tmp/deploy
cp index.html /tmp/deploy/
npx wrangler pages deploy /tmp/deploy --project-name player-test
```

3. 部署完成后访问上方地址验证

## 注意事项

- Cloudflare Pages 部署必须用干净目录，只包含需要部署的文件，否则可能导致访问异常（如变成文件下载）
- 首次部署后 SSL 证书生效需要 1-2 分钟
- 登录 Cloudflare：`npx wrangler login`
