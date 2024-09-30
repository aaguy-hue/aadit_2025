---
layout: post
title: What tools must be installed?
description: Tools to download for CSA
type: issues
comments: True
---

# How to set up tools?
- Install Git
  - `git clone` the repo
- Install Python
  - Run `pip install -r requirements.txt` in the root folder of this project
    - Installs all required python dependencies
- Install Ruby
  - Install bundler: `gem install bundler`
  - Install required packages: `bundle install`
- Enable WSL feature
  - Install a distro from the Microsoft store
- Install VSCode
  - Install GitLens extension
  - Install Python extension
  - Install Jupyter extension

## How to build project?
Run `make` to begin the server.

Run `make stop` to stop the server.

If you want to want to regenerate the `.md` files generated from the `.ipynb` files, run `make clean`.