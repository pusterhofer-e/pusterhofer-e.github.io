---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

## How to install Jekyll on Mac:

### 1. Update ruby:
```brew install ruby```

### 2. Update session and check if it worked:
```source ~/.zshrc```
```hash -r```
```ruby --version```
```which -a ruby```

### 3. Update RubyGems:
```gem update --system```

### 4. Install Jeckyll and Bundler:
```gem install jekyll bundler```
```gem env home```
```echo 'export PATH="/opt/homebrew/lib/ruby.../bin:$PATH"' >> ~/.zshrc```
```source ~/.zshrc```
```hash -r```
```which jekyll```
```jekyll -v```

### 5. Creating first project:
```jekyll new myblog```
```cd myblog```
```bundle exec jekyl serve```


---