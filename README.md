
## linkmap使用介绍

作者：
bang大神

地址:
https://gist.github.com/bang590/8f3e9704f1c2661836cd 

### 设置xcode，输入串linkmap文件

XCode -> Project -> Build Settings -> 搜map -> 把Write Link Map File选项设为yes，并指定好linkMap的存储位置

### 编译后，找出本地文件 xx-LinkMap-xx.txt

目录大概位置：~/Library/Developer/Xcode/DerivedData/XXX/Build/Intermediates/XXX.build/Debug-iphoneos/XXX.build/

### 运行命令

node linkmap.js filePath -hl
- filePath为上面linkmap.txt的路径 

输出到本地文件：
node linkmap.js filePath -hl > xxx.txt
