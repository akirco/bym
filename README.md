# bym

一个简单的 Bash TUI 音乐播放器，基于 yt-dlp + mpv。

## 功能

- YouTube/Bilibili 搜索并播放音乐
- 本地音乐播放（`~/Music` 目录）
- TUI 界面，支持键盘操作
- 进度条显示与控制

## 依赖

- `yt-dlp`
- `mpv`
- `socat`

## 操作

| 按键    | 功能                          |
| ------- | ----------------------------- |
| `↑/↓`   | 上下选择                      |
| `Enter` | 播放/暂停                     |
| `Space` | 播放/暂停                     |
| `→/←`   | 快进/快退                     |
| `/`     | 搜索                          |
| `s`     | 切换搜索源 (YouTube/Bilibili) |
| `r`     | 加载本地音乐                  |
| `q`     | 退出                          |
| `Esc`   | 退出                          |

## 配置

- 代理：`http://127.0.0.1:7890`
- Bilibili Cookie：`~/.config/bym/cookies.txt`

## 许可证

MIT
