# RandomGreen

[![Build Status](https://github.com/LingEmberMaple/RandomGreen-Template/workflows/ci/badge.svg)](https://github.com/LingEmberMaple/RandomGreen-Template/actions)

自动 GitHub 随机提交。

> a commit a day keeps your girlfriend away.

## 原理

使用 GitHub Actions 的定时任务功能，每隔一段时间自动执行 `git commit`，提交信息为 "a commit a day keeps your girlfriend away"，灵感来自知乎问题[在 GitHub 上保持 365 天全绿是怎样一种体验？](https://www.zhihu.com/question/34043434/answer/57826281)下某匿名用户的回答：

> 曾经保持了 200 多天全绿，但是冷落了女朋友，一直绿到现在。

有关 Github Action 的原理，可查看官方文档 [Github Action 简介](https://docs.github.com/cn/actions/learn-github-actions/introduction-to-github-actions)

## 使用

- 点右上角 **Use this template** 按钮复制本 GitHub 仓库，**:warning: 千万不要 Fork，因为 fork 项目的动态并不会让你变绿 :warning:**
- 根据 [创建 personal access token (classic)](https://docs.github.com/zh/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens#%E5%88%9B%E5%BB%BA-personal-access-token-classic) 勾选 `workflow` 创建一个永久令牌并将令牌复制到剪贴板，根据 [为存储库创建机密](https://docs.github.com/zh/actions/security-guides/using-secrets-in-github-actions#creating-secrets-for-a-repository) 创建一个名为 `PAT` 的机密，机密的值为上一步创建的永久令牌
- 修改 [ci.yml 文件的第 4、5 行](.github/workflows/ci.yml#L4-L5) 去掉 `#` 和 `#` 后一个空格

## Credit

[RandomGreen](https://github.com/LingEmberMaple/RandomGreen-Template) was forked from [auto-green](https://github.com/justjavac/auto-green). Credits to its original author 弥渡[@justjavac](https://github.com/justjavac).

[cron-randomizer](https://github.com/NeddM/cron-randomizer)

## License

[RandomGreen](https://github.com/LingEmberMaple/RandomGreen-Template) is released under the MIT License. See the bundled [LICENSE](./LICENSE) file for details.
