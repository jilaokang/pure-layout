## Layout

布局繁琐复杂，和其他的css不同，每次写的时候整个页面穿插着flex, float, grid, -margin, line-height, table等，为了实现我们的布局需求，在该方面非常混乱，页面布局非常适合用于抽象出来单独作为一个库，方便开发人员快速开发，更好的后期维护。

[效果预览](https://jilaokang.club/layout/example/)

<br/>

### 介绍
通过将整个页面划分成不同的行与列，共同构建起了栅格化系统，方便开发者进行排版布局，解决前端布局难题。

该库支持行内嵌套，实现了2\*3\*4\*5列所有可能性的布局需求。

为使显示效果更加，该库支持响应式式布局，通过`col`、`col-xs`的形式区分是PC端还是移动端，从而显示出不同的效果。

<br/>

### 导入 

方式一： 在线链接

```html
<link rel="stylesheet" href="http://pd37peogt.bkt.clouddn.com/main.css">
```
方式二：npm

````bash
npm i tq-layout --save
````
````js
import 'tq-layuot/main.css'
````

<br/>

### 功能
|      | 栅格化  | 响应式     | 列偏移                         | 父包裹 |
| ---- | ------- | ---------- | ------------------------------ | ------ |
| 10格 | col-10  | col-xs-10  | col-offset-2 col-offset-xs-12  | row    |
| 12格 | item-12 | item-xs-12 | item-ofsset-2 col-offset-xs-12 | row    |

<br/>

### 使用

逻辑：将页面划分成多行，再将一行划分成多列，从而实现栅格化布局。

#### 1.划分成一行

````html
<div class="row">
    ...
</div>
````

#### 2.划分成多列

````html
<div class="row">
    <div class="col-1">这个版块给1格</div>
    <div class="col-5">这个版块占5格</div>
</div>
````

#### 3.响应式布局

响应式：通过检测显示窗口尺寸不同，从而动态的显示布局效果。

````html
<div class="row">
    <div class="col-1 col-xs-10">在电脑上占1格，手机上占10格</div>
    <div class="col-5 col-xs-5">在电脑上占5格，手机上占5格</div>
</div>
````

#### 4.offset

列偏移：在部分我们用不到的区域可以采用列偏移的方式将其空出来。

````html
<div class="row">
    <div class="col-5 col-offset-4">
        左边空出4格，版块占5格
    </div>
</div>
````

#### 5.col & item

- col将一行划分成10格

- item将一行划分成12格

两者功能写法完全相同

<br/>

### API大礼包

APi速记：水平方向_垂直方向 .center_middle。

注意：我们将行列构成页面的栅格化，将内容作为版块放进去。切忌出现栅格混乱，内容栅格混为一体公用同一个块级标签。


|    | 从顶开始 | 水平垂直     | 从底开始 |
| -- | :----------:| ---------------- | :--------: |
| 左 |      x      | left_middle   |   x       |
| 中 |     x       | center_middle |     x     |
| 右 |      x      | right_middle |    x      |

#### 示例

````html
<div class="row">
    <div class="col-3">
        <div class="center_center" style="height:10vh">
            我们都垂直居中在一个版块里
            <p>垂直水平居中的文字</p>
            <img alt="垂直水平居中的图片"/>>
        </div>
    </div>
</div>
````

<br/>

如果有适用于布局相关的场景，欢迎[issues](https://github.com/jilaokang/layout/issues)。

Licenses under the [MIT](https://opensource.org/licenses/MIT) license.
