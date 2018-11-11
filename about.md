---
layout: page
title: "About"
description: "文明其精神，野蛮其体魄"
header-img: "img/post-BeachSoccerBoys.jpg"
---



我是张哲，中科院一名研究生。
### 最近阅读
> 《曾国藩传》
 《红星照耀中国》
 《三体》


### 联系

- [博客：Z](https://philosopherz.github.io/)    
- 邮箱：zhangzhe@mail.iap.ac.cn 
- [github](https://github.com/PhilosopherZ)

<div class="zh post-container">

    <ul>
        <li><a href="https://analytics.google.com/analytics">Google Analytics</a></li>
    </ul>
</div>


<!-- Gitalk 评论 start  -->
{% if site.gitalk.enable %}
<!-- Gitalk link  -->
<link rel="stylesheet" href="https://unpkg.com/gitalk/dist/gitalk.css">
<script src="https://unpkg.com/gitalk@latest/dist/gitalk.min.js"></script>

<div id="gitalk-container"></div>
    <script type="text/javascript">
    var gitalk = new Gitalk({
    clientID: '{{site.gitalk.clientID}}',
    clientSecret: '{{site.gitalk.clientSecret}}',
    repo: '{{site.gitalk.repo}}',
    owner: '{{site.gitalk.owner}}',
    admin: ['{{site.gitalk.admin}}'],
    distractionFreeMode: {{site.gitalk.distractionFreeMode}},
    id: 'about',
    });
    gitalk.render('gitalk-container');
</script>
{% endif %}
<!-- Gitalk end -->