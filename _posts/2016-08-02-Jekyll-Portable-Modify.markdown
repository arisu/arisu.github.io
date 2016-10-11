---
layout: post
title:  "[Jekyll] 윈도우에서 동작시키기. 3.2.0 -> 3.1.6 (Portable 포함)"
date:   2016-08-02 09:21:40 +0900
categories: jekyll update
---

Jekyll 설치하기
-----------------

### 설치

- [Jekyll을 사용하여 Github에 블로그 만들기](http://yongho1037.tistory.com/599)

- [Jekyll 소개 및 설치 - github로 만들수 있는 블로그](http://djflexible.github.io/blog/github-jekyll.html)

- [Run Jekyll on Windows : A step-by-step guide to setting up Jekyll on Windows by @juthilo.](http://jekyll-windows.juthilo.com)

위 글을 참조로 윈도우에서 로컬로 Jekyll을 설치했다.

동작시 문제 발생.

현재 Jekyll v3.2.0 에는 버그가 있는 거 같다.   
구글링 결과 아래와 같은 글들을 확인할 수 있었다.

관련글:

- [3.2.0 broken on Windows #5146](https://github.com/jekyll/jekyll/issues/5146)

- [Error: different prefix: "/" and "G:/" #4677](https://github.com/jekyll/jekyll/issues/4677)

- [Layout: set relative_path without using Pathname #5164](https://github.com/jekyll/jekyll/pull/5164)

- [Error while running “ jekyll serve ” command - stackoverflow](http://stackoverflow.com/questions/38691001/error-while-running-jekyll-serve-command)  



### 해결방법

```
gem uninstall jekyll -v 3.2.0    
gem install jekyll -v 3.1.6
```

### Jekyll 설치와 관련된 글 모음

- [지킬로 깃허브에 무료 블로그 만들기 - 15 Oct 2013](http://nolboo.kim/blog/2013/10/15/free-blog-with-github-jekyll/)

- [Setting up your GitHub Pages site locally with Jekyll](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/#platform-mac)  

    > Mac, Windows, Linux 모두 설명되어 있음.

- [How to set up a blog with Jekyll and Github Pages - Part 1](http://anandmanisankar.com/posts/set-up-blog-jekyll-github-pages/)  
