### 安装 Polybar

```shell
sudo apt-get install cmake cmake-data libcairo2-dev libxcb1-dev libxcb-ewmh-dev libxcb-icccm4-dev libxcb-image0-dev libxcb-randr0-dev libxcb-util0-dev libxcb-xkb-dev pkg-config python3-xcbgen xcb-proto libxcb-xrm-dev i3-wm libasound2-dev libmpdclient-dev libiw-dev libcurl4-openssl-dev libpulse-dev

sudo apt install libxcb-composite0-dev
sudo apt install libjsoncpp-dev
sudo ln -s /usr/include/jsoncpp/json/ /usr/include/json

cd polybar && ./build.sh

polybar example
```
在运行 `polybar example` 之前，需要将 polybar 的创建的默认文件拷贝至 `.config/polybar` 目录下，ubuntu 中的默认配置文件的地址是 `/usr/local/share/doc/polybar/config`。

### i3 默认 status bar

需要为 polybar 创建一个启动的 shell 脚本，具体参照 [launch.sh](./launch.sh)，并在 i3 的配置文件中配置默认启动，并移除 i3 默认的 bar 即可。
