# online-resume

[English](README.md) | [简体中文](README_CN.md)

---

基于Hugo的简历模板，可以使用Markdown来写自己的简历内容，然后渲染成HTML并且可以打印成PDF格式的文件。

特性：

+ 上手简单，容易编辑，可以隐藏
+ 使用Hugo + Markdown技术栈
+ 多语言支持
+ 自定义主题颜色
+ 简历内容模块化
+ 响应式设计
+ 打印格式友好

## 起步

### 使用

+ 创建Hugo网站，以git子模块的方式添加主题。
  + `hugo new site resume`
  + `cd resume && git init`
  + `git submodule add git@github.com:tarrex/hugo-theme-online-resume.git themes/online-resume`

+ 复制`config.yml`和`data.yml`两个文件到新网站。

  + `cp themes/online-resume/exampleSite/config.yml .`
  + `cp themes/online-resume/exampleSite/data/data.yml ./data`

+ 编辑`data/data.yml`文件来更新简历。

+ 执行`hugo server -w`并打开浏览器查看简历。

带照片简历：

![](https://github.com/tarrex/online-resume/raw/master/assets/images/resume1.png "resume with profile photo")

不带照片简历：

![](https://github.com/tarrex/online-resume/raw/master/assets/images/resume2.png "resume without profile photo")

如果想打印简历，直接在浏览器中打印，或者保存为PDF文件。

## 协议

[MIT](https://choosealicense.com/licenses/mit/)

## 其他

+ Jekyll版本: [online-resume](https://github.com/tarrex/online-resume)
