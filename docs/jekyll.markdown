---
layout: default
title: Jekyll on MacOS
permalink: /jekyll/
---

📋 [Assignment](/) | 👾 **[Jekyll](/jekyll/)** | 🌻 [Sunflowers](/sunflowers/)

<br>

## How to install Jekyll on MacOS:

<img src="https://www.galaxus.at/Files/7/6/4/9/9/9/4/6/m4mbp-6_321.png" width="50%" alt="MacBook auf Tisch mit Farn">


<br>

### 1. Update / Install Ruby:
* Install the lastest Ruby version using Homebrew.
```bash
brew install ruby
```

 <br>

### 2. Update session and check if it worked:
* Reload the shell configuration.
```bash
source ~/.zshrc
```
* Clear the command path cache.
```bash
hash -r
```
* Show the installed Ruby version.
```bash
ruby --version
```
* Display all Ruby installations in the PATH.
```bash
which -a ruby
```

<br>

### 3. Update RubyGems:
* Update the RubyGem package manager.
```bash
gem update --system
```

<br>

### 4. Install Jekyll and Bundler:
* Install Jekyll and Bundler.
```bash
gem install jekyll bundler
```
* Show the Ruby gems installation directory.
```bash
gem env home
```
* Add the Ruby gems binary folder to PATH.
```bash
echo 'export PATH="/opt/homebrew/lib/ruby.../bin:$PATH"' >> ~/.zshrc
```
* Reload the shell configuration.
```bash
source ~/.zshrc
```
* Refresh the command cache.
```bash
hash -r
```
* Check where Jekyll is installed.
```bash
which jekyll
```
* Display the installed Jekyll version.
```bash
jekyll -v
```

<br>

### 5. Creating first Jekyll site:
* Create a new Jekyll site.
```bash
jekyll new myblog
```
* Go into the project folder.
```bash
cd myblog
```
* Start the local Jekyll server.
```bash
bundle exec jekyll serve
```

_"myblog" was renamed to "docs"_

<br>
<br>

## How to start Jekyll Server
* Navigate to the site folder.
```bash
cd docs
```
* Run the local develepment server.
```bash
bundle exec jekyll serve
```
* Open provided server address in browser.
 ```bash
 Server address: http://127.0.0.1:4000/
 ```

<br>
<br>

## How to change the theme from minima to cayman
1) Change the layout on every page.
```markdown
layout: default
```
2) Change the theme in _config.yml.
```yml
theme: jekyll-theme-cayman
```
3) Change the theme in Gemfile.
```Gemfile
gem "jekyll-theme-cayman"
```
4) Open project folder in Terminal
```bash
cd docs
```
5) Install the gems listed in the Gemfile
```bash
bundle install
```
6) Remove old generated fildes (_site, cache)
```bash
bundle exec jekyll clean
```
7) Build site and start local server to preview
```bash
bundle exec jekyll serve
```
--- 