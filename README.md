# color3d [![NPM version](https://img.shields.io/npm/v/color3d.svg?style=flat)](https://npmjs.org/package/color3d)

Display color spaces with three.js.

![screen shot](https://user-images.githubusercontent.com/507615/29872910-161eb9e0-8dc4-11e7-94f9-722770872a95.png)

- [Live Demo](https://afc163.github.io/color3d)
- [Color Space Online Tool](http://afc163.github.io/color3d/tool.html)

## Install

```
npm install color3d --save
```

## Usage

```jsx
import Color3d from 'color3d';

const color3d = new Color3d([
  "#FFF0F6",
  "#FFD6E7",
  "#FFADD2",
  "#FF85C0",
  "#F759AB",
  "#EB2F96",
  "#C41D7F",
  "#9E1068",
  "#780650",
  "#520339",
], {
  spaceMode: 'hsv',
  background: '#000000',
});

// render into dom
color3d.render(document.getElementById('container'));

// change colors
color3d.updateData([
  "#F0F5FF",
  "#D6E4FF",
  "#ADC6FF",
  "#82A2FA",
  "#5579ED",
  "#2D51E0",
  "#1C36BA",
  "#0F2194",
  "#05106E",
  "#030747",
]);

// change color space
color3d.changeSpaceMode('hsl');  // hsv, hsl, rbg, lab
```
