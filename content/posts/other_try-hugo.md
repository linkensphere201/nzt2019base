---
title: "启用一个新blog（Hugo试用）"
date: 2020-11-07T21:26:49+08:00
description: "usages"
categories:
  - "CheatSheets"
tags:
  - "hugo"
menu: main # Optional, add page to a menu. Options: main, side, footer

thumbnail: "resources/rd3pjw.jpg" # Thumbnail image
lead: "Example lead - highlighted near the title" # Lead text
comments: false # Enable Disqus comments for specific page
authorbox: true # Enable authorbox for specific page
pager: true # Enable pager navigation (prev/next) for specific page
toc: true # Enable Table of Contents for specific page
mathjax: true # Enable MathJax for specific page
sidebar: "right" # Enable sidebar (on the right side) per page
widgets: # Enable sidebar widgets in given order per page
  - "search"
  - "recent"
  - "taglist"
---

## Hugo试用

- 基本流程走通：post -- publish
- basic configs
- basic markdown
- config the markup(code pieces)
- insert an image by ref as in static or by a shortcode
- organizations (page resources/bundles, )


### Shortcode

A shortcode is a simple snippet inside a content file that Hugo will render using a predefined template. Note that shortcodes will not work in template files.

```
{{< figure src="../../resources/rd3pjw.jpg" title="DeviantArt" >}}
```


## Test for markdown

* a1
* a2xxx
    1. a
    1. x
    1. 888

* an example code piece

```c++
auto tabs = std::make_shared<SmManager::DbTableArray>();
if (!SmManager::find_all_opened_tables(*tabs)) {
  log_warn("failed to find opened table...");
  is_deleting_.store(false);
  return false;
}
std::thread(SlotDeleter::do_purge_slots, 
    tabs, slvec, std::ref(is_deleting_)).detach();
```


> 引用文本 Blockquotes

引用的行内混合 Blockquotes

> 引用：如果想要插入空白换行`即<br />标签`，在插入处先键入两个以上的空格然后回车即可，[普通链接]("/")。

## GFM task list
- [x] GFM task list 1
    - [ ] GFM task list 3-2
    - [ ] GFM task list 3-3
- [ ] GFM task list 4
    - [ ] GFM task list 4-1
    - [ ] GFM task list 4-2

| Left-Aligned  | Center Aligned  | Right Aligned |
| :------------ |:---------------:| -----:|
| col 3 is `fuck()` | some wordy text | $1600 |
| col 2 is      | centered        |   $12 |
| zebra stripes | are neat        |    $1 |

