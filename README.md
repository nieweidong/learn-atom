# Atom使用纪要

#### 官网地址： [atom.io](https://atom.io)

> 目前(2015/7/29)Atom主题已有725个；Package已有2394

### 简单交代背景
  ___Atom___ 是 Github 专门为程序员推出的一个跨平台文本编辑器。

  2015/6/25 Atom发布1.0版本，所以趁着工作之余再次好好体验了一把Atom，确实眼前一亮，所以把使用纪要贴出来，方便后来者快速上手。

> ___PS：劳资是mac，所以windows用户请原谅，照顾不周哈:)___

  [如何评价 Github 发布的文本编辑器 Atom？](http://www.zhihu.com/question/22867204) 知乎这篇文章能让你更好的了解Atom

  [为什么选择Atom](http://atom-china.org/t/atom/59) 来看看官方怎么说吧.

  Atom的简单入口就不科普了，想了解来看看这篇文章吧：[Atom基础使用](http://atom-china.org/t/guan-fang-shou-ce-atom-ji-chu-shi-yong/62)

### 常用快捷键
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

### 推荐Packages
> 很多时候，安装后不能及时就生效，需要重启Atom，这块比较讨厌，略搓:(

- [linter](https://atom.io/packages/linter) 必备；代码校验工具
- [esformatter](https://atom.io/packages/esformatter) 必备；统一代码格式
- [atom-beautify](https://atom.io/packages/atom-beautify) 必备；格式化代码的，快捷键```ctrl-alt-b```
- [minimap](https://atom.io/packages/minimap) 推荐；就是Sublime右边那一竖块，显示缩小版的代码
- [color-picker](https://atom.io/packages/color-picker) 推荐；写CSS时非常方便的调色板
- [autocomplete-paths](https://atom.io/packages/autocomplete-paths) 填写路径的时候有Sug提示
- [vim-mode](https://atom.io/packages/vim-mode) 劳资就是喜欢zuo，所以在Atom上用vim写码:)
- [docblockr](https://atom.io/packages/docblockr) 方便写注释
- [emmet](https://atom.io/packages/emmet) 必备；前端开发必备，谁用谁知道，入门地址：[Emmet使用手册](http://www.w3cplus.com/tools/emmet-cheat-sheet.html)
- [terminal-panel](https://atom.io/packages/terminal-panel) 不是那么好用的CLI，勉强能凑活
- [git-plus](https://atom.io/packages/git-plus) Git插件；得先配置邮箱和用户名
- [javascript-snippets](https://atom.io/packages/javascript-snippets) 推荐；各种缩写，值得拥有；当然，俺用的最多的是cl命令:)
- [file-icons](https://atom.io/packages/file-icons) 推荐：让文件前面有彩色图片，看着非常享受(如果使用着 [seti-ui](https://atom.io/themes/seti-ui) 主题，则体现不了效果哦)


### 推荐Themes
> 其实Atom默认的主题就已经非常小清新、文艺范儿，但前端对美好事务的追求是永不停歇的...

> 提醒一点：Atom的主题是区分 __UI主题和语法主题__

- [seti-ui](https://atom.io/themes/seti-ui) + [seti-syntax](https://atom.io/themes/seti-syntax) 每个文件前的icons是最大亮点
- [atom-material-ui](https://atom.io/themes/atom-material-ui) + [atom-material-syntax](https://atom.io/themes/atom-material-syntax) 颜色正
- [monokai](https://atom.io/themes/monokai) 偶尔想用回Sublime的时候可以用:)

### 聊聊Settings
> 在这儿聊些很有用的设置

![](https://raw.githubusercontent.com/nieweidong/learn-atom/master/img/tree-view-settings.png)
上图红框中的选项 可以隐藏一些需要忽略的文件

![](https://raw.githubusercontent.com/nieweidong/learn-atom/master/img/tabs-settings.png)
上图红框中的选项 可以实现Sublime选择文件的效果。不勾选时，点击一个文件就是打开文件；勾选后，双击文件才是打开文件

![](https://raw.githubusercontent.com/nieweidong/learn-atom/master/img/esformatter-settings.png)
上图红框中的选项 会再保存时让代码格式化，比如去掉不需要的空格、换行之类

### 高级篇 - 写个Atom Package
> 原本想写个简单的Package当demo尝试下，但翻看文档发现已写的够清晰，俺也就不浪费时间费这个劲了。

#### 文档地址：[Package: Word Count](https://atom.io/docs/v1.0.3/hacking-atom-package-word-count)

### 小结
- Sublime用久了也有视觉疲劳，所以偶尔尝试下新编辑器也挺好，毕竟Atom号称“21世纪的编辑器”
- 免费(听说是暂时的)，所以没有Sublime那恶心的弹窗，你懂的
- 扩展能力叼爆，这就是webapp，界面啥都用CSS控制；扩展可以用JS开发，完全可以深度定制打造自己的IDE嘛...
- 邀请测试的那版确实比较慢，启动慢、打开文件慢等等，但是目前确实没有这种感觉，一切都很流畅(非正常情况俺也没试)
- Github发布的编辑器，那么对Git的友好支持不用多说了
- 同样其问题也有不少，比如用着用着Tree的颜色就变了，然后重新就好使了；比如安装个新包还需要重启编辑器等等...这都是比较糟糕的体验，在这里期望Atom能越做越好吧...
- Atom有中文社区：[AtomChina](http://atom-china.org/)
- 双手附上官网文档地址，请多关注：[Atom Documentation](https://atom.io/docs/v1.0.3/getting-started-why-atom)

---

如发现有趣的内容也会陆续更新补上，更欢迎伙伴们pull request，git地址：[learn-atom](https://github.com/nieweidong/learn-atom)
