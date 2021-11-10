# color-thief

## 功能

提取图片主题色。

```js
getPalette(image [, colorCount, quality]
```

### 参数：

- image：要提取主题色的图片。
- colorCount：可选参数，提取的主题色数量。
- quality：可选参数，必须为 1 或更大的整数，默认为 10。该数字确定在采样下一个像素之前跳过多少像素。数字越大，返回值的速度就越快。

### 返回值：

```js
[[数字，数字，数字]，...]
```

从图像中获取的调色板数组，每种颜色本身都是一个由三个整数组成的数组，分别代表 RGB。

## 使用

```js
var colorThief = new ColorThief()
var themeColors = colorThief.getPalette(
  image,
  4
)
```
