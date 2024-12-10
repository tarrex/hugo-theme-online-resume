<h1 align="center">online-resume</h1>

<p align="center">
  <a href="https://github.com/tarrex/hugo-theme-online-resume/blob/master/LICENSE"><img src="https://img.shields.io/github/license/tarrex/hugo-theme-online-resume?style=flat-square" alt="GitHub License"></a>
  <a href="https://github.com/tarrex/hugo-theme-online-resume/forks"><img src="https://img.shields.io/github/forks/tarrex/hugo-theme-online-resume?style=flat-square" alt="GitHub forks"></a>
  <a href="https://github.com/tarrex/hugo-theme-online-resume/stargazers"><img src="https://img.shields.io/github/stars/tarrex/hugo-theme-online-resume?style=flat-square" alt="GitHub Repo stars"></a>
  <a href="https://tarrex.github.io/online-resume"><img src="https://img.shields.io/website?down_color=red&down_message=down&style=flat-square&up_color=green&up_message=up&url=https%3A%2F%2Ftarrex.github.io%2Fonline-resume" alt="Demo Website"></a>
</p>

<h4 align="center">A minimalist Hugo theme for your resume.</h4>

---

## Live Demo

:point_right: [online-resume][Demo] :point_left:

## Getting Started

Online-Resume is a Hugo theme designed for creating resumes. It enables you to write your resume in YAML file using Markdown and manage it through Git. It can be displayed on a web page and printed as a PDF file directly from the browser.

You can deploy it on various platforms that support Hugo or static files, such as GitHub Pages, Cloudflare Pages, Vercel, Netlify, your own hosting service, and others.

Features:

- User-friendly and easy to deploy.
- Built with Hugo and Markdown.
- Supports multiple languages.
- Customizable theme color and basic styles.
- Modular content design.
- Responsive display.

### Usage

#### Quickly

- Create new hugo site and add the theme through git submodule.
  - `hugo new site resume`
  - `cd resume && git init`
  - `git submodule add git@github.com:tarrex/hugo-theme-online-resume.git themes/online-resume`
- Copy `hugo.yml` and `data.yml` files.
  - `cp themes/online-resume/exampleSite/hugo.yml .`
  - `cp themes/online-resume/exampleSite/data/data.yml ./data`
- Edit `data/data.yml` file directly to update your resume.
- Run `hugo server` and open in browser to preview the resume.

#### Customization

- `data/data.yml`: Edit the resume content.
- `static/images/profile.png`: Your profile photo.
- `config.yml`: Website and theme style settings.

## FAQ

#### How to change the order of the sections in the resume?

There is an `order` option in each section, you can adjust the order by modifying this, the smaller the value the more forward the position.

#### How to hide the specified section in the resume?

If there is no content you want to keep in the section, you can remove it directly. If you want to keep the content, you can set the value of the `show` option of the section to `false`.

#### How to create a resume in other languages?

For example, if you already have an English version resume and you want to create a Chinese version.
  - Copy a `data.yml` file in the `data` folder named `cn.yml` and edit the content.
  - Create `layouts/page` directories through `mkdir -p layouts/page`.
  - Copy `index.html` file in the theme layouts directory to above directory `cp themes/online-resume/layouts/index.html layouts/page/cn.html`
  - Change the `{{- partial "common.html" (dict "Site" .Site "data" .Site.Data.data) }}` in the `cn.html` to `{{- partial "common.html" (dict "Site" .Site "data" .Site.Data.cn) }}`.
  - Create `content` directory in root directory and create a markdown file named `cn.md`, add fromt matter `layout: cn` in `cn.md`.
  - Run `hugo server` and you can preview the Chinese version of your resume by visiting `https://YOUR_RESUME_URL/cn`.

#### How to deploy on other platforms, like cloudflare, vercel?

You can read and follow [Cloudflare Pages][Cloudflare Pages], [Vercel][Vercel] documents.

## Others

- Jekyll Version: [online-resume][Other Version]


[Demo]: https://tarrex.github.io/online-resume
[Cloudflare Pages]: https://developers.cloudflare.com/pages/framework-guides/deploy-a-hugo-site/
[Vercel]: https://vercel.com/guides/deploying-hugo-with-vercel
[Other Version]: https://github.com/tarrex/online-resume
