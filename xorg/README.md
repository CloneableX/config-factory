## 安装

apt install xorg

## 键位配置

输出全键盘键位配置文件

xmodmap -pke > ~/.xmodmap

下面所有键位配置都在 ~/.xmodmap 文件中进行，主要是将 .xmodmap 文件中 keycode 值对应的命令替换即可替换键位功能，键位的 keycode 可使用 `xev` 命令唤起界面拾取

对于重置的键位需要先清除，在重置后添加对新键位的映射，可参考 [.xmodmap](./.xmodmap)
