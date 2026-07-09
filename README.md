# wslg_custom
WSLG 自用修改版

## 用法

1. 下载 release 包。

2. 在 `$HOME/.wslconfig` 中添加 `systemDistro=<mirror_path>` 配置 ，重启 WSL。

   ```ini
   # 配置示例，改成自己的镜像路径
   [wsl2]
   systemDistro=C:\\wslg_custom\\wslg_x11RDP_window_enhance_v1.vhd
   ```

## 改动说明

- X11 窗口边框调整
  - 点击左上角标题栏图标可在浅色/深色间切换，默认为深色。
  - 替换了标题栏的图标。
  - 消除左、下、右三处的白色边框。
- `Alt+F12` 在"标题栏模式"和"无边框模式"之间切换，默认为"标题栏模式"。
- `Alt+F11` 在窗口化和最大化之间切换。
- `Alt+鼠标左键` 拖动调整窗口大小。
- `Alt+鼠标右键` 拖动移动窗口。
- 支持从 Windows 剪贴板粘贴图片到 WSLg 窗口。

## 参考

- https://github.com/qq1038765585/wslg_title_bar_beautify
