# SSRF漏洞（Server-Side Request Forgery）

​	SSRF(服务器端请求伪造)：是一种由攻击者构成形成由**服务器**发起请求的一个安全漏洞。

​	<img src="C:\Users\DELL\AppData\Roaming\Typora\typora-user-images\image-20230317161630384.png" alt="image-20230317161630384" style="zoom:50%;" />

  （网络的url没有对来源进行处理，导致访问者可以直接通过服务器来调取内网的相关数据）

​	参考文档：https://www.freebuf.com/vuls/191698.html

## 如何判断是否有SSRF漏洞

<img src="C:\Users\DELL\AppData\Roaming\Typora\typora-user-images\image-20230317165449271.png" alt="image-20230317165449271" style="zoom:50%;" />

使用一些特殊的符号来代替正常的数字，参考网站：github上的SSRF-Testing

一些简单的扫面程序：github上的Gopherus、SSRFmap

## 如何防御SSRF漏洞

​	<img src="C:\Users\DELL\AppData\Roaming\Typora\typora-user-images\image-20230317170144485.png" alt="image-20230317170144485" style="zoom:50%;" />