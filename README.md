#### react-native-img-with-placeholder

### 简介

`react-native-img-with-placeholder`控件封装了默认图片的功能。

当图片加载中或者加载失败(比如地址不正确)时，显示默认图片。
当图片加载成功时，移除默认图片。

### 属性

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
