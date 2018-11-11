---
layout: page
title: "Tags"
description: "我的航海志"  
header-img: "img/post-bg-unix-linux.jpg"  
---

## 本页使用方法

1. 在下面选一个你喜欢的词
2. 点击它
3. 相关的文章会「唰」地一声跳到页面顶端
4. 马上试试？

## 我的航海志



<!-- Main Content -->
<div class="container">
	<div class="row">
		<div class="col-lg-8 col-lg-offset-2 col-md-10 col-md-offset-1">
            <!-- 标签云 -->
			<div id='tag_cloud' class="tags">
				{% for tag in site.tags %}
				<a href="#{{ tag[0] }}" title="{{ tag[0] }}" rel="{{ tag[1].size }}">{{ tag[0] }}</a>
				{% endfor %}
			</div>

            <!--<blockquote class="tag-comments">
                标签命名规范：
                    <li>行业观察、职位、公司优先使用中文</li>
                    <li>外国产品、术语优先使用英文</li>
            </blockquote>-->

            <!-- 标签列表 -->
			{% for tag in site.tags %}
			<div class="one-tag-list">
			  	<span class="fa fa-tag listing-seperator" id="{{ tag[0] }}">
                    <span class="tag-text">{{ tag[0] }}</span>
                </span>
				{% for post in tag[1] %}
				  <li class="listing-item">
				  <time datetime="{{ post.date | date:"%Y-%m-%d" }}">{{ post.date | date:"%Y-%m-%d" }}</time>
				  <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
				  </li> 				 
				<hr>
				{% endfor %}
			</div>
			{% endfor %}

		</div>
	</div>
</div>


