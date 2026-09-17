# wslg_custom
WSLG 自用修改版

## 用法

1. 下载 release 包。

2. 在 `$HOME/.wslconfig` 中添加 `systemDistro=<mirror_path>` 配置 ，重启 WSL。

   ```ini
   # 配置示例，改成自己的镜像路径
   [wsl2]
   systemDistro=C:\\wslg_custom\\wslg_v1.0.71_fix1.0.vhd
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

## 开发

如果你想自己修改编译 WSLG，可以参考 [WSLG 构建文档](https://github.com/microsoft/wslg/blob/main/CONTRIBUTING.md#build-instructions)

## 源码

WSLG 基线版本 v1.0.71，基于以下仓库分支构建
- wslg: tags/v1.0.71
- weston : 2318feca
- FreeRDP : c4030980
- pulseaudio : 6f045ff0
- DirectX-Headers-1.0 : tags/v1.608.0
- mesa : tags/mesa-23.1.0

补丁文件 `patch-files/weston/base-2318feca.patch`，在 weston 仓库中使用。

## 参考

- https://github.com/qq1038765585/wslg_title_bar_beautify
