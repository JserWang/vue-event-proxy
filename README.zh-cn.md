# Vue Event Proxy

[![](https://img.shields.io/badge/zh--cn-中文-orange.svg)](https://github.com/jser-club/vue-event-proxy/blob/master/README.zh-cn.md) [![](https://img.shields.io/badge/en--us-英语-green.svg)](https://github.com/jser-club/vue-event-proxy/blob/master/README.md)

## 介绍

让Vue.js支持全局事件的库，压缩完只有 `1.79kb`。

1. 通过增加前缀实现全局事件
2. 组件销毁自动移除注册的事件

线上实例: [CodeSandbox](https://codesandbox.io/s/xlvz2p79vp)

## 安装
```
$ npm install --save vue-event-proxy
```

## 使用
只需要在 `$on`、`$emit`、`$once` 方法的第一个参数参数添加 `global:` 前缀

```js
import EventProxy from 'vue-event-proxy';
Vue.use(EventProxy);

this.$on('global:EVENT_NAME');
this.$once('global:EVENT_NAME');
this.$emit('global:EVENT_NAME');
```

更多: [https://cn.vuejs.org/v2/api/#vm-on](https://cn.vuejs.org/v2/api/#vm-on)
