# Strike Iron

本仓库是 [Strike Iron] 组织的主存储库, 该组织主要用于记录个人工作/学习/生活的文档集.

## Q&A

### 为什么使用 JetBrains Writerside 写文档?

对于一个懂一点点编程的人来说, 在写文章的工具上会纠结很久, 我也是这样, 用过的工具数不胜数.

现在选择 [JetBrains Writerside] 的原因也很简单, 除了 [JetBrains Writerside]
的官网介绍的功能点满足我现在以及未来的使用需求外, 最重要的原因是我付费了.

没错, 付费了 [JetBrains] 全家桶. 对于一个爱倒腾的人来说, 没理由不倒腾倒腾了.

### 站点为什么不搭建在自己的服务器上, 而是选择使用 GitHub Pages?

简单点说: 穷且志坚.

通俗点说就是穷的连 VPS 都买不起, 但还要有和部署在服务器一样的效果.

穷还都要..., 这可能是我没理由不倒腾倒腾的原因之一?

### 仓库为啥要存储在 strike-iron 组织下?

因为这个组织主要是专门为记录建的, 用组织这个命名空间把不相干的仓库隔离开.

### 仓库名为啥要叫 strike-iron.github.io?

GitHub 上建立网站有一些[规则][GitHub Pages]:

- 以 `<username | organization name>.github.io` 为仓库名构建网站,
  最终的域名是 `https://<username | organization>.github.io`.
- 以其他的名称作为仓库名构建, 则会被构建成普通的项目站点,
  最终的域名是 `https://<username | organization>.github.io/<repository>`.

上述规则说明, 在一个 `username` | `organization` 命名空间下, 只能创建一个 `<username | organization>.github.io` 仓库,
而通过 `URL` 的 `path` 做区分, 则可以创建无数个 `repository`.

仓库命名为 `strike-iron.github.io` 的原因也呼之欲出: 将其作为主站点, 方便在主站点中引入其他仓库创建的子站点.

P.S. 如果不想要 `<username | organization name>.github.io` 这么丑的仓库名字,
可以用 `DNS` 将域名映射到主仓库, 再利用通过域名 + `URL path` 访问其他子站点时会响应 HTTP Status Code: `404` 的特性,
在主仓库中添加的 `404.html` 中获取到 `URL path`, 并配合 `iframe` 来做站点转发;
还可以搭个服务器, 域名配合反向代理做转发等等.

[JetBrains Writerside]: https://www.jetbrains.com/writerside/

[JetBrains]: https://www.jetbrains.com/

[GitHub Pages]: https://pages.github.com/

---

基于 [JetBrains Writerside] 构建.

[Strike Iron]: https://github.com/strike-iron

[JetBrains Writerside]: https://www.jetbrains.com/writerside/
