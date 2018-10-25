# By-Health Native App Jssdk

汤臣倍健营养家App

### 安装

 * Yarn: `yarn add @byhealth/native-app-jssdk@next`
 * NPM: `npm install @byhealth/native-app-jssdk@next --save`

### 使用

```javascript
import { scanQrCode, closeWindow } from '@byhealth/native-app-jssdk';

scanQrCode()
  .then(result => {
    // result 是识别后的结果
    console.log(result);
  });

closeWindow();
```

### 更新

 * 生成 TypeScript 类型定义，使用 VSCode 可获得更佳体验；
 * 无回调或返回的接口，不再返回Promise对象；
 * 重写 iOS 端调用方法，支持连续调用接口（1.x不支持）；
 * 部分接口名称或参数变化：
   - `userInfo()` => `getUserInfo()`

## API 文档

[文档地址](https://by-healthfed.github.io/native-app-jssdk/)
