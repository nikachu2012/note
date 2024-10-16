---
title: Markdown Test
date: 1970-10-13T20:00:10+09:00
draft: true
math: true
tags: ["test"]
categories: ["test"]
---

# head1
## head2
### head3
#### head4
##### head5
###### head6

This is text[^1].  
This is `Inline code`  
[link](https://twitter.com)  

```plain
[Article link]({{</* ref "../second-post/index.md" */>}})
```
---

this is $inline$ math.  
$$
S = \int_a^b f(x)dx = \lim_{\Delta x_k \to 0}\sum_{k=0}^nf(x_k)\Delta x_k
$$

[^1]:前に入力した数式を呼び出せる機能。コマンドラインで上キー(0x26)を押したときと同じ

- default
- **bold**
- *italic*
- ***bold italic***
- ~~deleted~~
    - a
      - b
    - c
- d

1. a
2. b
    1. c
       1. a
    2. d
3. e

### figure

```plain
{{</* image src="hako.jpg" w="300" caption="hako" */>}}
```

{{<image src="image.png" w="200" caption="This is caption" >}}

### table
|Aaaaaaaaaaaa|Bbbbbbbbbbbbb|cccccccccccC|dddddddddddD|
|:--|:--:|--:|--|
|left|center|right|default|

### code
```c
#include <unistd.h>
#include <string.h>
int main(void)
{
    char str[] = "ほたるかわいいいいいいいいいいいいい\n";
    write(1, str, strlen(str))
}
```

### blockquote

> "楽しちゃだめだから"  
> 某高専某教員, 2024, S1教室にて


> "楽しちゃだめだから"  
> 某高専某教員
> > double blockquote


### alert

```plain
> [!NOTE]
> 

> [!TIP]
> 

> [!IMPORTANT]
> 

> [!WARNING]
> 

> [!CAUTION]
> 
```


> [!UNDEF]
> Useful information that users should know, even when skimming content.

> [!NOTE]
> Useful information that users should know, even when skimming content.

> [!TIP]
> Helpful advice for `doing` things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]
> Advises about risks or negative outcomes of certain actions.


### shortcodes
#### tweet
```plain
{{</* tweet user="" id="" */>}}
```


#### gist
```plain
{{</* gist nikachu2012 d6543f3422b2e36c9ce4cc856af7a6dd main.c */>}}
```
