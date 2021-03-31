# online-resume

[English](README.md) | [简体中文](README_CN.md)

---

Yet another resume template based on Hugo. You can write your resume using Markdown, it will be rendered into HTML and can be printed as PDF file.

Features:

+ Easy to use/edit/hide
+ Hugo + Markdown
+ Multiple languages
+ Multiple skins
+ Content modular
+ Responsive display
+ Print-friendly

## Getting Started

### Usage

+ Create new hugo site and add the theme by git submodule.
  + `hugo new site resume`
  + `cd resume && git init`
  + `git submodule add git@github.com:tarrex/hugo-theme-online-resume.git themes/online-resume`

+ Copy `config.yml` and `data.yml` files.

  + `cp themes/online-resume/exampleSite/config.yml .`
  + `cp themes/online-resume/exampleSite/data/data.yml ./data`

+ Edit `data/data.yml` file to update your resume.

+ use `hugo server -w` and open in browser to check the resume.

with profile photo:

![](images/resume1.png "resume with profile photo")

without profile photo:

![](images/resume2.png "resume without profile photo")

If you want to print your resume, just press the shortcut of print. Also, it can be saved as a PDF file.

## License

[MIT](https://choosealicense.com/licenses/mit/)

## Others

+ Jekyll Version: [online-resume](https://github.com/tarrex/online-resume)
