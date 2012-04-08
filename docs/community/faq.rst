.. _faq:

常见问题解答
==========================
这部分文档将会回答关于 Requests 的常见问题。


关于编码后的数据？
Encoded Data?
-------------

Requests 自动解压缩 gzip 压缩的返回数据，并且尽其所能将返回数据解码为 unicode 。
如果你需要的话，你可以直接访问原始的返回数据（甚至是 socket ）。

自定义 User-Agent? 
-------------------

Requests 能使你轻松地用任何别的 HTTP Header 替换 User-Agent 字符串。

为什么不使用 Httplib2？
-----------------

克里斯·亚当斯在 Hacker News 上做出了一番极好的总结

    httplib2 的存在是你应当使用requests的原因之一：作为一个客户端，它是可敬的，
    但是它并没有完备的文档，而且在进行日常的操作时必须要使用太多代码。
    在构建一个现代化的 HTTP 客户端时会遇到一大堆艰难的复杂的底层操作，我感谢
    httplib2 在致力于解决它们时所作的努力，但是实际上只要用 requests 替代就能
    解决。肯尼斯·赖茨非常明确地认为简单的事物应当是易用的，而 httplib2 与其说
    是人们用来构建产品系统的应用，不如说是更为学术化的东西[1]。
   
    小秘密：我在 requests 的作者名单当中，但是我只为这绝妙的项目贡献了很少。
    

    1. http://code.google.com/p/httplib2/issues/detail?id=96 是一个很好的例子:
    一个恼人的bug影响了许多人，曾经有一个 there was a fix available for
    months, which worked great when I applied it in a fork and pounded a couple
    TB of data through it, but it took over a year to make it into trunk and
    even longer to make it onto PyPI where any other project which required "
    httplib2" would get the working version.


对于Python 3的支持？
-----------------

是的！这里有官方支持的Python平台的列表：

* cPython 2.6
* cPython 2.7
* cPython 3.1
* cPython 3.2
* PyPy-c 1.4
* PyPy-c 1.5
* PyPy-c 1.6
* PyPy-c 1.7


支持 Keep-alive?
-------------------

当然么么哒！


支持代理吗？
--------------

答对了！


SSL 身份认证呢?
-----------------

必需的。

