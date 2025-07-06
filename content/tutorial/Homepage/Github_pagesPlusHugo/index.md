+++
title = "Homepage Setup Guide"
subtitle = "My academic homepage building log (2025 update)"

# Add a summary to display on homepage (optional).
summary = "Build my Github Pages (Homepages) by Hugo based on the theme of Academic."

date = 2025-07-06T11:27:09-07:00
draft = false

authors = ["Rongting Huang"]

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

Here’s a **comprehensive Markdown tutorial** for setting up and deploying your Hugo homepage using your legacy `academic-kickstart` template. This guide assumes you need **Hugo v0.71** or earlier due to theme compatibility.

---

> **Note:**  
> The `academic-kickstart` template is old and requires **Hugo v0.71 or before**.  
> See: [Rongtingting/academic-kickstart](https://github.com/Rongtingting/academic-kickstart)

---

## 1. Environment Preparation

### 1.1 Install Old Hugo (v0.71 or Earlier)

- Refer to:  
          [Install old hugo 0.71]({{< relref "../OldHugoinstall/" >}})
- For general Hugo installation on macOS, see [Hugo macOS install docs](https://gohugo.io/installation/macos/).




### 1.2 Install Prerequisites

You’ll need:

- **Git** (for cloning and managing repositories)
- **Go** (for some Hugo builds and theme tools)
- **Dart Sass** (for advanced CSS/Sass processing, if required)

**Check your versions:**

```bash
git version
# git version 2.39.5 (Apple Git-154)

go version
# go version go1.24.4 darwin/arm64

hugo71 version
# Hugo Static Site Generator v0.71.0-06150C87/extended darwin/amd64 BuildDate: 2020-05-18T16:13:04Z

hugo version
# (You may also have a newer hugo installed, but use hugo71 for this project)
```

If you need to install Git, Go, or Dart Sass, follow their respective documentation:

- [Git install](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- [Go install](https://go.dev/doc/install)
- [Dart Sass install](https://sass-lang.com/install)

---

## 2. Project Setup & Deployment

### 2.1 Clone Your Academic Kickstart Repo

```bash
git clone https://github.com/Rongtingting/academic-kickstart.git My_homepage
cd My_homepage
```

### 2.2 Initialize Submodules

```bash
git submodule update --init --recursive
```

### 2.3 Prepare the `public` Directory

Remove any existing `public/` folder:

```bash
rm -r public/
```

Then, add your GitHub Pages repo as a submodule to `public/`:

```bash
git submodule add -f -b master https://github.com/Rongtingting/Rongtingting.github.io.git public
```

---

## 3. Local Development

### 3.1 Start the Hugo Server

Run the Hugo development server with **drafts enabled**:

```bash
hugo server -D
# Or, if you have hugo71 installed as a separate binary:
hugo71 server -D
```

- Visit [http://localhost:1313](http://localhost:1313) in your browser to preview your site.

---

## 4. Build and Deploy

### 4.1 Build the Site

```bash
hugo
# Or
hugo71
```

- This generates the site into the `public/` folder, which is connected to your GitHub Pages repository.

### 4.2 Deploy to GitHub Pages

Commit and push your changes in both your main repo and the `public/` submodule:

```bash
# Commit changes in your main site repo
git add .
git commit -m "Update site content"
git push origin master

# Deploy the site by pushing the built files in public/
cd public
git add .
git commit -m "Publish site"
git push origin master
cd ..
```

---

## 5. Additional Resources

- [Rongting-s blog-github sites build.pdf](attachment:ee2921f4-1a20-4147-9443-fd482b9d34cd:Rongting-s_blog-github_sites_build.pdf)
- [Academic Documentation](https://sourcethemes.com/academic/docs/)
- [Official Hugo Documentation](https://gohugo.io/documentation/)

---

## 6. Common Issues

- **Theme errors?**  
  Ensure you’re using `hugo71` (v0.71) since the theme is not compatible with newer Hugo versions.
- **Submodule issues?**  
  Double-check your `public` submodule setup and remote URLs.
- **Build errors with Sass/CSS?**  
  Ensure Dart Sass is installed if you’re customizing styles.

---

## 7. Updating Content

- Edit Markdown files in `content/`.
- Add images and static files to the `static/` directory.
- Customize site configuration in the `config/` folders.

---

# 🎉 Your site is now ready!  
If you have any questions, refer to the resources above or [open an issue](https://github.com/Rongtingting/academic-kickstart/issues) on your repository. If you use the most update version of `academic-kickstart`, please refer to [HugoBlox/theme-academic-cv](https://github.com/HugoBlox/theme-academic-cv).

---

*Happy publishing!*