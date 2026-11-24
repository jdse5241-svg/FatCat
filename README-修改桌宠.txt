FatCat · Windows x64 桌宠

直接试用
解压后双击 FatCat.exe。如果旧版还在运行，先从托盘菜单退出旧版。

修改源码
FatCat 基于 chanke17/KuroCat v1.2.1（提交 073bc6d97c76a99db72a0eb103a2bd3245fe1ab1）。
https://github.com/chanke17/KuroCat/tree/v1.2.1

1. 安装 Git，打开命令提示符，获取对应版本的源码。
   git clone --branch v1.2.1 https://github.com/chanke17/KuroCat.git
   cd KuroCat

2. 把压缩包内的 FatCat-Windows-v1.2.1.patch 复制到当前 KuroCat 目录，执行以下命令。
   git apply --check FatCat-Windows-v1.2.1.patch
   git apply FatCat-Windows-v1.2.1.patch

3. 按你的想法修改 windows 目录下的代码或指针资源。

4. 在装有 MSVC C++ 工具和 Windows SDK 的电脑上，打开 x64 Native Tools Command Prompt，
   进入源码根目录并运行 windows\build.bat。构建成功后打开 windows\FatCat.exe。

重新分发时，保留原项目的 MIT LICENSE 和版权声明。
