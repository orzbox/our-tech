## GitHub 使用心得————那些年踩过的坑

> 作者：[ScarboroughCoral](https://github.com/ScarboroughCoral)


### # 问题与解答（FAQ）

#### 提交 `Pull Request` 时有太多 commit ，仓库主人需要 `squash` 或者直接弃用你的代码。

这是一个比较恶心的地方，我感触颇深。最近在参与一项开源项目。第一次提交就包含很多个 commit ，项目组长出于项目的可维护性就不得不 squash 了。`squash` 是一个 git 命令，作用就是将多个 commit 看做一个 commit 来处理。不过老是让别人处理你的提交并不是很好。

* Q：如何解决太多 commit 问题

* A：强调分支的重要性。你可能会看到过一些文章来解释为什么 `master` 分支一旦创建就不允许对其内容进行修改之类的问题了。的确是这样，master 分支是你的开源项目的主分支，这个分支的历史提交是否清晰对项目的可维护性有着关键作用。一般来说，对于 `master` 分支最新记录中出现的 bug，需要新建分支 `bugName` 来修复  bug ，待 bug 修复完成后，只需要将 `bugName` 分支合并到 `master` 分支就可以了，因为 `master` 分支只有合并一条修复bug记录，所以显得历史提交格外清晰。**一句话，你可以在贡献代码前先更新仓库，然后新建分支并在此新分支上贡献你的代码，最终合并到 master 分支，然后就可以提交你的 `pull request` 了。**
