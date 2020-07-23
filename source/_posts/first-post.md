---
extends: _layouts.post
section: content
title: This is my first post
date: 2020-12-24
description: This is fist post description 
categories: [html, css]
featured: true
excerpt: This is excerpt Lorem ipsum dolor sit amet, consectetur adipisicing elit. Cupiditate, earum.
---



## Laravel now supports pagination style for tailwind.      
```php
{{ $tweets->links('pagination::tailwind') }}

```


##   foreign relationship

```php 
Schema::table('likes', function (Blueprint $table) {
    $table->foreignId('user_id');

    $table->foreign('user_id')->references('id')->on('users')->onDelete('cascade');
});
```                        
###  Both are same                  
```php 
Schema::table('liskes', function (Blueprint $table) {
    $table->foreignId('user_id')->constrained()->onDelete('cascade');
})
```       



##  Use Turbolink for      
    access/go navigation subpage without Reload full site/page
    @faster


```js
   <script src="https://unpkg.com/turbolinks"></script>
```