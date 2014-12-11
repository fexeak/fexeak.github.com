---
title: 修改gor的Markdown渲染方式
date: '2013-12-10'
description:
categories:

tags: Gor

---


　　[wendal的gor](https://github.com/wendal/gor)在遇到code block的时候会不足, 把其markdown部分用官方Blackfriday替代后可以解决。

---

*下面是对Markdown语法的一些测试:*

---

# The largest heading 
## The second largest heading 

...

###### The 6th largest heading 

> Pardon my french

*This text will be italic*

**This text will be bold**

**Everyone _must_ attend the meeting at 5 o'click today.**

* Item
* Item
* Item

- Item
- Item
- Item

1. Item 1
2. Item 2
3. Item 3

1. Item 1
    1. A corollary to the above item.
    2. A corollary to the above item.
2. Item 2
    * A corollary to the above item.
        * A corollary to the above item.
        * A corollary to the above item.
3. Item 3

Here's an idea: why don't we take `SuperiorProject` and turn it into `**Reasonable**Project`.

Check out this neat program I wrote:

```
x = 0
x = 2 + 2
what is x
```

do_this_and_do_that_and_another_thing.

http://example.com

~~Mistaken text.~~

Here's an example:

```
function test() {
  console.log("notice the blank line before this function?");

}
```

```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```

First Header  | Second Header
------------- | -------------
Content Cell  | Content Cell
Content Cell  | Content Cell

| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

| Name | Description          |
| ------------- | ----------- |
| Help      | ~~Display the~~ help window.|
| Close     | _Closes_ a window     |


| Left-Aligned  | Center Aligned  | Right Aligned |
| :------------ |:---------------:| -----:|
| col 3 is      | some wordy text | $1600 |
| col 2 is      | centered        |   $12 |
| zebra stripes | are neat        |    $1 |

