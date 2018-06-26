# python-webapp
一个基于python开发的web应用，用于匹配筛选两个字符串中的相同字符。
采用Flask框架，提供用户输入，同时将输出实时显示在页面上，并将日志数据存储在数据库。
在这个应用的实现过程中，我们采用DB-API连接数据库，通过with语句挂接上下文管理器实现数据库的连接和清理工作，做到最大程度上的复用。
通过函数修饰符实现对某些URL的访问限制，并且添加了异常处理机制，使得我们的web应用遇到问题时，在后台静默的处理异常，而不是出现不友好的页面。