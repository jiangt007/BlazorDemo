[理解ASP.NET Core - 全球化&本地化&多语言(Globalization and Localization) - xiaoxiaotank - 博客园 (cnblogs.com)](https://www.cnblogs.com/xiaoxiaotank/p/17466952.html)



注意事项：

1. 资源的路径必须和调用对象的命名空间一致。

![image-20240416101420055](F:\1-Codes\02-ABE\04-Blazor\BlazorLocalization.assets\image-20240416101420055.png)

2. 也可以定义一个Class对象，使用共享资源

   将对象命名空间设为基础命名空间，对应资源文件可以直接放在Resources根目录下。

   
   
   ~~~c#
   @inject IStringLocalizer<ShareResource> _shareTranslator;
   ~~~
   
   
   
   ![image-20240416101555778](F:\1-Codes\02-ABE\04-Blazor\BlazorLocalization.assets\image-20240416101555778.png)

