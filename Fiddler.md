# Fiddler

https://www.cnblogs.com/woaixuexi9999/p/9247705.html

## 工具栏说明

### 短信图标

- 给会话添加备注信息

### Replay

- 重新加载当前会话

### 叉子图标

- 删除回话选项

### Go

- 放行，和断点对应

### Stream

- 响应模式。也即是，当Fiddler拿到远程的response后是缓存起来一次响应给客户端还是以stream的方式直接响应

### Decode

- 解码。有些请求是被编码的，点击这个按钮后可以根据响应的编码格式自动解码 

### Find

- 查找会话

### Save

- 保存会话

### 相机图标

- 截屏

## 会话列表

https://images2018.cnblogs.com/blog/1415062/201806/1415062-20180630153659653-291858709.png

### #

- HTTP Request 顺序
- 图标说明

	- https://images2018.cnblogs.com/blog/1415062/201806/1415062-20180630153923232-386817153.png

### Result

- HTTP 响应状态

### Protocol

- 请求使用的协议

### Host

- 请求地址的域名

### URL

- 请求服务器路径或文件名
- GET的传输参数

### Caching

- 请求的缓存过期时间
- 缓存控制的header值

### Content-Type

- 请求响应类型

### Process

- 发送请求的进程及进程id

## 标签页说明

https://www.cnblogs.com/woaixuexi9999/p/9247705.html

### Statistic

- 查看一些基本性能数据

### Inspectors

- 上面是请求
- 下面是响应

### AutoResponder

- 允许你从本地返回文件，而不用将http request 发送到服务器上
- 实操演示

  https://images2018.cnblogs.com/blog/1415062/201806/1415062-20180630155508506-1868008304.png

	- 把要重定向的这个session会话拖动到AutoResponder界面中
	- 选择要返回的图片
	- 点击save

## 操作实例

### 配置https证书

- 打开 Fiddler  Tool->Fiddler Options->HTTPS 
- 选中 " Decrpt HTTPS traffic ",    Fiddler 就可以截获 HTTPS 请求
- 第一次会弹出证书安装提示，若没有弹出提示，勾选 Actions-> Trust Root Certificate
- 监听的程序访问的 HTTPS 站点使用的是不可信的证书，则请接着把下面的 “Ignore servercertificate errors” 勾选上
- 查看证书，Actions—>open windows certificate Manager 

### 手机端抓包配置

- 打开 Fiddler  Tool->Fiddler Options->Connections 
- fiddler 监听端口默认是 8888，你可以把它设置成任何你想要的端口
- 勾选上 “Allow remote computersto connect” ，允许远程设备连接
- 为了减少干扰，可以去掉 “Act assystem proxy on startup” 

*XMind - Trial Version*