---
layout: page
title: Jekyll on MacOS
permalink: /jekyll/
---

## How to install Jekyll on MacOS:

![MacBook auf Tisch mit Farn](https://www.galaxus.at/Files/7/6/4/9/9/9/4/6/m4mbp-6_321.png)

### 1. Update ruby:
* ```brew install ruby```

### 2. Update session and check if it worked:
* ```source ~/.zshrc```
* ```hash -r```
* ```ruby --version```
* ```which -a ruby```

### 3. Update RubyGems:
* ```gem update --system```

### 4. Install Jekyll and Bundler:
* ```gem install jekyll bundler```
* ```gem env home```
* ```echo 'export PATH="/opt/homebrew/lib/ruby.../bin:$PATH"' >> ~/.zshrc```
* ```source ~/.zshrc```
* ```hash -r```
* ```which jekyll```
* ```jekyll -v```

### 5. Creating first project:
* ```jekyll new myblog```
* ```cd myblog```
* ```bundle exec jekyll serve```

_"myblog" was renamed to "docs"_

## How to start Jekyll Server
* ```cd docs```
* ```bundle exec jekyll serve```

---