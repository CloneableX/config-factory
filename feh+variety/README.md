壁纸更换工具

## 安装

apt install feh
apt install variety

## 配置

一般界面化设置即可，但 variety 的日期显示在有些地区会出现无法正常显示的情况，这是由于 variety 是将日期和时间处理为图片渲染而 ImageMerik 中没有对应文字的图像导致，我通过修改它的时间格式化处理将 clock_filter 替换即可，具体可查看 [variety.conf](./variety.conf) 文件
