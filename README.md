# react-smart-address
[![npm version](https://badge.fury.io/js/react-smart-address.svg)](https://badge.fury.io/js/react-smart-address)

自动识别收货地址

#### 感觉不错的话，[请点个🌟](https://github.com/gitSirzh/react-smart-address)

## 安装

npm:

```shell
npm install react-smart-address --save
```
yarn:

```shell
yarn add react-smart-address
```

## 使用
```javascript
import SmartAddress from 'react-smart-address';

let address = SmartAddress.smart('河北省唐山市古冶区赵各庄街道胜利路66号10楼1002室15518720000 小伙子');
console.log('SmartAddress: ' + address);

// SmartAddress: {
// "address": "胜利路66号10楼1002室",
// "city": "唐山市",
// "cityCode": "1302",
// "county": "古冶区",
// "countyCode": "130204",
// "name": "小伙子",
// "phone": "15518720000",
// "province": "河北省",
// "provinceCode": "13",
// "street": "赵各庄街道",
// "streetCode": "130204004"
// }

```
