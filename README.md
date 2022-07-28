# React-native-Responsive-Font-size
# Introduction

[![Platform](https://img.shields.io/badge/platform-react--native-lightgrey.svg)](http://facebook.github.io/react-native/)[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/heyman333/react-native-responsive-fontSize/blob/master/LICENSE)<a href="https://www.npmjs.com/package/react-native-responsive-fontsize">
<img alt="npm version" src="http://img.shields.io/npm/v/react-native-responsive-fontsize.svg?style=flat-square">
</a>

<strong>Use this library if you have a small problem with the font size 🎉</strong>

<hr />

# How to install

```shell
yarn add react-native-responsive-fontsize
```

or

```shell
npm install react-native-responsive-fontsize --save
```

#### How it looks on different device sizes

|                                                               iPhone SE                                                                |                                                               iPhone X                                                                |
| :------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------: |
| <img src="https://raw.githubusercontent.com/heyman333/react-native-responsive-fontSize/master/images/SE.png" width="320" height="568"> | <img src="https://raw.githubusercontent.com/heyman333/react-native-responsive-fontSize/master/images/X.png" width="385" height="812"> |

# Methods

|              |                  arguments                   | Description                                                                                         |
| :----------: | :------------------------------------------: | --------------------------------------------------------------------------------------------------- |
| RFPercentage |               percent: number                | The font size is calculated as a percentage of the height(`width` in landscape mode) of the device. |
|   RFValue    | value: number, standardScreenHeight?: number | The font size is calculated based on standardScreenHeight and passed value                          |

- when using `RFValue`'s `standardScreenHeight`
  - default standardScreenHeight is `680`
  - In landscape mode, please pass the `screen width`

# Usage

```javascript
import { RFPercentage, RFValue } from "react-native-responsive-fontsize";

const styles = StyleSheet.create({
  welcome: {
    fontSize: RFValue(24, 580) // second argument is standardScreenHeight(optional),
    textAlign: "center",
    margin: 10,
  },
  instructions: {
    textAlign: "center",
    color: "#333333",
    marginBottom: 5,
    fontSize: RFPercentage(5),
  },
});
```

#### Changelog

[Releases](https://github.com/heyman333/react-native-responsive-fontSize/releases)

#### Credits
[Original Author repository](https://github.com/heyman333/react-native-responsive-fontsize)
