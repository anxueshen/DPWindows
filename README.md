# DPWindows
How to compile dp for windows


## setup

1、First you need install visual studio 2015. I download vs2010 with sp1 from [MSDN I Tell You](https://msdn.itellyou.cn/]).The Visual Studio is commercial software. So you need register by youself. You need to choose the C++ develop environment by install.

2、Second you need to download and install QT 5.11.3. Download form the following [link](http://download.qt.io/new_archive/qt/5.11/5.11.3/). You need install Qt for vs2015 32bit, chats and remote object model.

3、Then you need install gstreamer for windows. You need to download [gstream binrary](https://gstreamer.freedesktop.org/data/pkg/windows/1.0.10/gstreamer-1.0-x86-1.0.10.msi) and [gstream develop](https://gstreamer.freedesktop.org/data/pkg/windows/1.0.10/gstreamer-1.0-devel-x86-1.0.10.msi). You must install this gstream library to C:\gstreamer. Because dp only serach this path to find gstreamer.

## compile and debug

1、First you need to add Gstream Path (C:\gstreamer\1.0\x86\bin) to windows environment Path variable.

2、The dp must have version info for windows rc compiler. So you need first run the generate_version_config.sh(in rootpath/custom). You will generate version_config.sh file with version info.

3、For debug dp in windows, you will also need [windbg tools](https://docs.microsoft.com/zh-cn/windows-hardware/drivers/debugger/debugger-download-tools).
