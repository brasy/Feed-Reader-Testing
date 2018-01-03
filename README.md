# 基于 web 的用来读取 rss 源的应用
这个项目让开发者意识到测试的价值。
工具http://jasmine.github.io)包含在了项目之中。

## 项目目的
测试是开发过程中一个很重要的部分，很多组织把一个标准的开发过程称之为测试驱动开发。
测试是我们要掌握的一项重要技能。

## 我学到内容
查阅jasmine资料，使用Jasmine 来给已经写好的应用编写一定数量的测用例。
这些测试用例既要测试深层次的商业逻辑，也要测试时间处理和 DOM 操作。

## 这对我的职业有何帮助？
* 编写测试需要分析应用中诸如 html , css , javascript 之类的各个层面。
* 阅读新的项目代码的能力尤其重要
* 长期编写测试会让你拥有不需要手动编写测试去测试所有的功能, 就能快速分析新的代码是否和已知代码冲突的能力。

## 完成这个项目 Feed-Reader-Testing_zh
1. 听完 javascript Testing [课程](https://www.udacity.com/course/ud549)
2. 下载[必要的项目资源](http://github.com/udacity/frontend-nanodegree-feedreader))
3. 浏览器里面查看一下应用的功能, vscode 查看项目的文件
```HTMl (**./index.html**)  CSS (**./css/style.css**)  JavaScript (**./js/app.js**) ``` 
Jasmine spec  `**./jasmine/spec/feedreader.js** `

4. 下载依赖文件 `jquery.min.js, handlebars.min.js, google font`
5. 目标修改文件为 `**./js/app.js , feedreader.js `, 测试第一个测试集
6. 编辑`allFeeds` 为空数组, 测试第一个测试
7. 编写第二个测试遍历 allFeeds 对象里面的所有的源来保证有链接字段而且链接不是空的，修改app.js，`allFeeds`添加空元素并测试。
8. 编写第三个测试遍历 allFeeds 对象里面的所有的源来保证有名字字段而且不是空的。修改app.js,`allFeeds`添加空元素并测试。

9. 编写第二个测试集 `"The Manu"`
10. 第一个测试用例保证菜单元素默认是隐藏的。根据app.js可知,toggleClass添加删除html标签的class，能改变隐藏、显示菜单。
11. 第二个测试用例保证当菜单图标被点击的时候菜单会切换可见状态,再次点击的时候隐藏。

12. 编写第三个测试集 `"Initial Entries"` 
13. 第一个测试用例保证 `loadFeed` 函数被调用而且工作正常, 期望`.feed`容器元素里面至少有一个`.entry`的元素.
    参考app.js `init()`. 并使用异步测试方法，保证测试运行前源已经被加载.
14. 编写第四个测试集 `"New Feed Selection"`
15. 第一个测试用例保证当用 `loadFeed` 函数加载一个新源的时候内容会改变.
    并使用异步测试方法，保证测试运行前源已经被加载。

16. 写 README.md 文件来详细说明运行应用的步骤。
