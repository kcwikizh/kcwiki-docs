舰娘百科网站使用的是大名鼎鼎的Wikipedia所开发的PHP软件mediawiki制作的

mediawiki这边 是一个php程序 他主要是通过 Extension:Scribunto 来实现Lua的功能的

Lua代码是直接写在wiki页面上的 不会有传统的前后台之分

所有的Lua代码页面会有一个规律 就是 页面的名字是 模块:xxx 开头 或者Module:xxx开头

先上个示范...

https://zh.kcwiki.org/wiki/%E6%A8%A1%E5%9D%97:%E8%88%B0%E5%A8%98%E8%A3%85%E5%A4%87%E5%87%BD%E6%95%B0%E6%94%B9

https://zh.kcwiki.org/wiki/%E6%A8%A1%E5%9D%97:%E8%88%B0%E5%A8%98%E8%A3%85%E5%A4%87%E6%95%B0%E6%8D%AE%E6%94%B9

这两个模块协同起来 一个作为程序 一个作为数据库 接管了wiki里大部分舰娘数值页面的更新

页面上显示的就是Lua源代码   代码编辑其实也是在这个页面进行的



mediawiki使用的Lua应该是基于5.1.5版本的

但是JIT环境是用的wikimedia自己写的LuaSandbox

插件页面的说明是这个 https://www.mediawiki.org/wiki/Extension:Scribunto



然后关于Lua的学习介绍的话...在这里可以找到大部分 是对于wiki上这个版本的Lua而言的

https://www.mediawiki.org/wiki/Extension:Scribunto/Lua\_reference\_manual

Lua语言的官方也有一份Lua的入门指南

官方介绍是这个https://www.lua.org/pil/index.html

写的过程中如果遇到问题的话 可以随时和我说 我来帮你找一下可以解答问题的人

您可以先在wiki上注册一个帐号

https://zh.kcwiki.org/wiki/%E6%96%B0%E6%89%8B%E5%BC%95%E5%AF%BC

然后看下这里如何创建页面之类的说明 创建一个您自己的沙盒 边学边做

比如我的用户名是TrickLin 就可以创建一个Module:TrickLin 这样的

Module的页面 编辑页面的下方会有Lua的console 可以调试的

