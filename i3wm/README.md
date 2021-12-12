## 安装 i3

apt install i3

如果 i3-wm 和 i3-gaps 是分别安装需要手动将 i3-gaps 安装

## 常用应用

- [alacritty](../alacritty/README.md) (terminal)
- dmenu (start application)
- [xorg](../xorg) (config keyboard)
- [feh + variety](../feh+variety) (wallpaper)
- [picom](https://github.com/yshui/picom) (render terminal)
- [rime](../rime) (chinese input method)
- chromium (browser)
- polybar(../polybar)

## 配置说明

通常 i3 的配置文件位于 ~/.config/i3/config，可参考 [config](./config)

### 初始化启动项

下列应用需要在 i3 启动时运行，通过配置 `exec_always` 命令达成

- xorg
- variety
- picom

### alacritty

将 `bindsym $mod+Return exec` 的应用替换为 alacritty

### xorg

在 xmodmap 配置完键位后需要在 i3 中配置 `exec_always xmodmap ~/.xmodmap`

### 快捷启动浏览器

添加 `bindsym $mod+b exec ${browser}` 可启动自己常用的浏览器，当然你也可以将 `$mod+b` 替换为任何你喜欢的组合键

### 其他快捷键

在 i3 的配置文件中也可以调配其他功能的快捷键，比如移动光标进入窗口的操作等，具体可以根据自己的习惯配置
