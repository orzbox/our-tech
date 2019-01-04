## Travis CI 持续集成工具
> 作者：[ScarboroughCoral](https://github.com/ScarboroughCoral)

### 为什么使用 Travis CI？

Travis CI 可以自动化测试和部署，你可能有这种经历：本地开发完毕，打包完毕，复制到服务器，运行。此时发现运行失败。修改 bug ，再次打包，复制到服务器，运行成功。访问时发现接口返回数据格式错误。再次修改bug……

前几天作者就遇到了这种情况，项目是一个 Java 的投票项目，集成了 web 端和 Android 端，后端和 web 前端由作者开发。自己写接口自己对接还是比较有趣的，当然这个过程文档还是必须要写的。

不停地修改、打包、复制是不是很重复、而且很浪费经历。今天分享的这个工具就是一个比较好的解决方案——Travis CI


### Travis CI 能用来干什么？

Travis CI 可以自动化上面这个过程。

个人了解，Travis CI 和 github 集成的比较好，假设你的项目存在于 GitHub 上，Travis CI 就可以使每次代码修改都会自动测试，并且显示结果。你可以建一个仓库来测试，可以参照[阮一峰大神的教程](http://www.ruanyifeng.com/blog/2017/12/travis_ci_tutorial.html)。

- 个人博客

个人博客可以使用 Travis CI，当然是使用 GitHub Pages 部署的博客。比如 Hexo 引擎每次都需要本地生成并发布，而且有可能出错，用了 Travis CI 你就可以在线编辑。

- Travis CI 支持的语言项目

Travis CI 支持一些主流语言，这些语言的项目都可以自动化测试部署。

### Travis CI 怎么用？

你要做的只是写一个 yml 配置文件和一些脚本

不会可以参考：

- [阮一峰大神的教程](http://www.ruanyifeng.com/blog/2017/12/travis_ci_tutorial.html)
- [Hexo 搭建博客实例](https://www.jianshu.com/p/6760159c44aa) 
