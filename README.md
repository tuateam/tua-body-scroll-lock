# tua-body-scroll-lock

> inspired by [body-scroll-lock](https://github.com/willmcpo/body-scroll-lock)

<img src="https://img.shields.io/badge/dependencies-none-green.svg" alt="dependencies">
<a href="https://www.npmjs.com/package/tua-body-scroll-lock" target="_blank">
    <img src="https://badgen.net/npm/dm/tua-body-scroll-lock" alt="Downloads per month">
    <img src="https://img.shields.io/npm/v/tua-body-scroll-lock.svg" alt="Version">
    <img src="https://img.shields.io/npm/l/tua-body-scroll-lock.svg" alt="License">
</a>

## 介绍
顾名思义 `tua-body-scroll-lock` 是用来锁住 `body` 滚动的包。并且针对`PC端`和移动端 `ios` 和 `android` 做了不同的处理，保证在各个端都可以完美使用。

## 安装

```bash
$ npm i -S tua-body-scroll-lock
# OR
$ yarn add tua-body-scroll-lock
```

## 使用

### 移动端

```js
import { lock, unlock } from 'tua-body-scroll-lock'

// 禁止滑动后还需要内部可以滚动的元素(针对移动端ios处理)
const targetElement = document.querySelector("#someElementId");

lock(targetElement)
unlock(targetElement)
```
### PC端

> tips: PC端不需要targetElement; 不传targetElement也不想要控制台提示可以传`null`

```js
import { lock, unlock } from 'tua-body-scroll-lock'

lock()
unlock()
```

## 测试
[测试链接](https://tuateam.github.io/tua-body-scroll-lock)

![bodyScrollLock](./tua-bsl.png)
