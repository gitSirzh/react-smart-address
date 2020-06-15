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
### 支持以下格式

#### 注意：地址、姓名、电话 用空格或者特殊字符分开
特殊字符(可自行添加：./node_modules/react-smart-address/src/address_parse.js line:389)：
```
~!@#$^&*()=|{}':;',\\[\\].<>/?~！@#￥……&*（）——|{}【】‘；：”“’。，、？-
```

1. 河北省唐山市古冶区赵各庄街道胜利路66号10楼1002室,小伙子，15518720000
2. 小伙子，河北省唐山市古冶区赵各庄街道胜利路66号10楼1002室 15518720000
3. 河北省唐山市古冶区赵各庄街道胜利路66号10楼1002室 小伙子 15518720000
4. 古冶区赵各庄街道胜利路66号10楼1002室 小伙子 15518720000
5. 河北省唐山市古冶区赵各庄街道胜利路66号10楼1002室 15518720000 小伙子
6. 河北省唐山市古冶区赵各庄街道胜利路66号10楼1002室15518720000 小伙子
7. 河北省唐山市古冶区赵各庄街道胜利路66号10楼1002室150-1872-0000 小伙子

### 不支持的数据格式

河北省唐山市古冶区赵各庄街道胜利路66号10楼1002室小伙子15518720000

## 使用
```javascript
import SmartAddress from 'react-smart-address';

let address = SmartAddress.smart('河北省唐山市古冶区赵各庄街道胜利路66号10楼1002室 15518720000 小伙子');
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
