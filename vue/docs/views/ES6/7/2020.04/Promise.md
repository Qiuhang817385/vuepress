---
title: Promise
date: 2020-04-02
categories:
  - ES6/7
author: 安若天
---

## 在 Promise 当中,调用原生的 ajax 需要注意的地方

```js
由于readyState的状态码有5个0-4 所以会调用4次ajax函数
如果是下面那种判断,那么第一次初始化的时候就会进入reject状态

xhr.onreadystatechange = function() {
  if (xhr.readyState === 4) {
    if (xhr.status == 200) {
      resolve(xhr.responseTest)
    } else {
      reject('暂时获取不到数据')
    }
  }
}

错误的写法

xhr.onreadystatechange = function() {
  if (xhr.readyState === 4 && xhr.status == 200) {
    resolve(xhr.responseTest)
  } else {
    reject('暂时获取不到数据')
  }
}
```
