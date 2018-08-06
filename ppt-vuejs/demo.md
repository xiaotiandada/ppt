title: vuejs
speaker: 小田
url: https://github.com/ksky521/nodeppt
transition: slide2
files: /js/demo.js,/css/demo.css

[slide]

# vuejs
## 演讲者：小田

[slide]

# vuejs简介
## Vue 是一套用于构建用户界面的渐进式框架。

----

![img](/img/vue.png)

[slide]

# vuejs开发环境搭建

---

1. 安装nodejs  {:&.zoomIn}

2. 安装vue cli

3. 初始化vue项目并启动


[slide]

# 安装nodejs

下载地址: https://nodejs.org/zh-cn/download/

---

1. 下载对应的 nodejs LTS 安装包 {:&.flexbox.vleft}

2. 检查是否安装成功

``` bash
$ node -v
v10.6.0

$ npm -v
6.1.0

```

[slide]

# 安装vue cli

- Install: {:&.flexbox.vleft}

```bash
npm install -g @vue/cli    # 安装 vue-cli 工具
# OR
yarn global add @vue/cli
```

- Create a project: {:&.flexbox.vleft}

```bash
vue create my-project    # 创建vue项目
# OR
vue ui
```

- 这里是最新版vue-cli3 {:&.flexbox.vleft}

- 目前开发可以采用以前的方式

---

```bash
vue init webpack my-project  # 初始化vue项目
```

这样会集成 webpack 工具,并且工具已经事先配置好了



[slide]

# 初始化vue项目并启动

安装完成之后根据提示操作

```bash
cd my-project # 进入目录

npm install   # 安装依赖

npm run dev   # 启动服务

localhost:8081 # 默认端口
```




[slide]

# vue基础语法


- 模板语法

- 事件和方法

- 属性绑定和双向数据绑定

- 计算属性和侦听器

- Class 与 Style 绑定

- 条件渲染

- 列表渲染

- 组件基础




[slide]

# 使用vue-cli开发简单的todoList



[slide]

----

## [-完-]