# 基于 web 的用来读取 rss 源的应用


## 项目简介

* 测试是开发过程中一个很重要的部分，很多组织把一个标准的开发过程称之为测试驱动开发。
* 测试工具: [Jasmine](http://jasmine.github.io)
* 测试目的: 测试深层次的商业逻辑，也要测试时间处理和 DOM 操作。
* 阅读新的项目代码的能力尤其重要
* 长期编写测试会让你拥有不需要手动编写测试去测试所有的功能, 就能快速分析新的代码是否和已知代码冲突的能力。


## 执行该项目
* 下载该项目, 包含Jasmine.
* 浏览器打开index.html, 正确获取到rss源, 以及内嵌的测试的结果


## 完成这个项目的step
1. 项目资源(http://github.com/udacity/frontend-nanodegree-feedreader))
2. 浏览器查看应用的功能, vscode 查看项目的文件
 ```HTMl (**./index.html**)
 CSS (**./css/style.css**)
 JavaScript (**./js/app.js**)
 ```
 Jasmine spec 
 `**./jasmine/spec/feedreader.js** `

3. 下载依赖文件 `jquery.min.js, handlebars.min.js, google font`
4. 第一个测试集
* 编辑`allFeeds` 为空数组, 测试第一个测试
* 编写第二个测试遍历 allFeeds 对象里面的所有的源来保证有链接字段而且链接不是空的，
* 编写第三个测试遍历 allFeeds 对象里面的所有的源来保证有名字字段而且不是空的。修改app.js,`allFeeds`添加空元素并测试。
* 修改app.js，`allFeeds`添加空元素, 浏览器打开index.html 测试。

5. 第二个测试集 `"The Manu"`
* 第一个测试用例保证菜单元素默认是隐藏的。根据app.js可知,toggleClass添加删除html标签的class，能改变隐藏、显示菜单。
* 第二个测试用例保证当菜单图标被点击的时候菜单会切换可见状态,再次点击的时候隐藏。
* 修改app.js，`allFeeds`添加空元素, 浏览器打开index.html 测试。

6 第三个测试集 `"Initial Entries"` 
* 第一个测试用例保证 `loadFeed` 函数被调用而且工作正常, 期望`.feed`容器元素里面至少有一个`.entry`的元素。
    参考app.js `init()`. 并使用异步测试方法，保证测试运行前源已经被加载。
* 浏览器打开index.html, 查看获取的rss内容

7 第四个测试集 `"New Feed Selection"` 
* 第一个测试用例保证当用 `loadFeed` 函数加载一个新源的时候内容会改变。
    并使用异步测试方法，保证测试运行前源已经被加载。
* 浏览器打开index.html, 查看获取的rss内容

8. 写 README.md 文件来详细说明项目。
