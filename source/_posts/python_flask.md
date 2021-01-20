---
title: python flask
date: 2021-01-20 12:39:39
tags: python
category: Code
---

## python flask

<!-- more -->
### 安装
安装Flask时会自动安装如下包  
**Werkzeug** 用于实现 WSGI ，应用和服务之间的标准 Python 接口。  
**Jinja** 用于渲染页面的模板语言。  
**MarkupSafe** 与 Jinja 共用，在渲染页面时用于避免不可信的输入，防止注入攻击。  
**ItsDangerous** 保证数据完整性的安全标志数据，用于保护 Flask 的 session cookie。  
**Click** 是一个命令行应用的框架。用于提供 flask 命令，并允许添加自定义 管理命令。  

### 依赖
**Blinker** 为信号提供支持。  
**SimpleJSON** 是一个快速的 JSON 实现，兼容 Python’s json 模块。如果安装了这个软件，那么会优先使用这个软件来进行 JSON 操作。  
**python-dotenv** 当运行 flask 命令时为通过 dotenv 设置环境变量提供支持。  
**Watchdog** 为开发服务器提供快速高效的重载。  

### 安装
在项目文件夹下创建虚拟环境  
`$ python3 -m venv venv`  
激活虚拟环境  
`$ . venv/bin/activate`

安装  
```
$ pip install blinker
$ pip install simplejson
$ pip install python-dotenv
$ pip install watchdog
$ pip install Flask
```

使用基础  
写好代码之后先在环境变量指定文件  
```
$ export FLASK_APP=hello.py
$ flask run
```  

调试模式，服务器会在修改代码之后自动重启  
`$ export FLASK_ENV=development`  
这样可以实现以下功能：  
1. 激活调试器。
2. 激活自动重载。
3. 打开 Flask 应用的调试模式。  
还可以通过导出 `FLASK_DEBUG=1` 来单独控制调试模式的开关。  

<font color=red size=5>不要在生产环境下使用调试器！！！</font>