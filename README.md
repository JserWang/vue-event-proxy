# Vue Event Proxy

[![](https://img.shields.io/badge/zh--cn-中文-orange.svg)](https://github.com/jser-club/vue-event-proxy/blob/master/README.zh-cn.md) [![](https://img.shields.io/badge/en--us-英语-green.svg)](https://github.com/jser-club/vue-event-proxy/blob/master/README.md)

## Introduction

Let Vue.js support global events

1. Global events are implemented by adding a prefix
2. Registered event will be removed when component is destroyed

Demo: [CodeSandbox](https://codesandbox.io/s/xlvz2p79vp)

## install
```
$ npm install --save vue-event-proxy
```


## Usage
Just add `global:` prefix to first argument of methods: `$on`, `$emit`, `$once`

```js
import EventProxy from 'vue-event-proxy';
Vue.use(EventProxy);

this.$on('global:EVENT_NAME');
this.$once('global:EVENT_NAME');
this.$emit('global:EVENT_NAME');
```

More see: [https://cn.vuejs.org/v2/api/#vm-on](https://cn.vuejs.org/v2/api/#vm-on)
