## 安装 Rime

使用 ibus-rime 的方案

apt install ibus-rime

然后安装 rime 中自己需要的中文方案

如果是 Ubuntu 的界面只需要配置 rime 作为输入法的一种即可

如果在 i3 中添加 ~/.xprofile 文件，并配置

```
export GTK_IM_MODULE=ibus
export QT_IM_MODULE=ibus
export XMODIFIERS=@im=ibus
ibus-daemon -drx
```

并在命令行输入 `ibus-setup`，在输入法中添加 rime
