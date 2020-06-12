# react-smart-address
[![npm version](https://badge.fury.io/js/react-smart-address.svg)](https://badge.fury.io/js/react-smart-address)

自动识别地址

#### 感觉不错的话，[请点个🌟](https://github.com/gitSirzh/react-smart-address)

## Getting started

Using npm:

```shell
npm install react-smart-address --save
```
or using yarn:

```shell
yarn add react-smart-address
```

## Usage
```javascript
import SmartAddress from 'react-smart-address';

console.log('SmartAddress: ', SmartAddress.smart('河南省商丘市夏邑县李集镇郭庄乡孟朱庄村小张庄66号15518766666 小伙子'));

// SmartAddress: {
//     'address': '郭庄乡孟朱庄村小张庄66号',
//     'city': '商丘市',
//     'cityCode': '4114',
//     'county': '夏邑县',
//     'countyCode': '411426',
//     'name': '小伙子',
//     'phone': '15518766666',
//     'province': '河南省',
//     'provinceCode': '41',
//     'street': '李集镇',
//     'streetCode': '411426104',
// }

```
