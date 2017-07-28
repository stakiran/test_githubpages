---
layout: default
title: トップページ
---

# リスト

redcarpet だと全部 ok だった。

アスタリスク表記のリストです。

* リスト
  * list
  * list

ハイフン表記のリストです

- リスト
  - list
  - list

リストのインデントスペースは何個？2個？

- list
  - list1
    - list2
      - list3

それとも 4 個？
- list
    - list1
        - list2
            - list3

# コードハイライト

python

```python
print 'hello world.'
```

c

```c
#include <stdio.h>

int main(){
  printf("Hello world.\n");
  return 0;
}
```

# リテラル
`こんにちは`

`hello`

`python -c "print 'hello world.'"`

# 画像
![rabbit](img/rabbit.jpg)

# リンク
- URL直 https://github.com/stakiran
- Page1へのリンク、正しいのはどれ？
  - `/page1.md` [Page1](/page1.md)
  - `/page1.html` [Page1](/page1.html) ← redcarpet だとこいつ以外は全部いけた
  - `page1.md` [Page1](page1.md)
  - `page1.html` [Page1](page1.html)
