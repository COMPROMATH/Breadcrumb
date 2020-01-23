# Breadcrumb
Updated Breadcrumb List for Blogger Platform 2020
```html
<!--CUSTOM BREADCRUMB START-->
<b:if cond='data:blog.pageType == "item"'>
<div class="breadcrumb-outer">
<div itemscope='' itemtype="http://schema.org/BreadcrumbList">
<b:if cond='data:post.labels'>
<span itemprop="itemListElement" itemscope='' itemtype="http://schema.org/ListItem"><a expr:href='data:blog.homepageUrl' itemprop="item"><span style='padding-left:8px;' itemprop="name">Home</span></a><meta itemprop="position" content="1" /></span>»
<b:loop values='data:post.labels' var='label' index='i'>
<b:if cond='data:i == 0'>
<span itemprop="itemListElement" itemscope='' itemtype="http://schema.org/ListItem"><a expr:href='data:label.url + "?&amp;max-results=7"' itemprop="item"><span itemprop="name"> <data:label.name/></span></a><meta itemprop="position" expr:content='data:i + 2' /></span><b:if cond='data:label.isLast != "true"'/>»
</b:if> <!--CONDITION-->
</b:loop>
</b:if>
<span class="breadcrumb-title" expr:title='data:post.title'>
<data:post.title/>
</span>
</div>
</div>
<!--CUSTOM BREADCRUMB STOP-->
```
See Details - [Fix Data-Vocabulary.Org Schema Deprecated Error In Blogger](https://www.compromath.com/2020/01/fix-data-vocabularyorg-schema.html "Fix Data-Vocabulary.Org Schema Deprecated Error In Blogger")
