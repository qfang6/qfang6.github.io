---
title: 'Setting up the Blog'
date: 2020-05-23
permalink: /posts/2020/05/setting-up-the-blog/
comments: true
---

This blog contains the steps I used to setup this blog repository.

The [repository](https://github.com/qfang6/qfang6.github.io) was forked from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/), which is © 2016 Michael Rose and released under the MIT License. See [LICENSE](https://github.com/mmistakes/minimal-mistakes/blob/master/LICENSE).

I followed the [Quick Start Guide](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/) provided by Michael Rose to perform the initial setup for the blog.

[Staticman](https://staticman.net/) commenting platform is added to blog posts. I followed the [blog instructions](https://travisdowns.github.io/blog/2020/02/05/now-with-comments.html) provided by Travis Downs. Part of the reason why I wrote this blog is to test the comment functionality.

Hopefully these resources will help you to start on your own blog on Github.


##### Reference:

[Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/)<br/>
[Travis Downs](https://travisdowns.github.io/)<br/>
[Staticman](https://staticman.net/)

{% if page.comments == true %}
  {% include comments.html %}
{% endif %}
