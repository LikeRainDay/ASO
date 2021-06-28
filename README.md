# ASO

> 此项目主要为，IOS端AppStore进行刷榜操作（项目为demo，可以参考逻辑内容）


   
## 项目技术介绍

1. 采用Tweak进行开发
2. 增加了部分私有库，需要自己根据我的makefile中引入的私有库。
3. 打包了PTFTouch的开源触碰（如果有兴趣可以fork）
4. 包含了OC的一些运行时内容
5. html脚本的注入

# 项目环境
* 由开发者反馈，项目中一些theos的依赖没有，因此将我本人的theos环境提交到此项目中`theos.zip`文件就是环境文件。解压后替换你本地的theos
* <del>项目提交是否有问题，导致子目录出现`_`前缀的文件，开发者需要把`_`前缀文件删除后，再编译。</del>
  
# 项目结构

|文件名|描述|功能|
|---|-----|------|
|ASO|AppStore Search optimize 的相关逻辑代码|包含注入点 ，改吗，过验证码，卸载，模拟点击 等|
|layout|一些常用的图标文件|用于美化插件|
|lib|插件需要的一些依赖，我已经将其打成支持各个手机arm的lib||
|Makefile|项目的编译管理||
|Tweak.xm|注入点的声明||
|NGASO.plist|当前此项目的注入程序的进程||
|theos.zip|开发所需要的theos环境||


# 编译实例
```
make clean && make package 
```
![实例图片](https://github.com/houshuai0816/ASO/blob/master/pic/QQ20180609-093818.png)

![实例图片](https://github.com/houshuai0816/ASO/blob/master/pic/QQ20180609-093803.png)


# target
仅供学习使用，一切商用后果与作者无关。
  
 
