## GitHub 使用心得————那些年踩过的坑

> 作者：[ScarboroughCoral](https://github.com/ScarboroughCoral)


### # 问题与解答（FAQ）

#### 提交 `Pull Request` 时有太多 commit ，仓库主人需要 `squash` 或者直接恶心弃用你的代码。

这是一个比较恶心的地方，我感触颇深。最近在参与一项开源项目。第一次提交就包含很多个 commit ，项目组长出于项目的可维护性就不得不 squash 了。`squash` 是一个 git 命令，作用就是将多个 commit 看做一个 commit 来处理。不过老是让别人处理你的提交并不是很好，所以我就换了一种思路来解决。

* Q：如何解决多次 commit 问题

* A：
