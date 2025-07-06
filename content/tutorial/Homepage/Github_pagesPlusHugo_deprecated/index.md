+++
title = "Homepages & Hugo & Academic theme (deprecated version)"
subtitle = "My academic homepage building log (deprecated)"

# Add a summary to display on homepage (optional).
summary = "Build my Github Pages by Hugo based on the theme of Academic."

date = 2019-03-23T21:37:43+08:00
draft = false

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Rongting Huang"]

# Is this a featured post? (true/false)
featured = true

# Tags and categories
# For example, use `tags = []` for no tags, or the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = ["WEB"]
categories = ["Study Record"]

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["deep-learning"]` references 
#   `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
# projects = ["internal-project"]

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
[image]
  # Caption (optional)
  caption = ""

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = ""

+++

Please refer to [Rongting Homepage Setup Guide]({{< relref "tutorial/Homepage/Github_pagesPlusHugo" >}})

# Introduction
做了许多尝试，但是最后发现，安装好**hugo_v53+**之后，只要按照[**Deployment**](https://sourcethemes.com/academic/docs/deployment/)一步一步来就可以。
基于之前win10PC中已有git等.
# Study Process-with learning links
https://pages.github.com/

https://gohugo.io/


https://gohugo.io/getting-started/quick-start/

## Install hugo
选择hugo而不是其他的，有一个原因是适用于windows环境（呜呜因为在服务器权限什么的限制很多比较麻烦，其实可能也不麻烦吧），下载好对应的版本修改环境变量就可以在command中使用。
（不过我都在git bash下使用，方便许多）
windows 下安装好hugo并进行test（这只是test,最后不是这样进行的，只是一个熟悉hugo的过程）
```
C:\Users\rthua>d:
D:\>hugo new site Rongting_Page
D:\>cd Rongting_Page
D:\Rongting_Page>git init
D:\Rongting_Page>git submodule add https://github.com/sourcethemes/academic-kickstart.git themes/academic
D:\Rongting_Page>
echo 'theme = "academic"' >> config.toml
```

## Theme usage-Academic
https://sourcethemes.com/academic/docs/
https://sourcethemes.com/academic/docs/get-started/#themes

- Getting Started
- Create Content
- Deployment
- Features
- Migrate

## Github_pages+Hugo
[Why you should create your personal website with Academic and Hugo](https://georgecushen.com/create-your-website-with-hugo/)
[**Deployment**](https://sourcethemes.com/academic/docs/deployment/)