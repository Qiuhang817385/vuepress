---
title: Await/Async
date: 2020-04-02
categories:
  - ES6/7
author: 安若天
---

## Async

### 语法

```js
async function foo() {
  await 异步操作
  await 异步操作
  await 异步操作
  return
}
```

### 基本使用

```js
async function foo() {
  return new Promise(resolve=>)
}
```

### 返回值

```js
let test = () => {
  return 111
}
// 普通函数
async function print() {
  let result = await test()
  clo(result)
}
// Promise函数
async function print() {
  let result = await new Promise.resolve('12')
  clo(result)
  // 不给resolve传递值的话是undefined
  // 传递的话是12
}
```

### sleep 函数

```js
const sleep = (time) => new Promise((resolve) => setTimeout(resolve, time))

// 使用
;async (ctx) => {
  await sleep(250)
  //后续操作
}

不简化的写法
async function foo(time) {
  return new Promise((resolve) => {
    setTimeout(() => {
      resolve()
    }, time)
  })
}
async function text() {
  await foo()
}
```
