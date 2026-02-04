# 参与 OpenRocket 贡献 🚀
嗨，感谢你对 OpenRocket 感兴趣！😊

我将引导你参与 OpenRocket 的贡献，无论是作为开发者、测试者还是任何其他形式的帮助，都能让 OpenRocket 更上一层楼——*玩笑而已*。

在继续之前：时间就是金钱，为节省时间，请习惯将 OpenRocket 简写为 _OR_。

#### 目录
[测试](#测试)
* [报告缺陷](#报告缺陷)
* [提出新功能建议](#提出新功能建议)

[开发](#开发)
* [提交规范](#提交规范)
* [拉取请求](#拉取请求)

[翻译](#翻译)

[文档](#文档)

[其他事项](#其他事项)

## 测试
OpenRocket 并不完美，但我们需要人们去发现并清晰记录所有不完美之处。测试者的工作是发现缺陷、提出新功能需求并测试软件更新。📝

### 报告缺陷
提交新 issue 时请尽量简洁。给出简短且恰当的标题，最好在开头加入“[Bug]”标签以表明是缺陷。

在描述问题时，以下要素很重要：
* 说明你期望 OpenRocket 的行为，以及实际行为
* 详细列出你（重新）复现问题的步骤
* 提供你的操作系统信息（例如“macOS Monterey version 12.1”）以及你使用的 OpenRocket 版本（例如“最新不稳定分支”）
* 如适用，请附上 OpenRocket 抛出的异常 Bug Report（最好单独作为 .txt 文件）

提供额外信息（如截图、录屏、触发错误的 .ork 文件等）有助于更快理解并解决问题。

### 提出新功能建议
如果你希望 OR 增加某项新功能，请为其创建一个新 issue。建议在标题中加入“[Feature Request]”标签。

请详细说明新功能：
* 你希望 OR 具备哪些新行为
* 为什么这个新功能重要

## 开发
请阅读我们的[开发者指南](https://openrocket.readthedocs.io/en/latest/dev_guide/development_overview.html)。如果你仍有关于环境配置、从哪些 issue 开始等问题，请不要犹豫，通过 [Slack](https://join.slack.com/t/openrocket/shared_invite/zt-dh0wtpc4-WmkSK1ysqAOqHa6eFN7zgA) 联系我们。

一开始开发 OpenRocket 可能令人望而生畏，但只要把 Google、IDE 的搜索与调试功能以及其他开发者当作好朋友，你就能轻松创建你的第一个拉取请求。

如果你想处理某个 issue，应先表明你想处理它。可以在 issue 下评论类似“我想处理这个 issue”。这样可确保同一问题不会被多人同时处理。

### 提交规范
请使用**原子提交（atomic commits）**。意思是：不要把 10 个不同问题的修复塞进一个提交里。应拆分成多个小提交，每个提交只修复一个问题/功能。

例如：你修复了一个按钮显示为红色而非蓝色的问题，同时发现其他地方有个错别字。那就把按钮修复放在一个提交里并取一个合适的名字，把错别字修复放在另一个提交里。原子提交能让代码审查更容易。

提交信息也要**有意义**。一个好的提交命名习惯是：`[#{你要修复的 GitHub issue 编号}] {提交主题}`。

以修复 issue #123 的红色按钮为例：`[#123] Display red button as blue`。提及“#123”也会自动将你的拉取请求链接到对应 issue。提交主题应简短精准。另外，除了提交主题，附上 git 提交信息正文来解释为什么以及如何进行此次提交也非常有用。

### 拉取请求
很好，你已经深入代码库，找到了那条让你头疼的坏代码并修复了它。现在是时候将代码推送并从你自己的仓库向官方仓库创建一个拉取请求（PR）了。作为 PR 文本，建议使用以下结构：

1. 简要说明你要解决的 issue，例如“此 PR 解决了 #123，其中按钮显示为红色而非蓝色”
2. 说明根本原因，例如“问题在于 Java Swing 默认将按钮显示为红色”
3. 说明你如何修复，例如“通过覆盖默认按钮颜色改为蓝色来修复”

你可以参考示例 PR [#979](https://github.com/openrocket/openrocket/pull/979)。

## 翻译
OpenRocket 软件与终端用户文档站点都是多语言的。译者的工作是维护现有语言，或为未列出的语言新增翻译。在开发过程中，有时会新增英文翻译键，但不会同步翻译到其他语言。因此译者需要检查自己的语言还缺少哪些翻译键。

如何进行翻译可在[开发者指南](https://openrocket.readthedocs.io/en/latest/dev_guide/contributing_to_translations.html)中找到。

## 文档
我们的文档托管在 [ReadTheDocs](https://openrocket.readthedocs.io/en/latest/index.html)。

## 其他事项
如果你有为 OpenRocket 录制教程的好嗓音、作为图形设计师想提升 OR 的设计，或作为销售人员扩大 OR 影响力，那就加入吧！我们非常感谢任何形式的帮助。🙃

---

# Contributing to OpenRocket 🚀
Hi, thank you for your interest in OpenRocket! 😊

I will guide you to contributing to OpenRocket, be it as a developer, tester or any other type of help that will launch - *pun intended* - OpenRocket to the next level.

Before I move on: time is money, so to save you time, get used to how OpenRocket is abbreviated with _OR_.

#### Table Of Contents
[Testing](#testing)
* [Reporting bugs](#reporting-bugs)
* [Suggesting new features](#suggesting-new-features)

[Development](#development)
* [Commit etiquette](#commit-etiquette)
* [Pull requests](#pull-requests)

[Translation](#translation)

[Documentation](#documentation)

[Anything else](#anything-else)

## Testing
OpenRocket is not perfect, but we need people to discover and clearly document all of its imperfections. The job of a tester is to discover bugs, formulate new feature requests and to test out software updates. 📝

### Reporting bugs
Please be very concise when you post a new issue. Give a short and appropriate title, preferably with the '[Bug]'-tag in the beginning to indicate a bug.

When explaining the issue, the following elements are important:
* Explain how you expected OpenRocket to behave, and how it behaved instead
* Go through the different steps that you took to (re)create the issue
* Include information about your operating system (e.g. 'macOS Monterey version 12.1') and which version of OpenRocket you are using (e.g. 'the latest unstable branch')
* If applicable, include a Bug Report (preferably in a separate .txt file) of the exception that OpenRocket threw

Providing extra information like a screenshot, a screen recording, the .ork file that produced an error etc. really help understand and solve the issue more quickly.

### Suggesting new features
If you would like to see a new feature implemented in OR, make a new issue for it. Preferably include the tag '[Feature Request]' in the issue's title.

Explain the new feature in detail:
* Which new behavior would you like OR to have
* Why is this new feature important

## Development
Please read our [Developer's Guide](https://openrocket.readthedocs.io/en/latest/dev_guide/development_overview.html). If you still have questions about how to set up your environment, with which issues you should start etc., then don't be afraid to send us a message on [Slack](https://join.slack.com/t/openrocket/shared_invite/zt-dh0wtpc4-WmkSK1ysqAOqHa6eFN7zgA).

Developing OpenRocket may be daunting at first, but if you keep Google, your IDE's search and debug features, and the other developers as close friends, then you will easily create your first pull request.

If you want to work on a certain issue, you should first communicate that you want to work on that issue. This can be done by commenting on the issue something like 'I would like to work on this issue'. This ensures that no more than one person works on a given issue.

### Commit etiquette
Please make use of **atomic commits**. This means: don't fix 10 different issues and cram them in one commit. Split up commits into smaller commits that fix only one issue/feature.

For example: I fixed an issue where a button was displayed as red instead of blue, but I also found that there was a typo in a text somewhere else. Then put the button-fix in a one commit, give it an appropriate name, and put the typo-fix in another commit. Atomic commits make it much easier for code reviewers to review the code changes.

Also give **useful names** to your commits. A good naming convention of a commit is in the form of '[#{GitHub issue number of the issue you are trying to fix}] {Commit subject}'.

Take the example of fixing the red button from issue #123: '[#123] Display red button as blue'. Mentioning '#123' will also automatically link your pull request to the corresponding issue. The commit subject should be short and precise. It is also very useful to include a git commit message body besides just the commit subject to explain why and how you made that commit.

### Pull requests
Right, you've dug into the codebase, found that one nasty line that caused all your troubles and fixed it. It is now time to push your code and create a pull request of the branch from your own repository to the official repository. As your PR (Pull Request) text, it is good to have the following structure:

1. Explain briefly which issue that you are trying to solve, e.g. 'This PR solves #123 in which buttons were displayed as red instead of blue' 
2. Next explain what the underlying issue was, e.g. 'The problem was that by default Java swing displays buttons as red.' 
3. Next is how you fixed the issue, e.g. 'Fixed it by overriding the default button color to blue' 

You can take a look at example PR [#979](https://github.com/openrocket/openrocket/pull/979).

## Translation
Both the OpenRocket software and the end-user documentation site are multilingual. The job of a translator is to maintain the existing languages, or to make a new translation of an unlisted language. During the development sometimes new translation keys get added in the English language that are not simultaneously translated to other languages. The translator must therefore check which translation keys are still missing in his/her/their language.

How you can make/edit a translation can be found in the [Developer's Guide](https://openrocket.readthedocs.io/en/latest/dev_guide/contributing_to_translations.html).

## Documentation
Our documentation is hosted on [ReadTheDocs](https://openrocket.readthedocs.io/en/latest/index.html).

## Anything else
Do you have the perfect voice for making OpenRocket tutorials, are you a graphical designer that screams to improve OR's design, or are you the salesman that can grow OR's influence? Then go for it! We highly appreciate any help that we get, in any shape or form. 🙃
