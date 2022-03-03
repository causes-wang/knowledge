# README

## 成立此项目的目的

1. 用于总结梳理知识体系（计算机专业知识，日后可能扩增其他内容的知识），知识库是内部知识库，旨在内部分享使用。
1. 用于记录每个人的进步过程。
    此项目其实类似于习惯进化，最终还是要靠自己自觉，但是有一个目标存在不至于每天颓废下去。
    以我个人的经验来看，学习的痛苦其实很大程度在于决定要学习的那段时间。类似考试一样，开考前感觉就像处刑，考试期间其实痛苦并不这么大。
1. 养成一个健康良好的学习方式，以更好的心态应对未来的就业挑战。

## 知识库维护规则

1. 硬性规则：使用 [markdown](https://www.runoob.com/markdown/md-tutorial.html)、[git](https://learngitbranching.js.org/?locale=zh_CN)。
1. 自己解决冲突，有冲突不要强制 push！
1. 假如你想学习/整理某一些具体的知识到知识库，建议自己开一个 issue，指定给自己，这样相当于有一个目标一直在催你。
1. 尽量不要直接 push 到 master 分支，自己新开分支，然后提交一个合并请求（Merge Request、MR）来合并。

    注意提交到远端时，一定要在 commit 中写清楚自己这次做了什么，而且注意最好只留下一个 commit（使用 `git commit --amend`）方便查看。
    同时注意，假如有对应的 issue，在 MR 的描述中贴上对应的 issue 链接。

1. 如果感觉其他人的知识库中有内容不对，提一个 issue，然后 at 对应的人，这样就做到了双方的共同成长。
1. 目前知识库的分层暂时只做计算机专业技能，大概为：

    - `README.md`
    - `docs`：这里是编写文章内容的地方，为的是让笔记通过 CI 自动部署到博客上。
        - `README.md`：VuePress 的说明。
        - `/.vuepress/`：VuePress 的一些配置和公共资源。
        - `/base/*`：存放一些通用技能，例如《计算机网络》、《计算机组成原理》、《数据结构》、《设计模式》等。
        - `/frontend/*`：前端专业技能。
        - `/backend/*`：后端专业技能。
        - `/bigdata/*`：大数据专业技能。
    - `package.json`：VuePress 的配置。

    如果之后知识库目录变动，会 at 所有人，并且更改 `README.md` 文件的说明，你可以首先在本地运行一下，看看内容是不是自己想要的：

    ```yarn
    yarn install
    yarn docs:dev
    ```

    之后进入到 `http://localhost:8080/knowledge/` 查看页面，和远程的没有任何区别。

1. [知识库博客地址](http://causes.cloud/)。
1. 其他[注意事项](http://causes.cloud/about)。
