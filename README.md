# bym

一个简单的 Bash TUI 音乐播放器，基于 yt-dlp + mpv。

## 功能

- YouTube/Bilibili 搜索并播放音乐
- 本地音乐播放（`~/Music` 目录）
- TUI 界面，支持键盘操作
- 进度条显示(控制未实现)
- [ ] 播放歌曲状态跟踪
- [ ] 歌曲更多信息
- [ ] 单曲循环/顺序/随机
- [ ] 音乐下载
- [ ] 哔哩哔哩登录
- [ ] 配置化
- [ ] 数据缓存
- [ ] 播放历史
- [ ] 移除yt-dlp依赖(当前仅youtube)

## 已知问题

- `""`能捕获到回车/空格
- 已设置/dev/null,mpv播放成功后仍输出

## 依赖

- `yt-dlp`
- `mpv`
- `socat`

```sh
# Arch Linux
paru -S yt-dlp mpv socat

# macOS
brew install yt-dlp mpv socat
```

## 安装

```sh
curl -o ~/.local/bin/bym -fsSL https://raw.githubusercontent.com/akirco/bym/refs/heads/main/bym
chmod +x ~/.local/bin/bym
```

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
