---
layout: post
title: "zsh: no matches found:"
date: 2014-10-29 21:23:35 +0900
comments: true
categories: [zsh]
---
zshを使うとたまに以下のエラーがあわられる

```
rsync -avz server:*.abc .
zsh: no matches found: server:*.abc
```

この場、クォーテーションで囲むと解決できる

```
rsync -avz "server:*.abc" .
```

