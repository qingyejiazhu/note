<!-- ex_nonav -->
# qingyejiazhu-note

关于里面有些路径跳转失效

路径跳转的具体地址是.md后缀的时候，就是没有在 SUMMARY.md 中列出这些文件；

对于 GitBook 生成的 HTML 来说，是以 SUMMARY.md 中列出来的所有项转化的；

现在不是很常用 GitBook 了，忘记了的话，可以先看GitHub

## 关于排版

> 中文文案排版指北 https://github.com/zq99299/chinese-copywriting-guidelines

中文文案排版指北，中的示例的确可以让文章整体看起来很舒服。所以尽量遵循该排版规则

## 关于 md 文件和图片文件存放问题

由于 Markdown 自身的特性，大部分的编辑器对图片的添加支持都不是很好

每次添加图片都很麻烦，基本上都要经过以下步骤：

1. 截图保存在本地，
2. 复制图片到指定项目目录下，一般为：/assets/image
3. 复制图片路径，写图片语法

对于一些插件来说，支持省略了复制这一步骤，但是对于图片保存的路径有很多不同处理方法。都需要自己手动或则写死一个路径，实在是很麻烦。

GitBook3 以后官网放弃了离线版本的支持，所以就丢掉了离线版的 GitBook 编辑器，而改用使用 Atom 编辑器。

偶遇一个 Atom 中的图片处理插件 markdown-img-paste ；

该插件最方便的在于只要复制图片，然后使用快捷键 ctrl + shift + v 粘贴图片，
就完成了 Markdown 的图片插入，默认保存在当前文件的 assets 中。

这个过程很方便，所以图片保存就近原则，而不是分离。这能节省很多时间；

```
|- chapter
  |- git
    |- assets    # 图片和当前编辑文件在同一目录的assets中
      |- imageA  
      |- imageB
    |- github.md   
```
以上目录存储结构，在使用过程中依赖插件的自动完成工，方便和节省更多的写书时间
