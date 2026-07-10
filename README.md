# xchina-downloader

## 环境变量

| 变量 | 说明 | 默认值 |
|------|------|--------|
| `CF_COOKIE` | xchina.co 的 Cloudflare cookie | (必填) |
| `TG_API_ID` | Telegram API ID | (必填) |
| `TG_API_HASH` | Telegram API Hash | (必填) |
| `TG_PHONE` | Telegram 手机号 (首次登录需填写) | (二选一) |
| `TG_CHAT_ID` | Telegram 频道 ID | (必填) |
| `TG_SESSION` | gzip+base64 编码的 Telegram session 文件 | (二选一) |
| `LOOP_INTERVAL` | 运行间隔秒数 | 21600 (6h) |
| `TG_INTERVAL` | 视频发送间隔秒数 | 10 |
| `FFMPEG_TIMEOUT` | ffmpeg 下载超时秒数 | 300 |
| `DATA_DIR` | 数据持久化目录 | /data |
| `LOG_LEVEL` | 日志级别 (DEBUG/INFO/WARNING/ERROR) | INFO |
| `VERIFY_SSL` | 是否验证 SSL 证书 (1=开启, 0=关闭) | 1 |
| `MAX_IMAGE_PIXELS` | Pillow 最大像素数限制 | 200000000 |

## 部署方式

### Railway
1. Fork 或 Push 到 GitHub
2. 在 Railway 连接仓库
3. 添加 volume 挂载到 /data
