# napcat-bulider
基于ntQQ的底层框架
```sequence
Title: QQ机器人运行流程图（咱们的框架eg：AA）
用户A->云服务器: 机器人响应
云服务器->AA框架: 发送请求
note right of AA框架: 逻辑处理
AA框架->napcat: 发送请求
note right of napcat: 此为底层框架
napcat->AA框架: 发送响应
AA框架->云服务器: 传递响应
云服务器->用户A: 发送消息
```



```sequence
Title: AA框架工作
napcat->AA框架:
note left of napcat: 主体由ts和js构成
note right of napcat: 可以通过python,java,\nc++,js等多种语言对接
note right of AA框架: 把napcat的结构\n对象打包逻辑处理
AA框架->云服务器: 部署在此处
AA框架->云服务器: 编写插件的形式
napcat->AA框架: 插件以及功能
```

