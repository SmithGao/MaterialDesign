#TextUtil
2016.3.29
1:此框架仅用于测试 待后续的开发。。。测试

2016.3.30
1:经过本人这几天的所有研究 终于把 GitHub客户端(/web) JitPack(一个自定义的Maven仓库) 轻松的融合到了一起
  现在已经实现了通过github客户端将本地项目文件传导服务器上 在通过jitpack生成库的链接倒入大家自己的开发项目中
  
Android studio：
===================================
 
jitpack：
===================================
 
  
GitHub：
===================================
那些注册登录 创建自己的库这些简单的配置我就不多说了
主要是详细的讲解一下如何配置自己的库(这也是在一个朋友那里看到的 想看原文的朋友可以点击这里 [sloop](https://github.com/GcsSloop) 

    直接上图吧 说的明白
 ![](https://raw.githubusercontent.com/SmithGao/ImageUtil/master/num1.png)

  如图所示点击图示进入Release界面（Release 就是项目的属性设置和版本管理一些基本配置）

  ![](https://github.com/SmithGao/ImageUtil/blob/master/num2.png)

    根据图中标记指示操作
  ![](https://github.com/SmithGao/ImageUtil/blob/master/num3.png)
  
  到这里 一个简单的开源库就已经配置好了 然后点击进入[JitPack](https://jitpack.io/) ,做最后的配置
    ![](https://camo.githubusercontent.com/ee22093c45970b2fc58009ff226b633bc6812ca5/687474703a2f2f7777332e73696e61696d672e636e2f6c617267652f30303558746469326a773166323361303535756f656a3330727330676f6469302e6a7067)
  
![](https://github.com/SmithGao/ImageUtil/blob/master/num6.png)

    总结：1:一个library只能创建一个开源库
          2:在library中 尽量不要有libs
          3:创建的时候 要新建一个项目里面会出现引包重复的冲突 (如果你的是最新版本的AS)
          4:当你的开源库有所改动需要更新的时候,一定要注意在github上的Release配置里更新你的版本,然后在jitpack上重新配置获取新的版本,如果不          更新,在你的项目中则不会改变 
          5:jitpack 可以使用github登录
          6:第一次写文章真的很费劲 但是我相信以后会越来越好的 以后只要写好一个开源库 我会更新的
          7:如果你有什么问题 可以加我的微信联系我 咱们在一起讨论学习 g2215719882  g以后的是我的qq号
