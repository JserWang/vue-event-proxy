# Vue Event Proxy

## Introduction

Let Vue.js support global events

## Usage
Just add `global:` prefix

```
  import EventProxy from 'vue-event-proxy';
  Vue.use(EventProxy);

  this.$on('global:EVENT_NAME');
  this.$emit('global:EVENT_NAME');
  
```

More see: [https://cn.vuejs.org/v2/api/#vm-on](https://cn.vuejs.org/v2/api/#vm-on)
