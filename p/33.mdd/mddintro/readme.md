

什么是mindevdesk ci.sh
=============

其实在diweb的介绍里就介绍过mindevdesk ci了。还介绍过它与mindevdesk的包含关系，总而言之：

概述
------

mindevdesk和mindevdesk ci.sh是：


```
mindevdesk是包含diweb.sh的源码基础codebase
源码所有的更改在mindevdesk ci.sh端所处的源码处发生，并编译成一个diweb.sh和一些target
之后,diweb.sh -t可以DD这些target
```

高级
------

这里还将介绍mindevdesk ci的源码结构：


mdd使用
-------

mindevdesk自助安装FAQ:

> 最低要求1h512m，推荐4h8g，小内存安装后会使用swap。    
> 如何扩大数据区：默认20G，可以执行/run/initramfs/usr/bin/growpart /dev/vda 2 && resize2fs /dev/vda2扩展此空间到整个剩余可余空间。  
> 如何清除数据：挂载vda2，清除mindevdeskd/changes中的内容，重启即可。  
> 如何以硬盘方式启动：重启编辑grub条目，去掉perch，解包01-core.ldeb到硬盘上的某rootcopy文件夹内。   
> 更多请自行探索。。。  