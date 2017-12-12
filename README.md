# 测试项目

* RSS Feeds这是我们的第一个测试用例, 用来测试allFeeds变量
  1. are defined 它用来保证 allFeeds 变量被定义了而且不是空的
  2. links are not empty 测试遍历 allFeeds 对象里面的所有的源来保证有链接字段而且链接不是空的
  3. names not empty 测试遍历 allFeeds 对象里面的所有的源来保证有名字字段而且不是空的。
* The menu这是我们的第二个测试用例, 用来测试菜单情况
  1. 菜单元素默认隐藏 试用例保证菜单元素默认是隐藏的。
  2. 测试用例保证当菜单图标被点击的时候菜单会切换可见状态。这个测试包含两个 expectation ： 当点击图标的时候菜单是否显示，再次点击的时候是否隐藏。
* Initial Entries 这是我们的第三个测试用例, 用来测试默认loadFeed功能是否正常
  1. Async loadFeed 测试保证 loadFeed 函数被调用而且工作正常，即在 .feed 容器元素里面至少有一个 .entry 的元素。
* New Feed Selection 这是我们的第三个用例， 用来测试当切换loadFeed时，获取的内容是否不一样
  1. should change content 测试保证当用 loadFeed 函数加载一个新源的时候内容会真的改变
