---
title: 'Blog Setup with Nested Staticman Comments'
date: 2020-05-23
permalink: /posts/2020/05/blog-setup-with-nested-staticman-comments/
---

This blog contains the steps I used to set up this blog repository.

The repository was forked from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/), which is © 2016 Michael Rose and released under the [MIT License](https://github.com/mmistakes/minimal-mistakes/blob/master/LICENSE).

Here is a handy [Quick Start Guide](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/) useful for the initial setup.

[Staticman](https://staticman.net/) commenting platform is added to blog posts. I followed the [instructions](https://travisdowns.github.io/blog/2020/02/05/now-with-comments.html) provided by Travis Downs to implement nested comments.

One [bug](https://stackoverflow.com/q/10636667) that occurred during the deployment process is after hitting the ‘Submit’ button to add a comment, Bootstrap modal appearing underneath the grey fade and is noneditable. This [behavior](https://stackoverflow.com/a/11788713) occurs when the modal container has a fixed or relative position or is within an element with a fixed or relative position. I was able to fix this issue by replacing the Bootstrap modal with [Sweetalert2](https://github.com/sweetalert2/sweetalert2). You can find my fix in this [commit](https://github.com/qfang6/qfang6.github.io/commit/4be0eabfbf877ed29fe0a56f925815d0ff40da68)

Hopefully these resources will help you start on your own blog on Github.


##### Reference:

[Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/)<br/>
[Travis Downs](https://travisdowns.github.io/)<br/>
[Staticman](https://staticman.net/)<br/>
[Sweetalert2](https://github.com/sweetalert2/sweetalert2)

{% if page.comments == true %}
  {% include comments.html %}
{% endif %}
