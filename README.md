Tincube website
=========================

## Production

View website at [https://tincubeth.org/](https://tincubeth.org/)

## Setup in Development

Update index of RBEnv and Ruby build versions. Show list of Ruby versions available. Install latest version of Ruby with RBEnv. Install dependencies for Jekyll static site. Serve the website.
```bash
brew update && brew upgrade rbenv ruby-build
rbenv install -l
rbenv install 2.6.3
rbenv shell 2.6.3
rbenv global 2.6.3
gem install github-pages
gem install bundler -v 1.12
bundle _1.12_ install
bundle exec jekyll serve
```

View the website at http://127.0.0.1:4000/

## How to use
 - Place a image in `/img/portfolio/`
 - Replace `your-email@domain.com` in `_config.yml` with your email address. Refer to [formspree](http://formspree.io/) for more information.
 - Create posts to display your projects. Use the follow as an example:
```txt
---
layout: default
modal-id: 1
date: 2014-07-18
img: code.png
alt: image-alt
project-date: July 2014
client: The Client
category: Web Development
description: The description of the project

---
```

## Demo

Based on [Freelancer bootstrap theme](http://startbootstrap.com/template-overviews/freelancer/)

View this jekyll theme in action [here](https://jeromelachaud.github.io/freelancer-theme)

---------
For more details, read the [documentation](http://jekyllrb.com/)
