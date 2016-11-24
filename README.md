# Atom使用纪要

#### 官网地址： [atom.io](https://atom.io)

> 目前(2015/7/29)Atom主题已有725个；Package已有2394

## 目录
- [简单交代背景](#101)
- [常用快捷键](#201)
- [推荐Packages](#301)
- [需慎重使用的Packages](#302)
- [推荐Themes](#401)
- [聊聊Settings](#501)
- [高级篇 - 写个Atom Package](#601)
- [小结](#701)
- [FAQ](#801)

<h3 id="101">简单交代背景</h3>

  ___Atom___ 是 Github 专门为程序员推出的一个跨平台文本编辑器。PS：基于强大的开源项目 [Electron](http://electron.atom.io/)。

  2015/6/25 Atom发布1.0版本，所以趁着工作之余再次好好体验了一把Atom，确实眼前一亮，所以把使用纪要贴出来，方便后来者快速上手。

  至今（2016年7月），我和我所在的团队都在使用Atom撸码，一切都很美好，但是如果哪天我们因为XXX忍不鸟Atom了，我也会及时告知大家的。

> ___PS：劳资是mac，所以windows用户请原谅，照顾不周哈:)___

  [如何评价 Github 发布的文本编辑器 Atom？](http://www.zhihu.com/question/22867204) 知乎这篇文章能让你更好的了解Atom

  [为什么选择Atom](http://atom-china.org/t/atom/59) 来看看官方怎么说吧.

  Atom的简单入门就不科普了，想了解来看看这篇文章吧：[Atom基础使用](http://atom-china.org/t/guan-fang-shou-ce-atom-ji-chu-shi-yong/62)


<h3 id="201">常用快捷键</h3>

> Sublime常用的功能Atom应该都有，比如俺最喜欢的多光标选中和多处选取;

> 和Sublime一样的快捷键俺这里就不再多浪费时间列举了哈；

> 在tree-view的Keybindings里面有非常详细的说明，都是针对Tree操作的

- ```cmd-\``` 显示或隐藏目录树
- ```ctrl-0``` 焦点移到目录树
- ```fn-F2```(选择tree后) 修改文件/文件夹名称
- ```ctrl-shift-M``` Markdown预览，这非常方便俺这种写手
- ```ctrl-alt-b``` 安装[atom-beautify](https://atom.io/packages/atom-beautify)后可使用，格式化代码
- ```ctrl-` ``` 安装[terminal-panel](https://atom.io/packages/terminal-panel)后可使用，调起CLI
- ```ctrl-shift-U``` 调出切换编码选项
- ```cmd-t```或```cmd-p``` 查找文件
- ```alt-cmd-[``` 折叠
- ```alt-cmd-]``` 展开
- ```alt-cmd-shift-{``` 折叠全部
- ```alt-cmd-shift-}``` 展开全部
- ```ctrl-m``` 相应括号之间，html tag之间等跳转
- ```alt-shift-S``` 查看当前可用代码片段

更多快捷键去Settings里面查看，如下图
![](https://raw.githubusercontent.com/nieweidong/learn-atom/master/img/keybindings.png)


<h3 id="301">推荐Packages</h3>

> 很多时候，安装后不能及时就生效，需要重启Atom，这块比较讨厌，略搓:(

- [activate-power-mode](https://atom.io/packages/activate-power-mode) 装逼必备，效果相当赞。PS：最新的版本(0.5.2)有升级性能，卡顿效果小很多了
- [linter](https://atom.io/packages/linter)+[linter-eslint](https://atom.io/packages/linter-eslint) 必备；代码校验工具
- [autocomplete-paths](https://atom.io/packages/autocomplete-paths) 填写路径的时候有Sug提示
- [pigments](https://atom.io/packages/pigments) 让颜色相关的字符，在任何文件下都可以展示对应的高亮，强烈推荐
- [color-picker](https://atom.io/packages/color-picker) 推荐；写CSS时非常方便的调色板
- [docblockr](https://atom.io/packages/docblockr) 注释也优雅，一款用于写注释的插件。支持常见的各种语言
- [emmet](https://atom.io/packages/emmet) 必备；前端开发必备，谁用谁知道，入门地址：[Emmet使用手册](http://www.w3cplus.com/tools/emmet-cheat-sheet.html)
- [file-icons](https://atom.io/packages/file-icons) 推荐：让文件前面有彩色图片，看着非常享受
- [git-plus](https://atom.io/packages/git-plus) Git插件；得先配置邮箱和用户名
- [git-time-machine](https://atom.io/packages/git-time-machine) Git党必备；可以查看当前编辑文件的 ci history，diff 版本间改动；快捷键 ```alt-t```
- [javascript-snippets](https://atom.io/packages/javascript-snippets) 推荐；各种缩写，值得拥有；当然，俺用的最多的是cl命令:)
- [atom-beautify](https://atom.io/packages/atom-beautify) 必备；格式化代码的，快捷键```ctrl-alt-b```
- [esformatter](https://atom.io/packages/esformatter) 统一代码格式用的
- [Minimap](https://atom.io/packages/minimap) 推荐；就是Sublime右边那一竖块，显示缩小版的代码
- [Expose](https://atom.io/packages/expose) 俺的开发习惯：开很多窗口；分多屏。那么问题来了：不能很好的切换对应的 ```tab```，这个插件就是解决 ```Tabs``` 切换的问题，依赖[Minimap](https://atom.io/packages/minimap)和[file-icons](https://atom.io/packages/file-icons)。PS：偶在使用中也遇见过小问题，但 [Issues](https://github.com/mrodalgaard/atom-expose/issues?q=is%3Aissue+is%3Aclosed) 里都解决了，有问题去上面找答案吧:)
- [terminal-panel](https://atom.io/packages/terminal-panel) 不是那么好用的CLI，勉强能凑活
- [vim-mode](https://atom.io/packages/vim-mode) 劳资就是喜欢zuo，所以在Atom上用vim写码:)

<h3 id="302">需慎重使用的Packages</h3>

- [esformatter](https://atom.io/packages/esformatter) 统一代码格式用的。但是，偶尔脑残，经常报些奇葩的错误，不知道最新版有木有改善，但是我们有了更好的格式化代码的办法，使用 [linter](https://atom.io/packages/linter) + [linter-eslint](https://atom.io/packages/linter-eslint)
- [atom-beautify](https://atom.io/packages/atom-beautify) 说说我遇到的情况，如果设置了保存时格式化，当文件比较大的时候，会有很明显的卡顿，所以我这已经不使用这个插件了
- [activate-power-mode](https://atom.io/packages/activate-power-mode) 装逼效果不用多说，但是无论如何优化，基于Browser搞动画所依赖的方面太多了，所以偶尔脑残和卡顿你得习惯:)


<h3 id="401">推荐Themes</h3>

> 其实Atom默认的主题就已经非常小清新、文艺范儿，但前端对美好事务的追求是永不停歇的...

> 提醒一点：Atom的主题是区分 __UI主题和语法主题__

- [seti-syntax](https://atom.io/themes/seti-syntax) 每个文件前的icons是最大亮点
- [atom-material-ui](https://atom.io/themes/atom-material-ui) + [atom-material-syntax](https://atom.io/themes/atom-material-syntax) 颜色正
- [monokai](https://atom.io/themes/monokai) 偶尔想用回Sublime的时候可以用:)
- [Dracula](https://draculatheme.com/atom/) 这个主题不光有 ```Atom```版本的，还有 ```Sublime, Vim, iTerm, Zsh```等等编辑器都存在
- [Lucario](https://github.com/raphamorim/lucario) 暗色系主题，支持 Vim, Atom, Sublime Text, TextMate, Terminal.app, iTerm, Xcode and XTerm


<h3 id="501">聊聊Settings</h3>

> 在这儿聊些很有用的设置

![](https://raw.githubusercontent.com/nieweidong/learn-atom/master/img/tree-view-settings.png)
上图红框中的选项 可以隐藏一些需要忽略的文件

![](https://raw.githubusercontent.com/nieweidong/learn-atom/master/img/tabs-settings.png)
上图红框中的选项 可以实现Sublime选择文件的效果。不勾选时，点击一个文件就是打开文件；勾选后，双击文件才是打开文件

![](https://raw.githubusercontent.com/nieweidong/learn-atom/master/img/esformatter-settings.png)
上图红框中的选项 会再保存时让代码格式化，比如去掉不需要的空格、换行之类

<h3 id="601">高级篇 - 写个Atom Package</h3>
> 原本想写个简单的Package当demo尝试下，但翻看文档发现已写的够清晰，俺也就不浪费时间费这个劲了。

#### 文档地址：[Package: Word Count](https://atom.io/docs/v1.0.3/hacking-atom-package-word-count)


<h3 id="701">小结</h3>

- Sublime用久了也有视觉疲劳，所以偶尔尝试下新编辑器也挺好，毕竟Atom号称“21世纪的编辑器”
- 免费(听说是暂时的)，所以没有Sublime那恶心的弹窗，你懂的
- 扩展能力叼爆，这就是webapp，界面啥都用CSS控制；扩展可以用JS开发，完全可以深度定制打造自己的IDE嘛...
- 邀请测试的那版确实比较慢，启动慢、打开文件慢等等，但是目前确实没有这种感觉，一切都很流畅(非正常情况俺也没试)
- Github发布的编辑器，那么对Git的友好支持不用多说了
- 同样其问题也有不少，比如用着用着Tree的颜色就变了，然后重新启动就好使了；比如安装个新包还需要重启编辑器等等...这都是比较糟糕的体验，在这里期望Atom能越做越好吧...
- Atom有中文社区：[AtomChina](http://atom-china.org/)
- 双手附上官网文档地址，请多关注：[Atom Documentation](https://atom.io/docs/v1.0.3/getting-started-why-atom)


<h3 id="801">FAQ</h3>

- 觉得卡？建议升级最新的 ```Atom```。如果还没有好转，建议查询下主题和包是否过旧或者有影响。如果各种尝试之后还是无解，那么还是用回 ```Sublime``` 吧...
- [markdown-preview](https://atom.io/packages/markdown-preview) 的快捷键为 ```ctrl-shift-m```，如果不好使那么需要配置一下 ```keymap.cson```，配好之后快捷键就可以正常使用啦，详情: [Keyboard Shortcut overriding](https://discuss.atom.io/t/keyboard-shortcut-overriding-emmet-and-markdown-preview/14113/8)
- 某些插件安装了为什么没有及时生效？答：重启大法
- 写 ```.md``` 文件的时候会莫名的卡，文件其实没有多大，原因未知


---

如发现有趣的内容也会陆续更新补上，更欢迎伙伴们pull request，git地址：[learn-atom](https://github.com/nieweidong/learn-atom)
