# GMT-mini-GUI

## 下载地址
https://github.com/CovMat/GMT-mini-GUI/releases

## 注意事项
使用本工具前请先在您的系统中安装好GMT，版本最低要求为5.4。  
如果想自行编译源代码，请使用Qt 5.13版。已知Qt 5.14版存在bug，无法编译。  
在Mac系统中编译时，除了Qt之外，还必须同时安装xcode 10(xcode 11与Qt 5.13不兼容)。  

## 运行方法
### windows
windows版直接双击运行exe即可
### Linux
首先需要将GMT的运行路径添加到系统的全局环境变量中。假定用户的GMT安装在`/opt/GMT-5.4.5`，请修改`/etc/profile`(使用`su`或`sudo`以管理员权限修改)，加入如下语句以修改环境变量  
```
export GMT5HOME=/opt/GMT-5.4.5
export PATH=${GMT5HOME}/bin:$PATH
export LD_LIBRARY_PATH=${LD_LIBRARY_PATH}:${GMT5HOME}/lib64
```
本工具暂时无法识别`~/.bashrc`这样的用户个人环境变量设置，因此需要设置全局变量。  
设置完成后需要重启电脑生效。之后双击GMT-GUI或AppRun即可运行


## 致谢
感谢@SeisSpath协助编译了Linux版本并进行了大量测试，给出了修改意见。感谢@yjmzj、@seisman、@core-man为软件修改提出的宝贵意见。