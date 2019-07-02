#解决新版sublime没有Package Control和无法用Package Contronl安装插件问题


1.没有Package Control
2.有了Package Control 却无法安装插件
1.没有Package Control
下载了新版（时间轴为2019-4-19 正好我生日 嘻嘻） 然后想装汉化的插件 <百度经验>中说在Preference中的Package Control中下载。
但是我没有啊？？？
于是，便是艰难的开始寻找，办法，过程很辛苦，但方法很简单。
接下来就带大家解决存在问题！！！！！

大家可能都看过去官网download一个Package Control的文件的解决方法，但很不幸，这个网站被祖国母亲的防火墙屏蔽了。于是在这里提供l另一个手动安装的方法。共四步

1.在GitHub上下载Package的文件。下载地址链接: (https://github.com/wbond/sublime_package_control )。
要是不会在GitHub上下载东西，那我就用小皮鞭抽你。
但是，最后还是给出下载操作过程：如图：

然后解压缩到某路径，这个再不会我抽我自己。
2.把刚刚解压缩的文件，剪切或复制到sublime的存放插件的目录下。
依次点击sublime菜单栏>>首选项（preference）>>浏览插件（ Browse Package）。
打开的文件夹就是要复制过来的位置。
并将其重命名为Package Control（不命名为这个，sublime会告诉你需要重命名，不信你试试）

（在此需要说明一下，完成以上操作只会有Package Control 和User 其他的那都是后来下载的，不用有疑惑）
3.在上层目录的 如图路径中 会有这个玩意（看看就行，无须任何操作）

在此之前，这里还会有一个跟他很像的文件，软件自带的**（0KB）**，删不删看软件有没有提醒。

在sublime中 打开preference就会出现package control了
成功！✌

但是真的就能用了么？ 未必，看下一个问题

2.有了Package Control 却无法安装插件
打开Package Control，找到install

过了一会儿后报错了！说什么下载不成功的原因，英文很复杂，我来说明真正原因。

问题原因，和第一个问题一样，被墙了，怎么可能在线下载下来！
但是还没有完全墙，只要把连接改成国内的地址就行。

步骤分2步。一看二改。十分简单！！！
1.看

2.改
把里面的内容改成如下图所示

附代码：
{
“bootstrapped”: true,
“channels”:
[
“https://erhan.in/channel_v3.json”
],
“in_process_packages”:
[
],
“installed_packages”:
[
“ChineseLocalizations”,
“Package Control”
]
}

接下来我们就可以用Package Control来下载东西了
输入你想要的插件比如汉化包 localization （因为我已经安装过了 所以下图中没有这个的提示信息）

安装成功后 就是汉化的 并且我们可以回过头又解决了一个疑问


我想在此大家就应该都明白这是什么意思了，没错 这就是我们新安装的汉化插件。
--------------------- 
作者：爱久弥新的妖刀 
来源：CSDN 
原文：https://blog.csdn.net/weixin_41976775/article/details/89414057 
版权声明：本文为博主原创文章，转载请附上博文链接！
