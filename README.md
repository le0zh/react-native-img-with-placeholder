# react-native-img-with-placeholder

[![npm version](https://badge.fury.io/js/react-native-img-with-placeholder.svg)](https://badge.fury.io/js/react-native-img-with-placeholder)


`react-native-img-with-placeholder`is used to display image with placeholder.

When image is loading, placeholder(aka default image) will be displayed.
After image is loaded successfullly, placeholder will be removed to reduce view count.

## Install

```
npm install react-native-img-with-placeholder --save
```

## Props

| props | type | desc |
| -- | -- | -- |
| source | ImageSource | image source  |
| placeHolderSource | number | placeholder，local image, `require('path')` |
| style? | object | image style |

### 用法

```js
import ImageWithPlaceHolder from 'react-native-img-with-placeholder';

<ImageWithPlaceHolder
  style={styles.inner}
  source={{ uri: 'http://xxxx/f190c59d6e014a97831c471777863301.jpg' }}
  placeHolderSource={require('./img/default.png')}
/>
```

----

`react-native-img-with-placeholder`控件封装了默认图片的功能。

当图片加载中或者加载失败(比如地址不正确)时，显示默认图片。
当图片加载成功时，移除默认图片。

## 安装

```
npm install react-native-img-with-placeholder --save
```

## 属性

| 属性名 | 类型 | 说明 |
| -- | -- | -- |
| source | ImageSource | 将要显示的图片源，一般是网络图片 |
| placeHolderSource | number | 默认图片，必须时本地图片，一般是通过`require('path')`得到的资源id |
| style? | object | 样式 |

### 用法

```js
import ImageWithPlaceHolder from 'react-native-img-with-placeholder';

<ImageWithPlaceHolder
  style={styles.inner}
  source={{ uri: 'http://xxxx/f190c59d6e014a97831c471777863301.jpg' }}
  placeHolderSource={require('./img/default.png')}
/>
```
