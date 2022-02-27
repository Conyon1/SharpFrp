# SharpFrp

使用方法：将配置文件hex编码命令行调用即可

![image-20220226135225039](./image-20220226135225039.png)

环境配置：

- TDM-GCC
- golang 1.17.3_amd64
- Visual Studio 2022

Windows编译（TDM-GCC GO1.17.3_amd64 Vs2022）：

1. 运行builddll.bat
2. 打开.sln文件进行编译

实现原理：

通过修改FRP源代码将exe修改成dll文件（./Costura64/main.dll），通过csharp调用。

注意：本项目没有对frp进行任何流量加密的修改，在实际使用中需要自己去修改并重新编译。
