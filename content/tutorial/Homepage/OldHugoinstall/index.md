+++
title = "Manually Download and Install Hugo 0.71"
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

1. **Download the macOS binary** from the [official Hugo releases page](https://github.com/gohugoio/hugo/releases/tag/v0.71.0):
    - [Hugo v0.71.0 (Extended) for macOS 64-bit](https://github.com/gohugoio/hugo/releases/download/v0.71.0/hugo_extended_0.71.0_macOS-64bit.tar.gz)
    - [Hugo v0.71.0 (Standard) for macOS 64-bit](https://github.com/gohugoio/hugo/releases/download/v0.71.0/hugo_0.71.0_macOS-64bit.tar.gz)
2. **Extract the download:**
    
    ```
    tar -xvzf hugo_extended_0.71.0_macOS-64bit.tar.gz
    
    ```
    
3. **Move the hugo binary to your PATH:**
    
    ```
    sudo mv hugo /usr/local/bin/hugo-0.71
    
    ```
    
4. **(Optional) Alias the binary:**
    
    Add to your `~/.zshrc` or `~/.bash_profile`:
    
    ```
    alias hugo71="/usr/local/bin/hugo-0.71"
    
    ```
    
    Then reload your shell:
    
    ```
    source ~/.zshrc
    
    ```
    
5. **Run the older Hugo:**
    
    ```
    hugo71 version
    
    ```
    
    You should see:
    
    ```
    Hugo Static Site Generator v0.71.0/extended ...
    
    ```


---

## **Summary**

- **Yes, you can downgrade the hugo if you installed higher hugo.**
- **Manual download** is the most reliable for old versions.
- Use an **alias** so you can run both old and new Hugos without conflict.

---
