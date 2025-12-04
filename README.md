# CppPath-
c++环境配置

https://blog.csdn.net/hubing601/article/details/149042159    具体步骤   cursor与trae类似  都是基于vscode开发    
https://www.mingw-w64.org/downloads/      编译工具链    trae可选MinGW-W64-builds
MinGW-W64-builds    对应链接    https://github.com/niXman/mingw-builds-binaries/releases    //githup仓库
具体发行版选择      x86_64-15.2.0-release-posix-seh-ucrt-rt_v13-rev0.7z

我这次选择的编译链    直达下载链接    
https://release-assets.githubusercontent.com/github-production-release-asset/446033510/4bc9f48f-f3da-4434-b514-866e8a6b6db4?sp=r&sv=2018-11-09&sr=b&spr=https&se=2025-12-04T05%3A56%3A40Z&rscd=attachment%3B+filename%3Dx86_64-15.2.0-release-posix-seh-ucrt-rt_v13-rev0.7z&rsct=application%2Foctet-stream&skoid=96c2d410-5711-43a1-aedd-ab1947aa7ab0&sktid=398a6654-997b-47e9-b12b-9515b896b4de&skt=2025-12-04T04%3A56%3A34Z&ske=2025-12-04T05%3A56%3A40Z&sks=b&skv=2018-11-09&sig=5ZgWhqLbHtdhWrvzW9ZZrcb%2F7rcjwzNcll%2BVrtGseZA%3D&jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmVsZWFzZS1hc3NldHMuZ2l0aHVidXNlcmNvbnRlbnQuY29tIiwia2V5Ijoia2V5MSIsImV4cCI6MTc2NDgyNjQ1NSwibmJmIjoxNzY0ODI0NjU1LCJwYXRoIjoicmVsZWFzZWFzc2V0cHJvZHVjdGlvbi5ibG9iLmNvcmUud2luZG93cy5uZXQifQ.1KLqQ9VVjeG_GCSg9ONsmj_tbybqNUoj5rd13lP55vU&response-content-disposition=attachment%3B%20filename%3Dx86_64-15.2.0-release-posix-seh-ucrt-rt_v13-rev0.7z&response-content-type=application%2Foctet-stream







（1）安装 C++ 编译工具链
Windows: 安装 MinGW-w64 或 MSVC（通过 Visual Studio 安装）。
先打开网址
Pre-built Toolchains - mingw-w64
https://www.mingw-w64.org/downloads/


在左侧导航栏选择downloads，选择编译好的安装包，在上图显示的列表框里选择适合自己开发环境的安装包，点击后一般会跳转到github，然后选择合适的版本下载即可。



各版本区别可以通过deepsee大模型查询。

按照后解压，然后将其中的bin文件夹路径加到系统环境变量中。



最后检查下配置是否成功

配置测试
g++ --version
gcc --version
运行项目并下载源码
Linux/macOS: 确保已安装 g++ 或 clang（通过终端命令检查）：
g++ --version  # 或 clang++ --version
运行项目并下载源码
若未安装：
sudo apt install g++        # Ubuntu/Debian
brew install llvm           # macOS (通过 Homebrew)
运行项目并下载源码
（2）配置编译路径（可选）
在 Cursor 设置中指定编译器路径（如果自动检测失败）：
打开设置（Ctrl/Cmd + ,），搜索 C++，填写 Cpp Compiler Path（如 C:\mingw64\bin\g++.exe 或 /usr/bin/g++）。
————————————————
版权声明：本文为CSDN博主「hubing601」的原创文章，遵循CC 4.0 BY-SA版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/hubing601/article/details/149042159
