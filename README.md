# ADM
Apex Dma 方框、辅助瞄准、网页地图分享, 支持Windows和Linux上运行

# 克隆
* 因为有子模块需要用下面命令克隆
* `git clone --recursive https://github.com/bbgsm/ADM.git`
* 不要直接用github的下载zip功能，必须要用上面命令克隆
* 克隆慢的话用代理，自己有代理的话用下面命令配置git代理加速
```shell
git config --global http.proxy 127.0.0.1:1080
git config --global https.proxy 127.0.0.1:1080
```

# 编译
- Windows
  编译环境: Clion + cmake + vs2022,vs2022 首先需要装Windows 10 SDK 开发包和 C/C++ 编译工具配置完成后，在 Clion 的 cmake 配置中选择vs2022编译工具链进行编译
- 直接使用cmake命令编译 :
```shell
mkdir build 
cd build 
cmake -G "Visual Studio 17 2022" ..
cmake.exe --build . --target ADM --config Release
```
- Linux
  编译环境: Clion + cmake + Unix Makefiles, 在 Clion 的 cmake 配置中选择Unix Makefiles编译工具
  <br/> 还需要安装: `sudo apt install libglfw3-dev`
  <br/><span style="color:red">Linux 下编译完成后运行还需要需要把 [vmm.so] [leechcore.so] [leechcore_ft601_driver_linux.so] 三个库文件复制到/usr/lib64/下
  并且用root权限执行<span/>

# 注意
- 辅助瞄准顾名思义就是用来辅助的，如果想完全当自瞄用，就把瞄准速度拉满，拉满不出一天号就没了

# 图片
* 方框
<br> <img src="img/player.jpg" width="800">
* 物品
<br> <img src="img/object.jpg" width="800">
* 网页地图
<br> <img src="img/webMap.jpg" width="300">
# 网页地图功能地址
* 运行ADM后访问下面地址
* http://127.0.0.1:6888/map.html


# 测试环境
#### Windows
- 主机: Windows 11 + CaptainDMA 75T + KmBoxNet
- 副机: Windows 11 
#### Linux
- 主机: Windows 11 + CaptainDMA 75T + KmBoxNet
- 副机: Ubuntu arm64 香橙派5 
- Linux X64 待开发....

# Telegram
* [✈️飞机群](https://t.me/+R3hf2s4ZVF81YmZl)

# 目录
* [cheat 作弊主目录](cheat)
* [blockScreen 黑屏背景(融合器背景专用)](blockScreen)
* [CEPlugin DMA读取整合cheat，方便绘制和CE同时运行在DMA上](CEPlugin)
* [MemTools 内存工具目录](MemTools)
* [render imgui绘制工具](render)
* [webMap 网页功能代码](webMap)
* [libhv C++网络工具](libhv)
* [testGui imgui绘制测试](testGui)
## 关于
* [CheatEngine-DMA(CE DMA内存插件)](https://github.com/Metick/CheatEngine-DMA)
* [libhv(C++网络工具)](https://github.com/ithewei/libhv)
* [imgui(C++绘制)](https://github.com/ocornut/imgui)
* [MemTools(内存读写、dump工具)](https://github.com/bbgsm/MemTools)
* [mINI(ini配置文件工具)](https://github.com/metayeti/mINI.git)