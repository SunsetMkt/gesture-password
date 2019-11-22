<h1 align="center">
  Gesture Password (手势密码)
</h1>

<div align="center">
<img height="300" src="https://user-images.githubusercontent.com/11746742/68995608-735b4a00-08ca-11ea-8402-2d5229beaceb.png"></img>
</div>

## The gesture password repo contains three packages: gesture-password (native version), gesture-password-react (react version), and gesture-password-vue (vue version). You can install the corresponding version as required

## gesture-password Install

```
// npm
npm install gesture-password --save

// yarn
yarn add gesture-password
```

## gesture-password Usage

```
import GesturePassword from 'gesture-password';

const config = {
  id:'gesture',
  width: 375,
  height: 300,
  onChange: (data: any) => console.log(data) // get gesture password
}

const gesturePassword = new GesturePassword(config)

<canvas id='gesture' />
```


## gesture-password-react Install

```
// npm
npm install gesture-password-react --save

// yarn
yarn add gesture-password-react
```

## gesture-password-react Usage

```
import React from 'react';
import GesturePassword from 'gesture-password-react';
export default () => {
  const config = {
    width: 375,
    height: 300,
    onChange: (data: any) => console.log(data) // get gesture password
  };
  return <GesturePassword {...config} />;
};
```

## gesture-password-vue Install


```
// npm
npm install gesture-password --save

// yarn
yarn add gesture-password
```

## gesture-password-vue Usage

// main.js registry
```
import Vue from 'vue'
import GesturePassword from 'gesture-password-vue'
 
Vue.use(GesturePassword)

<template>
  <GesturePassword :rowPont='rowPont' :width='width' :height='height' @onChange="onChange" />
</template>

<script>
export default {
  data() {
    return {
       {
        width: 375,
        height: 300,
        onChange: function(data){
          console.log(data) // get gesture password
        }
    };
  }
};
</script>


```

// Component registry
```
<template>
  <GesturePassword :rowPont='rowPont' :width='width' :height='height' @onChange="onChange" />
</template>

<script>
import GesturePassword from 'gesture-password-vue'
export default {
  components: {
    GesturePassword
  },
  data() {
    return {
       {
        width: 375,
        height: 300,
        onChange: function(data){
          console.log(data) // get gesture password
        }
    };
  }
};
</script>
```
