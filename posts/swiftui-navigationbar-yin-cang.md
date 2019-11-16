---
title: 'SwiftUI NavigationBar 隐藏'
date: 2019-11-14 15:34:34
tags: [SwiftUI,NavigationBar]
published: true
hideInList: false
feature: 
---
虽然在View 中有 `navigationBarHidden` 的方法，
![](http://v1ki.top//post-images/1573717474447.png)
但是,实际使用时却需要注意，如果没有设置 `title` 的情况下，
![](http://v1ki.top//post-images/1573717482360.jpg)
就设置 Hidden方法， 是不会生效的。

![](http://v1ki.top//post-images/1573717724985.png)


但是。如果设置了`title` 之后，就可以隐藏了。
![](http://v1ki.top//post-images/1573717769286.png)


另外，需要注意的是API中提到 了。 `This modifier only takes effect when this view is inside of and visible within a NavigationView.` , 也就是说只能在 `NavigationView` 中的可见 `View` 才会生效。