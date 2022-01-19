## pure-layout

[![npm](https://badge.fury.io/js/tq-layout.svg)](https://www.npmjs.com/package/tq-layout)
![language](https://img.shields.io/badge/language-scss-blue.svg)



### 介绍
[效果预览](https://jilaokang.github.io/pure-layout/example/)

一个纯粹的布局框架，实现功能有：
1. 响应式
2. 12列，10列布局
3. offset列位移
4. 9种行内布局
5. 3种占位方式
6. 2种占位控制
7. 0 padding，margin困扰

### Usage

#### 项目引入

```bash
npm i tq-layout --save
```

```js
import "tq-layuot/main.css";
```


#### 栅格布局

|       | 栅格化  | 响应式     | 列偏移                         | 父包裹 |
| ----- | ------- | ---------- | ------------------------------ | ------ |
| 10 格 | col-10  | col-xs-10  | col-offset-2 col-offset-xs-12  | row    |
| 12 格 | item-12 | item-xs-12 | item-ofsset-2 col-offset-xs-12 | row    |


#### 行内布局

APi 速记：水平方向\_垂直方向 .center_middle。

|     |  从顶开始  | 水平垂直      |   从底开始    |
| --- | :--------: | ------------- | :-----------: |
| 左  |  left_top  | left_middle   |  left_bottom  |
| 中  | center_top | center_middle | center_bottom |
| 右  | right_top  | right_middle  | right_bottom  |

#### 基础布局

|      |  左  | 中     |  右   |
| ---- | :--: | ------ | :---: |
| 位置 | left | center | right |

#### 占位控制

|      |  两边  |  居中   |
| ---- | :----: | :-----: |
| 位置 | around | between |
