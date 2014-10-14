ngx-patchs
==========

所有压缩包基于nginx-1.4.2稳定版本

nginx patch 集合。包括：工作中的修改、第三方patch等。

list：

1、自定义时间格式扩展，在ngx日志中使用。 $time_iso8601。 eg：2014-10-14 17:56:09

2、在error日志中上游服务器返回的500错误。指令：proxy_errors_log_upstream
  
   eg:
   
   proxy_errors_log_upstream http_500 http_404;   //记录上游服务器返回的500 和 404错误
   

3、过载保护。第三方patch

4、后端健康检查。第三方patch

5、xxx_upstream_tries 功能。第三方patch

6、自定义目录存储缓存。（代码开发中）

7、根据业务服务器返回的自定义响应头 X-Extend-Tag （文件内容是否发生更改的MD5值），决定只更新缓存文件头部中的过期时间（减少磁盘IO写）（代码测试中）

