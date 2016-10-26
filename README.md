# TechAccelerator Docs

This repo contains the source files for [http://www.techaccelerator.com/](http://www.techaccelerator.com/).

Documentation is written in Markdown (with options similar to [Github's Flavor](https://help.github.com/articles/github-flavored-markdown/)).

[Jekyll](https://http://jekyllrb.com//) is used to generate static HTML files.

## Usage

On windows:
```shell
C:\> @powershell -NoProfile -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"
C:\> choco install -y ruby atom github 
C:\> powershell
C:\> wget https://rubygems.org/downloads/rubygems-update-2.6.7.gem
C:\> gem install --local rubygems-update-2.6.7.gem
C:\> update_rubygems --no-ri --no-rdoc
C:\> gem uninstall rubygems-update -x
```

Ruby and bundler are required.

```shell
$ bundle install
$ jekyll serve
==    Server address: http://127.0.0.1:4000/
```

### Frontmatter

Each page in the documentation has a header, called frontmatter, this controls where it's displayed and it's title.

e.g.

```
---
title: "Custom Domains"
sort: 40
---
```
# Publishing

Docs are published automatically by Github Pages.
